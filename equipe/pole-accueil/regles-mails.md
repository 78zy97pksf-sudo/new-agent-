# Règles des mails automatiques

Ces règles s'appliquent à `secretaire-mails` et à la conversation
principale quand elle traite les mails. En cas de doute : **pas de réponse
automatique**, étiquette `3 A voir par Simon`.

## Le mode actuel

**MODE : ENVOI AUTOMATIQUE** (accord de simo le 2026-10-08)

- **BROUILLONS** : les réponses sont préparées en brouillon dans Gmail.
  Rien ne part. Simon relit et clique sur « Envoyer » s'il est d'accord.
- **ENVOI AUTOMATIQUE** : les réponses faites avec un modèle marqué
  « validé par simo » dans `modeles-reponses-mails.md` partent toutes
  seules. Tout le reste reste en brouillon.

Seul simo peut faire passer en ENVOI AUTOMATIQUE (ou revenir en
BROUILLONS). Il suffit qu'il le dise à Claude.

Premier contact à distance (modèle M6) : **envoi automatique** aussi,
décidé par simo le 2026-10-09. Cette décision remplace les « brouillons »
prévus pour ce mail dans `../pole-sport/coaching-distance.md`
(section 2).

## Quand vérifier la boîte

Une fois par jour (routine automatique), vers midi. simo peut demander
plus souvent, mais chaque vérification consomme une partie de son
abonnement Claude.

On regarde les mails de la boîte de réception reçus **depuis la date de
la dernière vérification** (notée dans le résumé précédent ; par défaut
les 2 derniers jours, pour ne rien rater si un jour a sauté), sans les
onglets Promotions et Réseaux sociaux. Une conversation qui porte déjà
l'étiquette `4 Reponse auto envoyee` ou qui a déjà un brouillon de
réponse n'est pas retraitée, sauf si la personne a écrit un nouveau
message depuis.

## Les 5 familles de mails

| Famille | Exemples | Ce qu'on fait |
|---|---|---|
| **A. Demande de coaching** | « Bonjour, je voudrais des infos sur vos formules », « Combien coûte un bilan ? », réponse à une de nos réponses automatiques | Étiquette `1 Prospect` (ou `2 Client`) + réponse avec le bon modèle + `agent-accueil` ouvre ou met à jour le dossier |
| **B. À voir par Simon** | Question de santé ou douleur, plainte, demande de remboursement, partenariat, presse, question à laquelle aucun modèle ne répond, mail en colère, personne qui vit hors de Belgique, sauf si elle veut venir à Huy (le coaching à distance n'y est pas encore ouvert) | Étiquette `3 A voir par Simon` + seulement le modèle « accusé de réception » s'il s'agit d'un futur client ; rien d'autre. Signalé dans le résumé du jour |
| **C. Personnel ou école** | École, stage, incubateur, famille, amis, banque, administration | **Aucune réponse, aucune étiquette.** Si le mail semble important ou urgent (date limite, rendez-vous, rappel), une ligne dans le résumé du jour |
| **D. Publicité et notifications** | Newsletters, promotions, Strava, Apple, réseaux sociaux, confirmations automatiques | **Rien.** On n'en parle pas dans le résumé |
| **E. Douteux** | Arnaque, lien bizarre, demande de mot de passe ou de paiement | **Rien.** Une ligne « mail douteux, ne clique pas » dans le résumé. On ne le supprime pas |

## Jamais de réponse automatique quand…

- l'expéditeur est une adresse « no-reply », « noreply », « mailer »,
  « notification », ou une réponse automatique (absence, « out of
  office ») : ça évite les boucles ;
- Simon a déjà répondu lui-même dans cette conversation, ou le dernier
  message de la conversation vient de Simon ;
- une réponse automatique est déjà partie dans cette conversation et la
  personne n'a rien écrit de nouveau depuis ;
- le mail parle de santé, de douleur, de blessure, de grossesse, de
  médicaments ou de régime (famille B). **Deux seules exceptions** : le
  modèle M3 (anamnèse reçue) et le modèle M5 (accusé de réception), qui
  ne disent rien sur le contenu santé du mail ;
- le mail demande un prix ou une offre qui n'existe pas dans
  `mon-coaching.md` (réduction, offre spéciale, groupe…) ;
- le mail est écrit dans une langue autre que le français (brouillon
  seulement, et on le signale) ;
- la personne semble mineure (on demande alors l'accord d'un parent, via
  Simon).

Au maximum **une** réponse automatique (ou un brouillon) par
conversation et par jour. Si un brouillon de réponse existe déjà dans la
conversation, on n'en crée pas un deuxième.

**Quand une de ces interdictions s'applique** : ni réponse, ni
brouillon. On met l'étiquette `3 A voir par Simon` et on le signale dans
le résumé du jour. (Seule exception : le mail dans une autre langue, où
l'on peut préparer un brouillon.)

## Ce qu'une réponse automatique ne fait jamais

- Fixer, déplacer ou annuler un rendez-vous (c'est Simon qui le fait).
- Donner un conseil de santé, d'entraînement ou de nutrition.
- Promettre un résultat (kilos, temps sur marathon…).
- Donner un prix qui n'est pas dans `mon-coaching.md`, ou une réduction.
- Demander des données bancaires, ou en donner (le numéro de compte est
  donné par Simon lui-même).
- Se faire passer pour Simon qui aurait lu le mail : les modèles disent
  honnêtement que c'est une première réponse et que Simon revient
  personnellement vers la personne.

## Le résumé du jour pour simo

Après chaque vérification, un message court dans le projet :
1. **Ce qui a été fait** (avec la date et l'heure de cette vérification,
   pour que la suivante reparte de là) : nombre de mails traités, réponses envoyées (ou
   brouillons prêts), nouveaux dossiers clients (avec leur code).
2. **Ce qui attend Simon** : une ligne par mail de la famille B, et les
   mails personnels importants (famille C), avec ce qu'il faut faire.
3. **Les clients prêts** : les dossiers où l'anamnèse et le bon de
   commande sont prêts et où il reste seulement à fixer le rendez-vous
   (ou, à distance, l'appel vidéo de bilan gratuit).

Pas de nom complet ni d'information de santé dans le résumé : le code
client et le prénom suffisent.
