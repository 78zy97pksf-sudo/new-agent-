# La micro-entreprise d'agents de simo

Ce dépôt est une **micro-entreprise d'agents IA**. Chaque agent est un « employé »
spécialisé, décrit par un fichier dans `.claude/agents/`. Le but : augmenter la
productivité de simo et réaliser des tâches complexes en les découpant entre
plusieurs spécialistes.

## Règles générales

- Toujours répondre à simo **en français**, avec des mots simples, sans jargon.
- simo débute avec GitHub et n'est pas développeur : expliquer chaque étape
  technique une par une.
- Avant de commencer une tâche, regarder dans `equipe/ORGANIGRAMME.md` quel
  agent est le mieux placé pour la faire, et lui confier le travail.
- Si aucun agent ne convient, demander à l'agent **directeur** d'en créer un
  nouveau (voir ci-dessous).

## Comment fonctionne l'entreprise

1. **simo exprime un besoin** (par exemple « j'ai besoin de quelqu'un qui
   prépare mes posts LinkedIn »).
2. **Le directeur** (`.claude/agents/directeur.md`) analyse le besoin, vérifie
   si un agent existant peut déjà le faire, sinon conçoit un nouvel agent en
   suivant la méthode `.claude/skills/creer-agent/SKILL.md`.
3. Le nouvel agent est ajouté dans `.claude/agents/` et inscrit dans
   `equipe/ORGANIGRAMME.md`.
4. Pour les grosses missions, le **chef de projet** découpe le travail en
   étapes et indique quel agent fait quoi ; la conversation principale
   confie ensuite chaque étape à l'agent indiqué.
5. Le **contrôleur qualité** relit le résultat avant de le présenter à simo.
   Pour un contenu public (post, vidéo, texte du site), le **jury de
   contenu** le note d'abord à la place des clients visés
   (`equipe/pole-marketing/grille-qualite-contenu.md`).

## Bon à savoir

- Un agent ne peut pas lancer lui-même un autre agent : c'est la conversation
  principale qui distribue le travail entre eux, selon le plan.
- Un agent nouvellement créé est disponible dès la prochaine conversation
  (ou après avoir rechargé les agents).
- Les fichiers d'agents sont écrits en français pour que simo puisse les lire
  et les modifier librement.
- Le but de chaque contenu est d'amener des clients : on écrit pour une
  personne précise de `equipe/pole-marketing/client-cible.md`, avec un seul
  appel à l'action (`equipe/pole-marketing/parcours-client.md`).
