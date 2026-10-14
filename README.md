# Renseignement d'urbanisme à la parcelle, Les Ponts-de-Cé

Une application web pour les agents d'une collectivité, qui renseignent le public et instruisent le droit des sols. On tape une adresse, ou on clique une parcelle, et on obtient une fiche complète, prête à lire et à imprimer.

C'est un outil d'aide à la décision et d'accompagnement. Il réunit sur une seule carte ce qu'un agent va d'habitude chercher dans plusieurs outils.

## Ce que fait l'application

La recherche. On tape une adresse, la carte s'y rend, via la Base Adresse Nationale.

La fiche de la parcelle. Au clic ou à la recherche, elle affiche
- la référence cadastrale et la surface de la parcelle, via l'API Carto de l'IGN,
- la zone du PLU, sa règle générale, et si la parcelle est constructible ou protégée,
- les risques connus à cet endroit, via Géorisques, avec le lien vers le rapport officiel,
- un accès direct aux prix des ventes autour, via DVF.

La lecture du territoire. Une légende filtre les familles de zones, urbaine, à urbaniser, agricole, naturelle. Un panneau donne la répartition des surfaces et la part déjà urbaine ou à urbaniser.

Les outils. Une bascule entre le plan et la photo aérienne. Un outil de mesure de distance et de surface. Et l'impression de la fiche.

## Les données

Le zonage du PLUi d'Angers Loire Métropole est intégré au fichier. Il vient du Géoportail de l'urbanisme, récupéré par l'API Carto de l'IGN, puis allégé pour le web. Toute la métropole s'affiche ainsi d'un seul coup.

Le reste est appelé en direct quand on utilise l'application. Les parcelles viennent de l'API Carto. Les adresses viennent de la Base Adresse Nationale. Les risques viennent de Géorisques. Les prix renvoient vers DVF. Les fonds sont CARTO Positron et la photo aérienne de l'IGN.

## Comment l'ouvrir

Ouvrez index.html dans un navigateur, avec une connexion internet. Pour une version en ligne, publiez le fichier sur un hébergement statique, par exemple GitHub Pages ou Netlify.

## Le dépôt

- `index.html`, l'application complète. Un seul fichier.

## Auteur

Victorine Maximilienne Djetcheu Toko, géomaticienne et ingénieure topographe.
Portfolio, https://portfolio-victorine-djetcheu.netlify.app
