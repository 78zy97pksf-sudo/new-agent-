# Direction artistique des couvertures illustrées

Depuis le lot du 19 octobre 2026. Le `graphiste` suit ce fichier ; `responsable-marque` en est le
gardien et simo valide les changements.

But : arrêter le pouce qui fait défiler. Chaque couverture a UNE illustration originale, forte, lisible en
miniature sur un téléphone, et reconnaissable comme « PUR COACHING » d'un post à l'autre.

D'où vient l'image : d'abord l'IA d'images de Canva (`generate-image`, crédit gratuit qui revient le 1er de
chaque mois). Quand le crédit est épuisé (épuisé le 9 octobre 2026, il revient le 1er novembre), le graphiste dessine
lui-même l'illustration en code SVG. Les mêmes règles valent dans les deux cas. Les autres générateurs
d'images en ligne ne sont pas accessibles depuis le projet.

## Style
- « Affiche sportive moderne » : illustration vectorielle plate mais avec de la profondeur (plans
  superposés, dégradés, halos doux, ombres portées simples), lignes de mouvement en diagonale.
- Un seul sujet central, grand, simple, qui se comprend en 1 seconde (un objet ou une scène).
- Grain léger possible (filtre feTurbulence discret), jamais de flou qui salit.
- Contraste fort : le sujet doit ressortir sur le fond.

## Couleurs
- Base de la marque : bleu foncé #12304F, bleu #2B5A96, bleu ciel #DCEFF8, très clair #F4FAFD, blanc.
- Accents permis selon le thème :
  - automne et course de jour : orangé chaud #F2B56B et #E07A3F, en touches ;
  - nuit et heure d'hiver : bleus très foncés, lumière de lampe jaune pâle #FFE9A8, bandes réfléchissantes
    gris clair brillant ou jaune fluo doux #E9F27A ;
  - l'or (#C9A24A, #E8C770) est RÉSERVÉ à PUR GOLD : seulement IG9 (si PUR GOLD y figure) et IG13 / TT13.
- Le bas de l'image doit tirer vers le bleu foncé #12304F (un voile bleu foncé y est ajouté pour le texte).

## Ce qui est interdit
- Visage réaliste, personne reconnaissable, imitation de Simon, faux client. Si une silhouette de coureur
  apparaît : stylisée, de dos ou de profil, sans visage détaillé, corps neutre (pas de « corps parfait »).
- Faux monument de Huy (Collégiale, fort, etc.) : un paysage générique (rivière, chemin, arbres) est permis.
- Chiffre de poids ou de pourcentage sur une balance, « avant / après », mètre ruban autour d'un corps.
- Symboles médicaux (croix, électrocardiogramme, seringue, pilule).
- Logo de marque (Nike, Strava, etc.), texte copié, photo trouvée sur Internet.
- Texte dans l'illustration, sauf un grand mot ou chiffre décoratif (ex. « VMA », « 18:00 ») qui ne répète
  pas le titre et qui reste discret (opacité faible ou contour) ; police Montserrat uniquement.

## Mise en page (très important)
- Instagram : fichier `<ID>.svg`, viewBox exactement "0 0 1080 1350". Le sujet tient dans la moitié
  haute (y de 120 à 720). De y = 760 à 1350, le texte sera posé sur un voile bleu foncé : garder ce bas
  calme et sombre.
- TikTok : fichier `<ID>.svg`, viewBox exactement "0 0 1080 1920". Le sujet tient entre y = 180 et
  y = 940. En dessous, garder calme et sombre (texte + boutons de TikTok). Rien d'important à droite
  au-delà de x = 930 entre y = 700 et 1750 (boutons de l'appli).
- Le petit logo rond se pose en haut à gauche (x 64 à 160, y 56 à 152) : rien d'important derrière.
- Pour une paire Instagram + TikTok (même sujet), garder le même dessin, recadré et réorganisé pour
  chaque format.

## Règles techniques
- Un fichier SVG autonome par couverture, avec xmlns="http://www.w3.org/2000/svg" et le viewBox ci-dessus.
- Aucun lien externe (pas d'<image href="http...">, pas de police externe, pas de script).
- Tous les id (dégradés, filtres, masques) commencent par l'identifiant du post en minuscules
  (ex. "ig7-ciel"), pour ne pas se mélanger avec les autres.
- Moins de 200 Ko par fichier.

## Vérifier son travail
Les outils sont dans le dossier partagé `pur-coaching/marketing/outils-visuels/` (voir son LISEZMOI) :
`python3 apercu.py <fichier.svg> ig|tt "<accroche>" "<kicker>"` crée la couverture avec son texte et
l'illustration seule dans `apercu/`. Regarder les deux images et corriger jusqu'à ce que : le sujet soit
beau et clair, rien d'important ne soit caché par le texte ou le logo, le titre se lise très bien, et
l'ensemble donne envie de s'arrêter.
