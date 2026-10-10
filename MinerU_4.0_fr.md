# MinerU 4.0

MinerU 4.0 réunit l'analyse de documents, une bibliothèque de documents locale et des outils de service dans un seul flux de travail, pour la conversion de documents, l'intégration d'applications et la lecture par agent.

## Quatre niveaux d'analyse

- **Flash** — pour les aperçus rapides et l'indexation
- **Basic** — pour l'OCR et l'analyse basée sur des modèles
- **Standard / Advanced** — pour les mises en page plus exigeantes et des exigences de qualité supérieures

## Formats d'entrée multiples

PDF, images, DOC/DOCX, PPT/PPTX, XLS/XLSX, RTF, ODT/ODS/ODP, EPUB, OFD, HTML/MHTML et CSV/TSV. DocVortex assure l'analyse native des documents.

## Bibliothèque de documents et lecture par agent

- Découvrir les fichiers
- Mettre les résultats en cache
- Rechercher le contenu
- Reprendre la lecture par page ou par bloc
- Conserver des localisateurs de citation stables

## Configuration indépendante des modèles

- **Petits modèles :** ONNX ou Torch
- **VLM :** llama.cpp, vLLM ou LMDeploy

## Outils unifiés

- SDK Python
- API V1
- Conversion par lots sans état
- Routeur multi-services
- WebUI basée sur Gradio

## Résultats structurés et rendu

Un modèle de document unique prend en charge **neuf cibles de rendu** :

1. Markdown
2. HTML
3. LaTeX
4. DOCX
5. EPUB
6. PDF
7. Contenu structuré (Structured Content)
8. Liste de contenus V1 (Content List V1)
9. Liste de contenus V2 (Content List V2)

Chaque CLI/API expose son propre sous-ensemble d'exportations ; voir Formats de sortie et Contrat de résultat.

## Prise en charge des formats et notes d'analyse

| Format | Niveau / méthode d'analyse |
| --- | --- |
| PDF et images | Les quatre niveaux (Flash / Basic / Standard / Advanced) |
| Office (DOC/DOCX, PPT/PPTX, XLS/XLSX), RTF, ODT/ODS/ODP | Analyse native Flash locale |
| EPUB, OFD | Analyse native Flash locale |
| HTML/MHTML | Analyse native Flash locale |
| CSV/TSV | Analyse native Flash locale |
| Texte brut | Lecture directe (sans analyse) |

> Les documents ne sont pas téléversés automatiquement vers le service officiel ; l'analyse à distance nécessite une configuration explicite.
