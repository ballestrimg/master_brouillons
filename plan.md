# Mémoire : plan structuré  
  
## Remerciements  
Cmm  
USP  
SEENC  
Enseignants.es  
*ex-machinae*  
  
## Résumé  
Dans le cadre de mon stage au sein du DaSCH, j'ai développé trois applications visant à permettre à des versions allégées d'images 2D et 3D d'intégrer leurs métadonnées structurelles et descriptives au cadre international d'interopérabilité des images (International Image Interoperability Framework - IIIF). La question de recherche est la suivante : est-il réellement possible de garantir la persistance des données archivistiques en utilisant IIIF ?   
  
Le principal défi aujourd'hui réside dans la gestion de données hétérogènes provenant d'objets intrinsèquement variés, ainsi que de différentes organisations ayant des objectifs distincts. L'enjeu est d'éviter l'effet "setting and forgetting" en cherchant à rendre la description et l'exploitation des données pérennes entre diverses organisations. De plus, l'utilisation de ces données soulève des problèmes et des impacts environnementaux. Par conséquent, l'optimisation de la préservation numérique et de l'interopérabilité apparaît comme une priorité à développer, car elle permettrait une utilisation efficace des données dans un contexte patrimonial.  
  
  
## Introduction  
(phrase) accrochée : K. Pomian AJOUTER BIBLIO  
A. bullet points : présenter de quoi il s'agit et les principales questions à être dévéloppées  
B. Introduire questions théoriques sur les données

## Chapitre I  
  
### A. Contexte DaSCH  
#### a1. DaSCH actuellement  
**sous-argument 1 :** acteurs actuels et mission  
*exemple.:* About us DaSCH  
**sous-argument 2 :** financement du DaSCH  
*exemple.:* cf. road map SNF  
**Sources :** https://www.dasch.swiss/about-us  
**Sources :** https://www.snf.ch/en/fvnejfErYvg7ShsD/funding/infrastructures/roadmap  
  
#### a2. Qu'est-ce que DaSCH ?  
**sous-argument 1 :** histoire de la création et but  
*exemple.:* About us DaSCH  
**sous-argument 2 :** les acteurs historiques du DaSCH  
*exemple.:* About us DaSCH  
**Sources :** https://www.dasch.swiss/about-us  
  
#### a3. DaSCH et le nouveau scénario de la conservation patrimoniale  
**sous-argument 1 :** dasch-app : expliquer le site  
**sous-argument 2 :** DaSCH et les start-up ou DaSCH et IIIF    
**Sources :** https://www.dasch.swiss/dsp-app  
**Sources :** Docs Google sur DaSCH (fichier partagé)  
  
#### a3.1. Mission de conservation de données du DaSCH : menacé ?  
**sous-argument 1 :** Conservation des données et ses pérénité  
**sous-argument 2 :** problemes face au financement SNSF ?  
**Sources :** https://www.snf.ch/en/FKhU9kAtfXx7w9AI/page/home  
**Sources :** https://www.snf.ch/en/fvnejfErYvg7ShsD/funding/infrastructures/roadmap  
**Sources :** Road Map https://www.sbfi.admin.ch/sbfi/en/home/services/publications/data-base-publications/roadmap_research_infrastructures_2023.html#:~:text=The%202023%20Swiss%20Roadmap%20for,and%20European%20research%20infrastructure%20networks  

### B. Contexte IIIF  
#### b1. Qu'est-ce que l'IIIF ? Définition  
**sous-argument 1 :** expliquer création et but  
**sous-argument 2 :** enjeux majeurs de IIIF  
  
#### b2. Usages : répandu milieu patrimoniale  
**sous-argument 1 :** grandes institutions qui l'utilisent  
*exemple.:* Bnf, Cambridge University, Vaticani  
**sous-argument 2 :** viewers en lignes  
*exemple.:*  universal, Mirador etc.
  
**à mentionner :**  
"Viewer" est une dénomination générique pour les outils qui nous permettent de rendre des modèles 3D visibles sur web (cf. Rossenova, 2023) 
  
#### b3. IIIF versions : API 3.0.  
**sous-argument 1 :** expliquer création et but  
**sous-argument 2 :** enjeux majeurs de IIIF  
  
**Sources :** https://iiif.io/api/presentation/3.0/ (Presentation API)  
**Sources :** https://iiif.io/api/image/3.0/ (Image API)  
**Sources :** https://iiif.io/get-started/iiif-viewers/  
  
#### b4. IIIF versions : vers l'API 4.0.  
**sous-argument 1 :** expliquer création et but  
**sous-argument 2 :** enjeux majeurs de IIIF  
**Sources :** https://github.com/IIIF/3d (GitHub Julie Winchester)  
#### à mentionner :  
manifest JSON  
  
### C. Durabilité des données : document, archive et conservation patrimoniale  
#### c1. Qu'est-ce qu'un document ?  
accroché : phrase de Marc Bloch (cf. notes cours historiographie BR)  
**sous-argument 1 :** définition préliminaire de document  
*exemple.:*  
**sous-argument 2 :** déf. document contexte plus large  
*exemple.:* article Ulpiano AJOUTER BIBLIO  
  
#### c2. Qu'est-ce qu'un archive ?  
**sous-argument 1 :** définition  
**sous-argument 2 :** possibilité de critiquer le concept d'archive  
  
**Sources :** livret sur les archives ENC, reprendre la discussion conceptuale  
  
#### c3. Que'est-ce que une donnée ?  
**sous-argument 1 :** définition des sciences dures  
*exemple.:*  
**sous-argument 2 :** redéfinition dans le contexte de Digital Humanities  
*exemple.:*  
  
**Sources :**  
txts de Julien Raemy  
txts de Gregor Bachman  
txts Ulpiano Bezerra   
  
à mentionner :  
API 3.O vs API 4.0  
  
### D. Défis du stage  
#### d1. But du stage : créer deux pipelines automatisées - expliquer missions (cf. fiche de stage)  
**sous-argument 1 :** premier pipeline  
*exemple.:* python code simplification des images  
**sous-argument 2 :** deuxième pipeline  
*exemple.:* python code pour insertion de métadonnées  
  
#### d2. Pourquoi ces pipelines ?  
  
#### d2.1. Réalité chez DaSCH . Utilisation de Desktop Softwares  
**sous-argument 1 :** montrer les apps et ses usages  
*exemple.:* apps utilisées + fonction basique et utilisation chez DaSCH  
**sous-argument 2 :** possibilité d'automatisation avec Python plus optimisée déjà envisagée pour remplacer MeshLab, GIMP et Blender  
*exemple.:* citer article Rossenova, L., cf. Biblio  
  
#### d2.2. Utilisation chez DaSCH des outils de transformation d'image qui vont être intégrés au API 4.0.  
**sous-argument 1 :** DaSCH utilise ces deux processus  
*exemple.:*  
**sous-argument 2 :** Suivre les prérequis minimales du nouveau API 4.0.  
*exemple.:*  
**Sources :** présentation Rita Gautschy, dans Downloads Folder, ou  
GitHub Julie Winchester : https://github.com/IIIF/3d  
Rossenova, L. (2023) ‘IIIF for 3D – making web interoperability multi-dimensional’ ...  
  
#### d3. Néanmoins, impossibilite d'automatiser efficacement des Desktop software  
**sous-argument 1 :** apps peuvent ne pas etre executables si version ou OS changent  
**sous-argument 2 :** bibliothéques qui fonctionnent ou qui sont plus suivies  
  
#### d4. Python  
**sous-argument 1 :** langage accessible  
*exemple.:* syntaxe easy-friendly et open source  
**sous-argument 2 :** plus de ressources avec Python  
*exemple.:* documentation facile à trouver, facile à réutiliser et encore possibilité de intégrer à diff. multimédias (Flask, Docker)  
  
#### d5. Usage Docker  
**sous-argument 1 :** permettre execution de l'app dans différents OS  
exemple.: syntaxe easy-friendly  
**sous-argument 2 :** plusieurs d'applications de DaSCH sont sur Docker  
exemple.: DaSCH container sur Docker et par consequent connnaissance de l'outil (use interne)  
**Sources :** docker doc https://docs.docker.com/build-cloud/   
DaSCH docker https://hub.docker.com/u/daschswiss and  
Docker Cheat Sheet by DaSCH https://docs.dasch.swiss/2023.11.01/DSP-API/05-internals/development/docker-cheat-sheet/  
  
#### d6. Bootstrap 4.0. : outil pour créer des websites modernes  
**sous-argument 1 :** ressources pour créer des sites responsives  
exemple.: citer les classes en Bootstrap et les features responsives  
**sous-argument 2 :** ressources pour intégrer CSS et JS facilement  
*exemple.:* citer la ligne de code avec JSS/CSS qu'on peut intégrer facilement dans nos dossiers  
**Sources :** https://getbootstrap.com/docs/4.0/getting-started/introduction/ (Version 4)  
  
#### d7. Bootstrap 4.0.: version 4 a plus de documentation et rassure le deploiement de l'application sans beaucoup de contraintes  
**sous-argument 1 :** version plus stable, plus d'informnations sur site  
*exemple.:* comparer avec la versions 5.0.  
**sous-argument 2 :**  
*exemple.:*  
**Sources :** https://getbootstrap.com/docs/4.0/getting-started/introduction/ (Version 4)  
  
## Chapitre II : Cas d'usages : Applications : des images au IIIF  
  
### A. Applications pour gérer la taille des images (file size)  
#### a1. DaSCH Converter  
**sous-argument 1 :** simplifier images 2D  
*exemple.:* réduction de pixels 1024x1024 pour pouvoir être lue par les nouveaux viewer  
**sous-argument 2 :** pourquois ?  
*exemple.:* api 4.0. et questions environnementales  
  
#### a2. DaSCH Mesh    
**sous-argument 1 :** simplifier images 3D  
*exemple.:* M. Garland and P. Heckbert., Surface Simplification Using Quadric Error Metrics (pdf) AJOUTER BIBLIO  
**sous-argument 2 :** pourquois ?  
*exemple.:* minimum vertices pour l'api 4.0. et questions environnementales  
**Source**: http://mgarland.org/files/papers/quadrics.pdf 1997  
  
### B. Application pour insérer les métadonnées dans les fichiers  
#### b3. DaSCH IIIF  
**sous-argument 1 :** associer des métadonnées aux images à partir d'un fichier JSON dont le but est les intégrer aux standards du IIIF  
*exemple.:*  
**sous-argument 2 :** pourquois ?  
*exemple.:* raisons IIIF + raisons liées à la conservation  
  
**à mentionner:**   
base de données DaSCH (dasch-api)  
daschify IIIF (presentation app), app Julien  
  
## Chapitre III : resultats  
### A. Applications "dockerisés" sur DaSCH Docker Hub  
**sous-argument 1 :** facile à télécharger  
*exemple.:*  
**sous-argument 2 :** open source app  
*exemple.:*  
**Source:** https://hub.docker.com/u/daschswiss  
  
### B. Performance des applications :  
#### b1. DaSCH Converter  
**sous-argument 1 :** taille des fichiers réduite (réduction de pixels)  
*exemple.:* graphes de performance  
**sous-argument 2 :** analyse des graphes  
*exemple.:*  
  
#### b2. DaSCH Mesh  
**sous-argument 1 :** taille des fichiers réduite (contraction de vértices)  
*exemple.:* graphes de performance  
**sous-argument 2 :** analyse des graphes  
*exemple.:*  
  
#### b3. DaSCH IIIF  
**sous-argument 1 :** insertion JSON  
*exemple.:* insertion minimum features  
**sous-argument 2 :**  
*exemple.:* annexe file size ou print github tests???  
  
### C. Courbe d'apprenstissage courte des applications  
#### c1. Applications faciles à utiliser, avec interface responsive  
**sous-argument 1 :** structure "drag and drop" pour convertir les fichiers  
*exemple.:* prints du box drag and drop des applications  
**sous-argument 2 :** download automatique : un click, une conversion  
*exemple.:* print des boutons  
  
### D. Améliorations dans les applications  
  
#### d1. Features plus imimentes  
**sous-argument 1 :** créer input pour fichiers multiples  
*exemple.:* possibilité de faciliter l'utilisation des longues dossiers, problèmes possibles avec les exports  
**sous-argument 2 :** plus d'options de download  
*exemple.:* fichier zip qui est téléchargé automatiquement ou si plus d'un archive download zip automatique  
  
#### d2. D'autres features possibles  
**sous-argument 1 :** créer input pour fichiers multiples  
*exemple.:* la même box, mais avec une interaction JavaScript pour multiples fichiers (page intermédiaire?)  
**sous-argument 2 :** écran de loading si fichier trop long (> 50 mb ou > 0,5 seconde d'attente)  
*exemple.:* fichier zip qui est téléchargé automatiquement ou si plus d'un archive download zip automatique  
  
### Bibliographie  
**Abergel, V. et al. (2023)** ‘Aïoli: A reality-based 3D annotation cloud platform for the
collaborative documentation of cultural heritage artefacts’, Digital Applications in Archaeology
and Cultural Heritage, 30, p. e00285. Available at: https://doi.org/10.1016/j.daach.2023.e00285.  
**Cornut, M., Raemy, J.A. and Spiess, F.** (2023) ‘Annotations as Knowledge Practices in Image
Archives: Application of Linked Open Usable Data and Machine Learning’, Journal on
Computing and Cultural Heritage, 16(4), pp. 1–19. Available at:
https://doi.org/10.1145/3625301.  
**Daems, J. et al. (2017)** ‘Towards a IIIF-based corpus management platform’, in. Digital
Humanities Benelux 2017. Available at: http://hdl.handle.net/1854/LU-8538793 (Accessed: 18
May 2024).  
**Delmas-Glass, E. and Sanderson, R.** (2020) ‘Fostering a community of PHAROS scholars
through the adoption of open standards’, Art Libraries Journal, 45(1), pp. 19–23. Available at:
https://doi.org/10.1017/alj.2019.32.  
**Felsing, U. et al. (2023)** ‘Community and Interoperability at the Core of Sustaining Image
Archives’, Digital Humanities in the Nordic and Baltic Countries Publications, 5(1), pp. 40–54.
Available at: https://doi.org/10.5617/dhnbpub.10649.  
**Freire, N. et al.** (2017) ‘A survey of Web technology for metadata aggregation in cultural
heritage’, Information Services & Use, 37(4), pp. 425–436. Available at:
https://doi.org/10.3233/ISU-170859.  
**Freire, N. et al. (2018)** ‘Cultural heritage metadata aggregation using web technologies: IIIF,
Sitemaps and Schema.org’, International Journal on Digital Libraries [Preprint]. Available at:
https://doi.org/10.1007/s00799-018-0259-5.  
**Gomez, J., Clarke, K.S. and Vuong, A.** (2020) ‘IIIF by the Numbers’, The Code4Lib Journal,
2020(48). Available at: https://journal.code4lib.org/articles/15217 (Accessed: 17 May 2024).  
**Manz, M.C., Raemy, J.A. and Fornaro, P.** (2023) ‘Recommended 3D Workflow for Digital
Heritage Practices’, in Archiving Conference. Archiving 2023, Oslo, Norway: Society for
Imaging Science and Technology, pp. 23–28. Available at:
https://doi.org/10.2352/issn.2168-3204.2023.20.1.5.  
**Raemy, J.A.** (2017) The International Image Interoperability Framework (IIIF): raising
awareness of the user benefits for scholarly editions. Bachelor’s thesis. HES-SO University of
Applied Sciences and Arts, Haute école de gestion de Genève. Available at:
https://sonar.ch/hesso/documents/314853 (Accessed: 21 May 2024).  
**Rossenova, L. (2023)** ‘IIIF for 3D – making web interoperability multi-dimensional’, Europeana
PRO, 14 November. Available at:
https://pro.europeana.eu/post/iiif-for-3d-making-web-interoperability-multi-dimensional
(Accessed: 14 May 2024).  
**Weinthal, D. and Childress, D. (2019)** ‘IIIF for Open Access’. Open Access Week, UCLA, Los
Angeles, CA, USA, 23 October. Available at: https://escholarship.org/uc/item/260616w7
(Accessed: 18 May 2024)  
  
#### Ne pas prendre en compte dans le plan  
Structure à reprendre  
Argument  
**sous-argument 1 :**  
*exemple.:*  
**sous-argument 2 :**  
*exemple.:*  
  
#### Vérifier à chaque validation:  
CONF  
AJOUTER BIBLIO  
  
#### à mentionner:  
graphes de reduction comparative des archives  
graphes de performance  

#### caractéristiques formelles du master
travail écrit en LaTeX
ajout de table de matières 
ajout d'une section annexes 

