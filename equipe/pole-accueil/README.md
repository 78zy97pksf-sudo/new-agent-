# Le pôle accueil

Le pôle accueil s'occupe de **tout ce qui arrive dans la boîte mail** de
PUR COACHING et de **l'arrivée de chaque nouveau client**, pour que tout
soit prêt avant le premier rendez-vous avec Simon.

## ATTENTION : le dépôt GitHub est PUBLIC

Ici, jamais d'adresse e-mail, de nom de client, d'information de santé ni
de montant réel. Les vrais dossiers clients vont dans le **Google Drive
privé de simo**, dossier `Pur Coaching / Clients` :
- un sous-dossier par client, dont le **nom indique où il en est**, par
  exemple `C01 - Julie - PUR GOLD - 3 Prêt pour le rendez-vous` ;
- dans ce dossier : sa fiche contact, son anamnèse, son bilan et son bon
  de commande.

Il suffit d'ouvrir `Pur Coaching / Clients` pour voir tous les clients et
leur étape. (Les outils des agents ne peuvent pas écrire dans un tableau
Google Sheets, d'où ce système de noms de dossiers.)

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
- `../pole-sport/coaching-distance.md` : le protocole du coaching à
  distance (parcours, sécurité, places).

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
   « premier contact » (formules, prix, questionnaire d'anamnèse), ou
   « premier contact à distance » pour une personne qui vit loin de Huy.
2. **Le dossier est ouvert.** `agent-accueil` donne un code client et
   crée le dossier du client dans le Drive (étape `1 Contact`).
3. **L'anamnèse revient.** `agent-accueil` range les réponses dans le
   dossier, puis la conversation principale demande à `coach-bilan`
   l'état du bilan (incomplet, vert, orange, rouge).
4. **La commande potentielle.** Dès que la personne a dit quelle formule
   l'intéresse, `agent-accueil` prépare le bon de commande (formule, prix
   de la grille, paiement, prochaines étapes) dans le dossier.
5. **Simon prend le relais.** Le résumé du jour lui dit : « C03 est prêt :
   anamnèse reçue, feu vert, bon de commande PUR GOLD prêt, il reste à
   fixer le rendez-vous Tanita » (ou l'appel vidéo de bilan gratuit pour
   PUR ONLINE et PUR ONLINE+). Simon fixe le rendez-vous et encaisse ;
   le `comptable` note le paiement.
6. **La suite** se fait avec le pôle sport (programme, contrôle sécurité).

Pour les formules **à distance** (PUR ONLINE, PUR ONLINE+), le parcours
complet est dans `../pole-sport/coaching-distance.md` : questionnaire avec
la partie « À distance », appel vidéo de bilan gratuit, confirmation
écrite, feu final de `coach-bilan` (tri A / B / B bis / C), puis seulement
les conditions et le premier paiement par virement. Pendant la phase
test : 3 clients à distance au maximum (au-delà, Simon décide). Résumé
des règles dans `modele-bon-de-commande.md`.

## La règle d'or

Les agents **préparent**, Simon **décide et rencontre** le client. Une
réponse automatique ne fixe jamais de rendez-vous, ne donne jamais de
conseil de santé et ne promet jamais de résultat.
