# Organigramme de la micro-entreprise

Le directeur met ce tableau à jour à chaque création ou modification d'agent.

| Agent | Rôle | Exemple de demande |
|---|---|---|
| `directeur` | Crée et organise les agents de l'équipe | « Crée-moi un agent qui prépare mes posts LinkedIn » |
| `chef-de-projet` | Découpe une grosse mission et répartit les tâches | « Organise le lancement de ma nouvelle offre » |
| `chercheur` | Se renseigne et résume des informations fiables | « Trouve les 5 meilleurs outils de facturation pour freelance » |
| `redacteur` | Écrit et améliore des textes | « Rédige un e-mail de relance pour un client » |
| `controleur-qualite` | Relit et vérifie un travail terminé | « Vérifie ce plan avant que je l'envoie » |
| `directeur-croissance` | Fait chaque semaine le tour de toute l'entreprise et choisit les 3 améliorations de la semaine | « Qu'est-ce qu'on améliore cette semaine ? » |

## Pôle sport

Crée des programmes sportifs complets et sûrs pour les clients de simo.
Fonctionnement détaillé, règles et modèles : `equipe/pole-sport/`.

| Agent | Rôle | Exemple de demande |
|---|---|---|
| `coach-bilan` | Fait le bilan du client (questions, questionnaire santé) et donne un état : bilan incomplet, feu vert / orange / rouge | « Fais le bilan de Julie, 35 ans, débutante, veut perdre du poids » |
| `coach-programmeur` | Construit le programme complet (8 à 12 semaines) à partir de la fiche client, et programmes types à revendre | « Crée le programme de Julie à partir de sa fiche » |
| `coach-nutrition` | Coach nutrition et hygiène de vie : donne des conseils généraux d'hygiène de vie et d'alimentation, non médicaux | « Prépare des conseils d'hygiène de vie pour accompagner le programme de Julie » |
| `coach-securite` | Vérifie la sécurité de chaque programme avant livraison : « validé » ou « à corriger » | « Contrôle la sécurité du programme de Julie » ou « Contrôle le programme type remise en forme débutant » |

**Enchaînement des étapes :** bilan (`coach-bilan`) → programme
(`coach-programmeur`) → conseils d'hygiène de vie si demandés
(`coach-nutrition`) → contrôle sécurité (`coach-securite`) → contrôle de la
forme (`controleur-qualite`) → livraison par simo. C'est la conversation
principale qui lance chaque étape, l'une après l'autre.

**Programme à revendre :** programme type (`coach-programmeur`, rangé dans
`equipe/pole-sport/programmes-a-vendre/`) → contrôle sécurité grille
« programme type » (`coach-securite`) → `controleur-qualite` → mise en vente
par simo.

Attention : le dépôt est public, aucune vraie donnée de client (nom complet,
santé) ne doit y être enregistrée. Utiliser un code client.

## Pôle marketing

Fait vivre la marque PUR COACHING sur Instagram et TikTok et l'améliore en
continu. Fonctionnement détaillé, charte et règles : `equipe/pole-marketing/`.

| Agent | Rôle | Exemple de demande |
|---|---|---|
| `responsable-marque` | Agent marketing : garde la charte, veille à ce que tous les canaux disent la même chose, planifie le calendrier éditorial du mois, fait le bilan des statistiques et note les leçons | « Prépare le calendrier d'octobre » ou « Voici mes statistiques du mois, fais le bilan » |
| `commercial-instagram` | Posts, carrousels, scripts de Reels, stories, légendes, hashtags et modèles de réponses aux messages privés | « Écris le carrousel de mardi sur les 3 erreurs au squat » |
| `commercial-tiktok` | Scripts de vidéos courtes plan par plan, légendes, hashtags, réponses aux commentaires | « Écris 3 scripts TikTok pour cette semaine » |
| `graphiste` | Designer : logo et ses déclinaisons, modèles de visuels, visuel de chaque post et design du merch (dans Canva si disponible) | « Crée le visuel du carrousel de mardi » |

**Enchaînement des étapes :** calendrier (`responsable-marque`) → textes et
scripts (`commercial-instagram` / `commercial-tiktok`) → visuels
(`graphiste`) → contrôle sécurité si le post donne un conseil d'exercice ou
de nutrition (`coach-securite`) → `controleur-qualite` → **validation de
simo** → publication par simo. C'est la conversation principale qui lance
chaque étape. Aucun agent ne publie lui-même.

## Pôle accueil

Traite chaque mail qui arrive et prépare chaque nouveau client avant son
premier rendez-vous. Fonctionnement, règles et modèles :
`equipe/pole-accueil/`.

| Agent | Rôle | Exemple de demande |
|---|---|---|
| `secretaire-mails` | Lit les nouveaux mails une fois par jour, les trie et les étiquette, répond aux demandes de coaching avec les modèles validés (sinon brouillon), fait le résumé du jour | « Qu'est-ce que j'ai reçu aujourd'hui ? » ou « Réponds au mail de Julie » |
| `agent-accueil` | Pour chaque nouveau client : code client, dossier dans le Drive privé, anamnèse, commande potentielle (bon de commande), puis relais à `coach-bilan` | « Nouvelle cliente Julie, elle veut PUR GOLD, prépare son dossier » |

**Enchaînement des étapes :** mail reçu (`secretaire-mails`, réponse avec
le questionnaire d'anamnèse) → dossier ouvert (`agent-accueil`) →
anamnèse reçue → état du bilan (`coach-bilan`) → bon de commande
(`agent-accueil`) → Simon fixe le rendez-vous et encaisse → paiement noté
(`comptable`) → programme (pôle sport). Une routine vérifie la boîte mail
une fois par jour. Les réponses partent seules seulement quand simo a
validé les modèles ; avant, ce sont des brouillons dans Gmail.

## Pôle commercial

Transforme la visibilité en clients, fait évoluer les offres et le merch,
écrit avec la voix de Simon et garde l'argent en ordre. Fonctionnement et
fichiers communs : `equipe/pole-commercial/`.

| Agent | Rôle | Exemple de demande |
|---|---|---|
| `developpeur-commercial` | Offres et packs, parrainage, partenariats locaux, scripts de vente, suivi des prospects | « Propose-moi une offre de parrainage » |
| `responsable-merch` | Produits dérivés en impression à la demande (sans stock), prix, marge, lancements | « Imagine une première collection de t-shirts PUR COACHING » |
| `ghostwriter` | Textes à la première personne avec la voix de Simon | « Écris mon histoire pour le site, comme si c'était moi » |
| `comptable` | Registre des recettes et dépenses, factures, point du mois, questions d'administration (tout dans le Drive privé) | « Note le paiement PUR GOLD de C01 reçu aujourd'hui » |

**Étapes :** proposition de l'agent → `coach-securite` si le contenu donne
un conseil d'exercice ou de nutrition → `controleur-qualite` → décision de
simo.

**Amélioration continue :** chaque lundi matin, une routine automatique
réveille la conversation principale, qui demande au `directeur-croissance`
de faire le point de la semaine et choisit 3 améliorations au maximum ; la
conversation principale confie ensuite chaque amélioration à l'agent
indiqué. Les agents proposent, simo décide. Les chiffres et les noms de
clients restent dans le Google Drive privé de simo, jamais dans le dépôt.
