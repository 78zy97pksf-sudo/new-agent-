# Modèles de réponses aux mails

Utilisés par `secretaire-mails`. Écrits avec la voix de Simon (tutoiement,
bienveillant, phrases courtes). Les prix viennent de
`../pole-sport/mon-coaching.md` : si un prix change là-bas, on le change
ici aussi.

**Statut de chaque modèle** : seul simo peut passer un modèle de « à
valider » à « validé par simo ». Tant qu'un modèle est « à valider », les
réponses faites avec lui restent en **brouillon** dans Gmail, quel que soit
le mode écrit dans `regles-mails.md`.

On adapte seulement ce qui est entre crochets `[ ]` : le prénom, la
formule citée par la personne, une phrase pour reprendre sa question. On
ne rajoute ni conseil, ni promesse, ni prix.

Signature commune (à la fin de chaque modèle) :

> Simon
> PUR COACHING · Coach sportif à Huy
> https://pur-coaching.github.io/ · Instagram @simon_ruisseau

---

## M1. Premier contact (demande d'informations)

**Statut : validé par simo (2026-10-08)**
**Quand :** une personne découvre PUR COACHING et demande des infos, les
prix, ou comment ça se passe, sans avoir encore choisi de formule.
**Objet :** reprendre l'objet du mail (« Re: … »).

> Salut [prénom],
>
> Merci pour ton message, et bienvenue chez PUR COACHING !
> Ceci est une première réponse automatique pour que tu aies tout de
> suite les infos. Je reviens ensuite vers toi personnellement.
>
> Voici mes formules à Huy :
>
> - **PUR HEALTH (70 €)** : analyse corporelle Tanita, rapport PDF
>   détaillé avec recommandations, anamnèse complète et plan
>   d'entraînement personnalisé.
> - **PUR GOLD (150 € par mois)** : analyse Tanita chaque mois, test VMA
>   et tests physiques, plan 100 % personnalisé sur 3 mois, conseils
>   nutritionnels adaptés et 2 séances d'accompagnement par mois.
> - **PUR TRACK (35 € la séance d'1 h 30, 300 € les 12, 750 € les 36)** :
>   coaching en présentiel avec moi, plan alimentaire de base, analyse
>   Tanita au début et à la fin.
>
> Tu peux aussi faire une analyse Tanita seule (15 €).
> Les séances et les analyses ont lieu à Huy.
>
> Tu n'habites pas près de Huy ? Je te suis aussi **100 % à distance** :
>
> - **PUR ONLINE (69 € par mois)** : pour les sportifs plutôt autonomes.
>   Plan sur mesure ajusté toutes les 4 semaines, un bilan chaque semaine
>   avec ma réponse sous 48 h, correction de ta technique en vidéo et
>   1 appel vidéo par mois.
> - **PUR ONLINE+ (109 € par mois)** : un suivi serré à distance. Plan
>   ajusté chaque semaine, réponse sous 24 h, 2 appels vidéo par mois,
>   et préparation au semi-marathon ou au marathon si c'est ton objectif.
>
> Les formules à distance durent 3 mois minimum, puis se continuent mois
> par mois. On les démarre après ton anamnèse.
>
> Pour gagner du temps, tu peux déjà remplir ton anamnèse (le
> questionnaire de départ) : il est juste en dessous. Réponds simplement
> à ce mail avec tes réponses et la formule qui t'intéresse. Je te
> proposerai ensuite un premier rendez-vous, à Huy ou en appel vidéo.
>
> À très vite,
> [signature]
>
> [questionnaire d'anamnèse : `questionnaire-anamnese.md`, partie
> « Ton anamnèse PUR COACHING »]

## M2. La personne a choisi une formule

**Statut : validé par simo (2026-10-08)**
**Quand :** la personne dit clairement qu'elle veut une formule (« je
veux commencer PUR GOLD », « je prends le pack 12 séances », « je veux
PUR ONLINE »). On garde seulement les phrases entre crochets qui
correspondent à sa formule.

> Salut [prénom],
>
> Super nouvelle, merci pour ta confiance !
> Ceci est une réponse automatique pour te dire que ta demande pour
> **[formule]** est bien enregistrée.
>
> Récapitulatif : [formule], [prix de la grille], [ce qui est compris, en
> une ligne].
> [Formule à Huy :] Le paiement se fait par virement, ou en liquide pour
> les séances en présentiel. On en parle ensemble au premier rendez-vous.
> [PUR ONLINE ou PUR ONLINE+ :] L'engagement est de 3 mois minimum, puis
> mois par mois. Le paiement se fait par virement, seulement une fois ton
> anamnèse lue : je t'envoie les infos à ce moment-là.
>
> [Si l'anamnèse n'est pas encore reçue :] La prochaine étape : remplir
> ton anamnèse (le questionnaire juste en dessous) et me la renvoyer en
> répondant à ce mail. Elle me permet de préparer ton suivi en toute
> sécurité.
> [Si l'anamnèse est déjà reçue :] J'ai bien ton anamnèse, merci.
>
> Je reviens vers toi personnellement pour fixer notre premier rendez-vous
> [à Huy / en appel vidéo].
>
> À très vite,
> [signature]
>
> [Si l'anamnèse n'est pas encore reçue : questionnaire d'anamnèse,
> `questionnaire-anamnese.md`, partie « Ton anamnèse PUR COACHING »]

## M3. Anamnèse reçue

**Statut : validé par simo (2026-10-08)**
**Quand :** la personne renvoie son anamnèse (réponses au questionnaire).

> Salut [prénom],
>
> Merci, j'ai bien reçu ton anamnèse !
> Ceci est une réponse automatique : je la lis attentivement et je
> reviens vers toi personnellement pour la suite et pour fixer notre
> premier rendez-vous.
>
> À très vite,
> [signature]

Attention : ce modèle ne dit **rien** sur le contenu des réponses (pas de
« tout est bon », pas de commentaire santé). Si le bilan est orange ou
rouge, c'est Simon qui en parle avec la personne, avec le message préparé
par `coach-bilan`.

## M4. Question pratique simple

**Statut : validé par simo (2026-10-08)**
**Quand :** une question dont la réponse est écrite noir sur blanc dans
`mon-coaching.md` ou sur le site : lieu (Huy), coaching à distance
(PUR ONLINE, PUR ONLINE+), moyens de paiement, ce que contient une
formule, prix de la grille.

> Salut [prénom],
>
> Merci pour ta question !
> Ceci est une réponse automatique : [réponse en une ou deux phrases,
> reprise mot pour mot des informations de `mon-coaching.md`].
>
> Si tu as d'autres questions, réponds simplement à ce mail. Je reviens
> vers toi personnellement si besoin.
>
> À très vite,
> [signature]

Si la réponse n'est pas écrite quelque part : on n'utilise pas M4, on
utilise M5.

## M5. Accusé de réception (Simon répond lui-même)

**Statut : validé par simo (2026-10-08)**
**Quand :** un futur client ou un client écrit quelque chose qui demande
Simon : santé, douleur, plainte, demande spéciale, report, question sans
réponse écrite.

> Salut [prénom],
>
> Merci pour ton message, je l'ai bien reçu.
> Ceci est une réponse automatique : je te réponds personnellement très
> vite.
>
> À très vite,
> [signature]

On ne reprend **pas** le contenu santé du mail dans la réponse.

---

## Corrections de simo sur les modèles

(Les plus récentes en haut. Chaque correction est appliquée au modèle
concerné ci-dessus.)

| Date | Modèle | Correction |
|---|---|---|
| 2026-10-08 | Signature | Instagram de Simon (@simon_ruisseau) au lieu de @pur.coaching, à la demande de simo |
| 2026-10-08 | M1, M2, M4 | Ajout des formules à distance PUR ONLINE (69 €/mois) et PUR ONLINE+ (109 €/mois), validées par simo le même jour pour le site |
