# Fonctions gratuites pour la portée et la communauté

Demande de simo (10/11/2026) : « utilise toutes les fonctionnalités gratuites
que tu peux trouver en ligne et qui sont sûres pour devenir virale et amener
une communauté à nous suivre afin de réaliser des ventes et des abonnements ».

Règle : seulement les fonctions **intégrées** à Instagram, TikTok et Metricool
(plan gratuit). Budget 0 €, rien de payant, aucune publicité.

## Ce que l'équipe com fait seule, à chaque post (Metricool)

| Fonction | Comment | Depuis |
|---|---|---|
| Meilleure heure | `getBestTimeToPostByNetwork` avant de programmer. Jeudi : TikTok 18 h (1 378) plutôt que 19 h (999) ; Instagram 18 h (5 078), 10 h est encore mieux (6 275). | 10/11 : épisode 2 sur TikTok passé à 18:00 |
| 1er commentaire Instagram | `firstCommentText` : la question de l'épisode, en réponses numérotées (1, 2, 3). Un « 2 » se tape en une seconde, donc plus de gens répondent. | 10/11 : épisode 2 |
| Question à choix sur TikTok | Dans la légende : « Réponds en commentaire : 1 …, 2 …, 3 … ». Test mesuré le 16/11 (commentaires pour 100 vues). | 9/11 : épisode 2 |
| Duo et Collage TikTok ouverts | `disableDuet` et `disableStitch` à false : d'autres comptes peuvent reprendre la vidéo. | toujours |
| Étiquette IA | `isAiGenerated` (Instagram) et `isAigc` (TikTok) sur chaque vidéo IA : obligatoire, et la plateforme ne la pénalise pas. | toujours |
| Essai Instagram (Trial Reel) | `instagramData.type = TRIAL_REEL` : la vidéo est montrée d'abord à des gens qui ne te suivent pas. Utile pour tester une accroche sans lasser les abonnés. **Seulement si simo le choisit** pour une vidéo sous 8/10. | à proposer |
| Collaboration Instagram | `instagramData.collaborators` : le post apparaît aussi chez un partenaire (salle, club de course de Huy). Il faut son accord d'abord (développeur commercial, puis simo). | à préparer |

## Ce que simo fait lui-même (2 minutes, depuis son téléphone)

1. **Répondre à chaque commentaire dans l'heure** après la sortie du jeudi :
   une conversation au début pousse la vidéo. Commentaire sur la santé :
   seulement « Demande d'abord l'avis de ton médecin »
   (`regles-publication.md`, section c).
2. **Jeudi soir, partager l'épisode en story avec un sticker « Sondage »**
   (1, 2 ou 3) : chaque vote compte comme une interaction.
3. **Épingler les épisodes de la série en haut du profil Instagram**
   (jusqu'à 3) : un nouveau visiteur comprend la série tout de suite.
4. **Une seule fois : brancher dans Metricool une chaîne YouTube et sa fiche
   Google (Google Business Profile)**. Ensuite l'équipe y publie les mêmes
   vidéos (YouTube Shorts) et des nouvelles sur la fiche Google, qui sort
   quand quelqu'un cherche « coach sportif Huy ». À vérifier au premier
   essai : si un post sur plusieurs réseaux compte pour une ou plusieurs
   places du plan gratuit (20 par mois).

## Interdit (pas sûr)

- Acheter des abonnés, des vues ou des commentaires ; groupes d'échange de
  « j'aime » ; applications qui suivent et ne suivent plus à ta place.
- Donner le mot de passe Instagram ou TikTok à une application « pour devenir
  viral ».
- Fausse tendance, faux chiffres, faux avis, faux Simon ou faux client.
- Musique connue ajoutée dans le fichier vidéo (droits d'auteur) : la musique
  reste celle de l'équipe.

## Comment on mesure

Metricool ne montre plus les Reels Instagram publiés après le 19/10 : les
tests se mesurent sur TikTok (vues, commentaires, partages), en comptant les
commentaires **pour 100 vues** quand l'heure ou la portée change.
