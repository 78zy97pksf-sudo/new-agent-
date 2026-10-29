---
name: creer-agent
description: Méthode et modèle pour créer un nouvel agent (un nouvel « employé ») dans la micro-entreprise. À utiliser dès qu'il faut concevoir ou réécrire une fiche d'agent dans .claude/agents/.
---

# Créer un nouvel agent

## 1. Les questions à se poser

- **Quel métier ?** Un seul métier par agent (ex. « rédacteur de posts
  LinkedIn », pas « marketing en général »).
- **Quel résultat concret ?** Ce que l'agent doit rendre à la fin.
- **Quand l'utiliser ?** Les situations où la conversation principale doit
  lui confier le travail. C'est ce qui va dans la `description`.
- **Quels fichiers lire avant de travailler ?** Les fichiers communs qui
  contiennent les faits (offres et prix dans `mon-coaching.md`, règles,
  leçons, client cible…), pour ne jamais les recopier dans la fiche.
- **Quels outils ?** Ce qu'il faut pour faire le travail, pas plus, parmi :
  - `Read, Glob, Grep` : lire et chercher dans les fichiers ;
  - `Write, Edit` : créer et modifier des fichiers ;
  - `Bash` : lancer des commandes (seulement pour les agents techniques) ;
  - `WebSearch, WebFetch` : chercher et lire sur Internet (chaque lecture
    de page avec `WebFetch` demande l'accord de simo : à garder rare) ;
  - les connexions du projet, outil par outil (par exemple
    `mcp__Metricool_Social_Media_Management__getAnalyticsDataByMetrics`
    pour lire des statistiques, `mcp__Canva__generate-design` pour un
    visuel, les outils `mcp__Gmail__…` ou `mcp__Google_Drive__…`). Pour
    un agent qui ne doit que lire, ne donne que les outils de lecture.
- **Comment sait-on que c'est bien fait ?** 3 à 6 critères vérifiables
  (un seuil, une liste, une grille) que l'agent applique avant de rendre.
- **Quelles limites ?** Ce que l'agent ne doit pas faire.

## 2. Le modèle de fiche

Copier ce modèle dans `.claude/agents/<nom>.md` et le remplir :

```markdown
---
name: <nom-en-minuscules-avec-tirets>
description: <Métier en une phrase>. À utiliser quand <situations précises>.
tools: <liste des outils, séparés par des virgules>
---

Tu es <rôle> dans la micro-entreprise d'agents de simo.
Tu réponds toujours en français, avec des mots simples.

## Ta mission
<Ce que tu dois accomplir, pour qui, et le résultat pour l'entreprise.>

## Avant de commencer
Lis toujours :
- <fichier commun 1> ;
- <fichier commun 2>.

## Ta méthode
1. <Étape 1>
2. <Étape 2>
3. <Étape 3>

## Critères de qualité
Avant de rendre, vérifie :
- <critère vérifiable 1> ;
- <critère vérifiable 2>.

## Ce que tu rends
<Format exact du résultat : liste, tableau, texte, fichier…>

## Tes limites
- <Ce que tu ne fais pas, et à qui renvoyer dans ce cas.>
```

## 3. Après la création

1. Ajouter l'agent dans `equipe/ORGANIGRAMME.md` (nom, rôle, exemple de
   demande).
2. Vérifier qu'il ne fait pas doublon avec un agent existant.
3. Donner à simo une phrase d'exemple pour l'utiliser.
