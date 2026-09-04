# Site vitrine ML Clean Services

Site statique Jekyll, hébergé sur GitHub Pages (build natif, aucune GitHub Action à maintenir).

**ML Clean Services**, Débarrassage • Nettoyage • Accompagnement
Débarras, nettoyage/désinfection et accompagnement social en Périgord Noir
(Sarlat et alentours, rayon d'environ 1 h). Entreprise de l'ESS.

## Organisation du contenu

| Dossier | Contenu |
|---|---|
| `_prestations/` | Les 3 pôles de service (pages piliers) |
| `_situations/` | Une page par situation traitée (Diogène, insalubrité, après décès…). **Ajouter un fichier `.md` ici suffit** : la page apparaît automatiquement dans le méga-menu, le footer, et les blocs de maillage interne. Rattacher au pôle via `pole:` dans le front-matter. |
| `_zones/` | Phase 2, une page par zone d'intervention. Le menu s'active automatiquement dès le premier fichier. |
| `pages/` | Pages fixes (Qui sommes-nous, Espace pros, Contact, Mentions légales) |
| `_data/` | Coordonnées (`contact.yml`), navigation (`navigation.yml`), engagements/valeurs (`social_proof.yml`) |

## Mise en ligne (GitHub Pages)

1. Créer un dépôt GitHub et pousser ces fichiers.
2. Settings → Pages → Source : `Deploy from a branch` → branche `main`, dossier `/ (root)`.
3. Renseigner `url:` et `baseurl:` dans `_config.yml` selon le nom du dépôt.

## À compléter avant mise en ligne publique

Rechercher `À REMPLACER` et `À COMPLÉTER` dans le projet :

- [x] Téléphone et email (`_data/contact.yml`)
- [x] Formulaire de devis : FormSubmit (`_data/contact.yml`), aucun compte à créer — activer en
      cliquant le lien reçu par email à la première vraie soumission
- [ ] SIRET, siège social, capital, RCS (`pages/mentions-legales.md`)
- [x] `url:`/`baseurl:` (`_config.yml`)
- [x] Logo + favicon (`assets/img/`)
- [x] Politique de confidentialité RGPD (`pages/confidentialite.md`, publiée)

## Prévisualisation locale (optionnel)

Nécessite Ruby : `bundle install` puis `bundle exec jekyll serve`.
Sinon : pousser sur GitHub et vérifier le site en ligne.
