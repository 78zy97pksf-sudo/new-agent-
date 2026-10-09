# Le pôle sport

Le pôle sport crée des **programmes sportifs complets et sûrs** pour les
clients de simo (coach sportif), et des **programmes types à revendre**.

## ATTENTION : le dépôt GitHub est PUBLIC

Tant que le dépôt est public, **ne jamais y mettre de vraies données de
clients** (nom complet, informations de santé). Utiliser un code client
(ex. `client-012`), ou garder les vraies fiches hors du dépôt.
Voir `clients/README.md`.

## Qui fait quoi

| Agent | Son métier |
|---|---|
| `coach-bilan` | Fait le bilan du client et donne un état : bilan incomplet, feu vert, orange ou rouge |
| `coach-programmeur` | Construit le programme complet (client ou programme type à revendre) |
| `coach-nutrition` | Coach nutrition et hygiène de vie : conseils généraux, non médicaux |
| `coach-securite` | Vérifie la sécurité du programme avant qu'il parte au client ou soit vendu |
| `controleur-qualite` | (équipe générale) Relit la forme : clarté, fautes, présentation |

## Les fichiers communs (à lire par tous les agents du pôle)

- `mon-coaching.md` : la façon de travailler de simo (marque, ton, clients,
  matériel). C'est ici que simo écrit ses corrections.
- `regles-securite.md` : les règles de sécurité communes. Elles passent
  avant tout le reste.
- `coaching-distance.md` : tout le fonctionnement des formules 100 % à
  distance PUR ONLINE et PUR ONLINE+ (parcours, bilan, suivi, sécurité).
  À lire pour chaque client suivi à distance.
- `modele-fiche-client.md` et `modele-programme.md` : les modèles à remplir.
- `clients/<prenom-ou-code>/` : un dossier par client.
- `programmes-a-vendre/` : les programmes types destinés à la vente.

## Les étapes pour un client, dans l'ordre

1. **Bilan** — `coach-bilan`
   Pose les questions, remplit la fiche client, donne l'état.
   - **Bilan incomplet** → on pose les questions manquantes au client, puis
     on refait le bilan. Pas de programme.
   - Feu **rouge** → on s'arrête là. Le client doit d'abord obtenir un avis
     médical écrit.
   - Feu **orange** → avis médical recommandé ; programme très léger, sans
     progression, seulement si le client le souhaite (voir
     `regles-securite.md`).
   - Feu **vert** → on continue.
2. **Programme** — `coach-programmeur`
   Construit le programme avec le modèle.
3. **Nutrition** (seulement si demandé) — `coach-nutrition`
   Ajoute des conseils généraux d'hygiène de vie.
4. **Contrôle sécurité** — `coach-securite`
   Verdict « validé » ou « à corriger ». Si « à corriger », on renvoie à
   l'agent indiqué, puis on recontrôle.
5. **Contrôle de la forme** — `controleur-qualite`
   Vérifie que c'est clair, sans fautes, agréable à lire.
6. **Livraison** — simo relit et envoie le programme au client.

## Les étapes pour un programme à revendre

1. **Programme type** — `coach-programmeur`
   Écrit le programme avec l'en-tête « Programme type » (public visé, niveau,
   à qui il ne convient pas, questionnaire santé à faire soi-même) et
   l'enregistre dans `programmes-a-vendre/`.
2. **Nutrition** (si on veut l'inclure) — `coach-nutrition`.
3. **Contrôle sécurité** — `coach-securite`, grille « programme type ».
4. **Contrôle de la forme** — `controleur-qualite`.
5. **Mise en vente** — simo relit, puis met le programme sur sa page de
   vente.

## Important : qui lance les étapes ?

Un agent **ne peut pas lancer un autre agent**. C'est la **conversation
principale** (celle où simo écrit) qui enchaîne les étapes : elle confie le
bilan à `coach-bilan`, puis passe la fiche à `coach-programmeur`, et ainsi
de suite.

Exemples de demandes de simo :
- « Nouveau client : client-012, 35 ans, débutante, veut perdre du poids,
  3 séances par semaine à la maison. Lance le pôle sport. »
- « Crée un programme type à vendre : remise en forme débutant à la maison,
  8 semaines. »

## Améliorer le pôle

Quand simo n'est pas satisfait d'un résultat, il note sa remarque dans la
section « Corrections et préférences de simo » de `mon-coaching.md`. Tous
les agents la liront la prochaine fois.
