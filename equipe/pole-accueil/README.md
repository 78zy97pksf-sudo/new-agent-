# Le pôle accueil

Le pôle accueil s'occupe de **tout ce qui arrive dans la boîte mail** de
PUR COACHING et de **l'arrivée de chaque nouveau client**, pour que tout
soit prêt avant le premier rendez-vous avec Simon.

## ATTENTION : le dépôt GitHub est PUBLIC

Ici, jamais d'adresse e-mail, de nom de client, d'information de santé ni
de montant réel. Les vrais dossiers clients vont dans le **Google Drive
privé de simo**, dossier `Pur Coaching / Clients` :
- le tableau `Suivi clients PUR COACHING` (une ligne par client) ;
- un sous-dossier par client, nommé avec son code (`C01`, `C02`…), qui
  contient son anamnèse et son bon de commande.

## Qui fait quoi

| Agent | Son métier |
|---|---|
| `secretaire-mails` | Lit les nouveaux mails une fois par jour, les trie, range chacun sous une étiquette Gmail, répond automatiquement aux demandes de coaching avec les modèles validés, et fait le résumé du jour pour simo |
| `agent-accueil` | Pour chaque nouveau client : donne un code client, prépare l'anamnèse, la commande potentielle (bon de commande) et le dossier dans le Drive, puis passe le relais au pôle sport |

## Les fichiers communs

- `regles-mails.md` : quels mails reçoivent une réponse automatique, et
  lesquels jamais. Contient le **mode** actuel (brouillons ou envoi
  automatique).
- `modeles-reponses-mails.md` : les réponses types, écrites avec la voix
  de Simon.
- `questionnaire-anamnese.md` : les questions de l'anamnèse envoyées au
  futur client.
- `modele-bon-de-commande.md` : le modèle de la commande potentielle.
- `../pole-sport/mon-coaching.md` : offres et prix (la seule source des
  prix).

## Les étiquettes Gmail

| Étiquette | Pour quoi |
|---|---|
| `PUR COACHING/1 Prospect` | Une personne intéressée qui n'est pas encore cliente |
| `PUR COACHING/2 Client` | Un client qui a choisi une formule |
| `PUR COACHING/3 A voir par Simon` | Simon doit répondre lui-même (santé, plainte, partenariat, question sans réponse dans les modèles…) |
| `PUR COACHING/4 Reponse auto envoyee` | Une réponse automatique est partie (ou un brouillon est prêt) |

Les mails personnels, de l'école, publicitaires ou automatiques ne
reçoivent **aucune étiquette et aucune réponse**.

## Le parcours d'un nouveau client

1. **Le mail arrive.** `secretaire-mails` le reconnaît comme une demande
   de coaching, lui met l'étiquette `1 Prospect` et répond avec le modèle
   « premier contact » (formules, prix, questionnaire d'anamnèse).
2. **Le dossier est ouvert.** `agent-accueil` donne un code client, ajoute
   une ligne au tableau de suivi et crée le dossier du client dans le
   Drive.
3. **L'anamnèse revient.** `agent-accueil` range les réponses dans le
   dossier, puis la conversation principale demande à `coach-bilan`
   l'état du bilan (incomplet, vert, orange, rouge).
4. **La commande potentielle.** Dès que la personne a dit quelle formule
   l'intéresse, `agent-accueil` prépare le bon de commande (formule, prix
   de la grille, paiement, prochaines étapes) dans le dossier.
5. **Simon prend le relais.** Le résumé du jour lui dit : « C03 est prêt :
   anamnèse reçue, feu vert, bon de commande PUR GOLD prêt, il reste à
   fixer le rendez-vous Tanita » (ou le premier appel vidéo pour
   PUR ONLINE et PUR ONLINE+). Simon fixe le rendez-vous et encaisse ;
   le `comptable` note le paiement.

Pour les formules **à distance** (PUR ONLINE, PUR ONLINE+), les règles du
`coach-securite` s'ajoutent : pas de coaching à distance pour une femme
enceinte, une personne mineure ou une personne qui a un problème de cœur,
accord du médecin quand la santé le demande, paiement par virement
seulement après le bilan santé, et 3 clients à distance au maximum pour
commencer (au-delà, Simon décide). Détails dans
`modele-bon-de-commande.md`.
6. **La suite** se fait avec le pôle sport (programme, contrôle sécurité).

## La règle d'or

Les agents **préparent**, Simon **décide et rencontre** le client. Une
réponse automatique ne fixe jamais de rendez-vous, ne donne jamais de
conseil de santé et ne promet jamais de résultat.
