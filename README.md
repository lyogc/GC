# GC – Générateur de certificats de travail

Maquette du Service des Ressources Humaines de la Ville de Carouge, pour la prise en main et les retours utilisateurs.

## Fonctionnement

1. Le ou la chef·fe de service remplit le questionnaire `FORM_Certificat_Travail.pdf` (PDF interactif, sans donnée personnelle).
2. Dans l'application (`index.html`), on dépose le questionnaire rempli et la bibliothèque `MOD_Bibliotheque_Certificat_Travail.xlsx`.
3. L'application assemble le texte à partir de la bibliothèque, puis le télécharge dans le modèle Word de la Ville.
4. Le sexe et les dates de mission viennent du questionnaire ; les autres informations personnelles (nom, date de naissance, taux) sont surlignées en gris et se complètent dans le Word.

Tout se passe dans le navigateur : rien n'est enregistré ni envoyé.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | L'application, en un seul fichier |
| `FORM_Certificat_Travail.pdf` | Le questionnaire à remplir |
| `MOD_Bibliotheque_Certificat_Travail.xlsx` | La bibliothèque : formulations, services de la Ville, métiers par service (épicène) et cahiers des charges (à compléter) |

Les codes des champs du questionnaire (par exemple `SF_QUALITE`) sont ceux de la colonne « Code » de la bibliothèque : c'est ce qui fait le lien entre les deux.
