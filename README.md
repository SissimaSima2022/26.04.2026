Je souhaite restaurer un site web à partir de fichiers existants. Les ressources du projet sont contenues dans une archive compressée nommée 26.04.2026.8.43.zip. Merci d’utiliser ces fichiers comme base principale pour le développement. Le projet est également disponible sur GitHub via le lien suivant : https://github.com/SissimaSima2022/21.04.2026.git Objectifs : Extraire et analyser le contenu de l’archive Comprendre et reproduire la structure actuelle du projet Améliorer si nécessaire l’organisation et la qualité du code Mettre en place un site web fonctionnel, propre et responsive Respecter au maximum le design et la logique du projet initial Contraintes techniques : Conserver une structure de fichiers similaire à celle du fichier ZIP d’origine (PHP, CSS, JS, etc.) Le code final devra être facilement re-déployable sous forme d’archive ZIP, avec la même organisation Le site sera hébergé sur un serveur Apache 2 Accès au serveur via SSH (Termius) Gestion des fichiers avec FileZilla Précision importante : Lors des modifications futures, je souhaite que chaque version du projet puisse être téléchargée sous forme d’archive respectant strictement la structure initiale, afin de pouvoir l’uploader directement sur mon serveur sans ajustements supplémentaires. comme j'ai l'abitude de faire : sudo rm -rf /var/www/public_html/nassima/* && sudo rm -rf /var/www/public_html/nassima/.[!.]* puis # 2. Uploader le nouveau ZIP via FileZilla dans /var/www/public_html/nassima/ comme suit cd /var/www/public_html/nassima sudo unzip -o enstsa-php-site.zip sudo rm enstsa-php-site.zip # 3. Permissions sudo chown -R www-data:www-data /var/www/public_html/nassima sudo chmod -R 755 /var/www/public_html/nassima sudo chmod -R 775 /var/www/public_html/nassima/data sudo systemctl restart apache2 Puis ouvrez http://votre-domaine/nassima/ → vous verrez tous les nouveaux contenus avec la section Statistiques animée sur la page d'accueil.
je souhaite aussi dans la partie "Chiffres clés L'ENSTSA en quelques chiffres" quand je clique sur 541 étudiant pop up s'affiche pour m'afficher les détails suivant: 
Preparatory Cycle

**1st Year**

* Enrolled students: 201
* On academic leave: 14
* Registered students: 215

**2nd Year**

* Enrolled students: 196
* On academic leave: 10
* Registered students: 206

**Total Preparatory Cycle:** 421 étudiants

---

### 🔹 Specialty Cycle

**1st Year – Autonomous Embedded Systems Engineering**

* Enrolled students: 38
* On academic leave: 1
* Registered students: 39

**2nd Year – Robotics and Autonomous Systems Design**

* Enrolled students: 37
* On academic leave: 3
* Registered students: 40

**3rd Year – Navigation and Control of Unmanned Systems**

* Enrolled students: 41
* On academic leave: 0
* Registered students: 41

**Total Specialty Cycle:** 120 étudiants

---

### 🎨 Design attendu

* Une interface **moderne, claire et innovante**
* Utilisation des **couleurs principales du site : bleu et orange**
* Intégration de **graphiques en cercle (pie charts)** pour visualiser :

  * Répartition Preparatory vs Specialty
  * Statut des étudiants (enrolled / leave / registered)
* Mise en page fluide avec sections bien séparées et lisibles

L’objectif est d’avoir une **visualisation intuitive et professionnelle** des données dans une pop-up élégante.

Je souhaite implémenter la même fonctionnalité pour la section “Teachers” (Enseignants).
Au clic, une fenêtre pop-up moderne et innovante doit s’afficher avec les statistiques suivantes, présentées en français, anglais et arabe :

👨‍🏫 Teachers Statistics | Statistiques des enseignants | إحصائيات الأساتذة
🔹 Détails | Details | التفاصيل
Professor | Professeur | أستاذ : 6
Associate Professor (Class A) | Maître de conférences A | أستاذ محاضر قسم "أ" : 6
Associate Professor (Class B) | Maître de conférences B | أستاذ محاضر قسم "ب" : 14
Assistant Professor (Class A) | Maître assistant A | أستاذ مساعد قسم "أ" : 2
Assistant Professor | Maître assistant | أستاذ مساعد : 20
Temporary Teachers | Enseignants vacataires | أساتذة مؤقتة : 33
Seconded Teachers | Enseignants en mise à disposition | أساتذة تحت وضع التصرف : 4
🔸 Total | Total | المجموع

85 enseignants | 85 teachers | 85 أستاذ

🎨 Design attendu
Pop-up moderne et professionnelle
Couleurs principales : bleu et orange
Ajout d’un graphique en cercle (pie chart) montrant la répartition des enseignants par catégorie
Interface claire, bien organisée et responsive
Possibilité d’afficher les langues de manière élégante (tabs, icônes ou sections)

L’objectif est d’obtenir une visualisation claire, multilingue et intuitive des statistiques des enseignants.

Je souhaite ajouter, dans la section “Employés”, l’organigramme de l’école.

🔹 Fonctionnalité demandée
Intégrer un organigramme clair et structuré représentant :
Le directeur
Les sous-directions
Les différents services administratifs, techniques et pédagogiques
L’organigramme doit refléter fidèlement la hiérarchie présentée dans les images fournies.dans une fenêtre pop-up moderne (comme pour les étudiants et enseignants).Design attendu
Interface moderne, fluide et professionnelle
Respect de la charte graphique du site (bleu et orange)
Organigramme sous forme :
de blocs (cards) reliés entre eux
avec une hiérarchie bien visible
Support du multilingue (arabe / français / anglais) si possible
Compatible responsive (mobile + desktop).Organigramme de l’école
🔹 Direction
Directeur
🔹 Structures rattachées à la Direction
Secrétaire général
Directeur de la bibliothèque
Chef du département de la formation de base
Chef du département d’ingénierie des systèmes autonomes
🔹 Sous-direction de la pédagogie et de la formation
Sous-directeur chargé de la formation, des diplômes et de la formation continue
Chef du service de l’enseignement et de l’évaluation
Chef du service de la formation continue et des certifications
Chef du service de suivi pédagogique et assurance qualité
🔹 Sous-direction de la recherche et du développement
Sous-directeur chargé de la formation doctorale, de la recherche scientifique, du développement technologique et de l’innovation
Chef du service de la formation doctorale et recherche
Chef du service de suivi et valorisation de la recherche
Chef du service de l’innovation et entrepreneuriat
Chef du service du développement technologique
🔹 Sous-direction de la communication et des systèmes d’information
Sous-directeur chargé des systèmes d’information, de la communication et des relations extérieures
Chef du service des systèmes d’information et réseaux
Chef du service des statistiques et de la prospective
Chef du service communication et relations extérieures
🔸 Secrétariat Général
🔹 Sous-direction des ressources humaines et des activités
Chef du service des personnels enseignants
Chef du service des personnels administratifs et techniques
Chef du service des activités culturelles et sportives
Chef du service des affaires juridiques et contentieux
🔹 Sous-direction des finances et des moyens
Chef du service du budget et financement de la recherche
Chef du service des marchés et équipements
Chef du service des moyens généraux et archives
Chef du service de maintenance et entretien
🔹 Services techniques
Centre des systèmes et réseaux, communication et enseignement à distance
Service systèmes
Service réseaux
Service enseignement à distance
Centre audiovisuel
Service impression
Service audiovisuel
Centre d’enseignement intensif des langues
Service programmation et suivi
Service maintenance et support
🔸 Bibliothèque
Chef du service acquisition, traitement et conservation des documents
Chef du service bibliothèque numérique
Chef du service accueil et orientation
🎯 Objectif

Cet organigramme représente la structure hiérarchique complète de l’établissement, facilitant la compréhension des rôles, responsabilités et interactions entre les différents services.


dans la dernière "salle" pédagogiques": voici ce qu'on ajoute: 
L’établissement dispose de plusieurs infrastructures pédagogiques permettant d’assurer la formation des étudiants dans de bonnes conditions :

🏫 Détails des espaces
Salles de cours
Nombre de salles : 3
Capacité par salle : 40 étudiants
Capacité totale : 120 étudiants
Salles de travaux dirigés (TD)
Nombre de salles : 12
Capacité par salle : 30 étudiants
Capacité totale : 360 étudiants
Centres de calcul (informatique)
Nombre de salles : 3
Capacité par salle : 25 étudiants
Capacité totale : 75 étudiants
Laboratoires de langues
Nombre de salles : 1
Capacité : 25 étudiants
Amphithéâtres
Nombre : 4
Capacité par amphithéâtre : 250 étudiants
Capacité totale : 1000 étudiants
🔸 Capacité globale
Capacité totale d’accueil : 1580 étudiants
🎨 Affichage recommandé
Présentation sous forme de cartes (cards) ou tableau moderne
Ajout d’un graphique circulaire (pie chart) pour visualiser la répartition des capacités
Respect des couleurs du site : bleu et orange
Design moderne, clair et responsive
🎯 Objectif

Mettre en valeur les moyens pédagogiques et les capacités d’accueil de l’établissement de manière claire, visuelle et professionnelle.


pour la partie Cooperation:
Nous avons 8 partenariats et qui sont les suivants :
1-ATM Mobilis
Télécommunications et technologies de l’information
Présentation :
ATM Mobilis est l’opérateur national de téléphonie mobile et le leader des télécommunications en Algérie. L’entreprise s’engage dans l’innovation technologique, la modernisation de ses infrastructures et le développement des compétences nationales dans le numérique.
But de la convention :
Ce partenariat vise à renforcer la collaboration en recherche et développement dans le domaine des télécommunications, à créer un laboratoire de recherche mixte au sein de l’ENSTSA, ainsi qu’à favoriser la formation, l’encadrement des stages et la réalisation de projets communs. Il contribue également à accompagner la digitalisation et l’innovation, tout en encourageant la création de startups issues des travaux des étudiants.
Adresse :
Quartier d’Affaires d’Alger, îlots 05, lots 27, 28 et 29, Bab Ezzouar, Alger.
2-CDTA (Centre de Développement des Technologies Avancées)
Recherche scientifique et innovation technologique
Présentation :
Le CDTA est un établissement public à caractère scientifique et technologique, acteur majeur de la recherche appliquée en Algérie. Il intervient dans plusieurs domaines tels que la robotique, l’intelligence artificielle, la réalité augmentée et virtuelle, les systèmes embarqués, le cloud computing et l’industrie 4.0.
But de la convention :
Ce partenariat avec l’ENSTSA vise à mutualiser les efforts de recherche et d’innovation, notamment à travers le développement de projets technologiques multidisciplinaires. Il favorise la valorisation des PFE et des startups étudiantes, l’échange de chercheurs, l’accès partagé aux plateformes technologiques, ainsi que la co-organisation d’activités scientifiques et de formations spécialisées.
Adresse :
Lotissement du 20 Août 1956, B.P. 17, Baba Hassen, Alger.
3-ALCADWorks
Ingénierie assistée par ordinateur (CAO/FAO/IAO) et fabrication numérique
Présentation :
EURL ALCADWorks est une société algérienne spécialisée dans l’intégration de solutions de conception, simulation et fabrication assistées par ordinateur, la rétro-conception et le prototypage rapide. Elle est également distributrice de marques internationales telles que Dassault Systèmes SolidWorks et Hyundai WIA Machine Tools.
But de la convention :
Cette collaboration vise à renforcer la formation pratique et technique des étudiants, à développer des projets communs en conception et simulation industrielles, et à promouvoir la recherche appliquée dans les technologies de conception numérique. Elle prévoit également l’accueil de stagiaires, des échanges d’expertise et des actions de perfectionnement professionnel.
4-DeepMinds Technology Ltd
Intelligence artificielle, systèmes autonomes, innovation et entrepreneuriat
Présentation :
DeepMinds Technology est une entreprise technologique algérienne spécialisée dans l’intelligence artificielle, l’innovation numérique, l’accompagnement de startups et le développement de solutions basées sur les systèmes autonomes. Elle joue un rôle important dans l’écosystème entrepreneurial et technologique.
But de la convention :
Développer un partenariat scientifique dans l’IA et les systèmes autonomes
Intégrer les étudiants de l’ENSTSA dans les programmes d’incubation
Accueillir des stagiaires au sein des startups incubées
Organiser des séminaires, conférences et programmes de sensibilisation à l’entrepreneuriat
Développer des projets conjoints en innovation et création de startups
Adresse :
Mohammadia Mall, 4ᵉ étage, Bureau 1162, Alger.
5-École Nationale Polytechnique (ENP)
Enseignement supérieur et recherche en ingénierie
Présentation :
L’ENP est l’une des plus anciennes et prestigieuses écoles d’ingénieurs en Algérie. Elle assure la formation dans plusieurs domaines de l’ingénierie et joue un rôle majeur dans la recherche scientifique et l’innovation.
But de la convention :
Échanges de professeurs, chercheurs et doctorants
Encadrement mutuel des étudiants et des PFE
Projets de recherche communs et publications conjointes
Accès partagé aux laboratoires et plateformes scientifiques
Coopération pédagogique et renforcement de la formation
Collaboration en entrepreneuriat et innovation étudiante
Adresse :
10, Rue des Frères Oudek, El Harrach, Alger.
6-NESDA / ANADE (ex-ANSEJ)
Développement de l’entrepreneuriat
Présentation :
NESDA/ANADE est un organisme public chargé du soutien et du développement de l’entrepreneuriat en Algérie. Il accompagne les jeunes porteurs de projets et finance les micro-entreprises à travers des dispositifs d’appui.
But de la convention :
Mise en place et animation du Centre de Développement de l’Entrepreneuriat (CDE) au sein de l’ENSTSA
Accompagnement des étudiants porteurs de projets
Organisation de formations, ateliers et sessions de coaching
Renforcement de la culture entrepreneuriale
Encadrement des PFE liés à l’entrepreneuriat
Coordination pour encourager la création de startups
Adresse :
Cité AADL 2, Zéralda, Alger.
7-USTHB – Université des Sciences et de la Technologie Houari Boumediene
Sciences, technologies et recherche scientifique
Présentation :
L’USTHB est l’une des plus grandes universités scientifiques d’Algérie, reconnue pour son excellence en sciences, technologies et recherche appliquée.
But de la convention :
Développement de programmes de recherche conjoints
Mutualisation des ressources pédagogiques et scientifiques
Organisation de séminaires, ateliers et conférences
Encadrement des étudiants (PFE, mémoires, thèses)
Accueil de chercheurs et doctorants
Coopération sur les thématiques technologiques
Adresse :
BP 32 El Alia, 16111 Bab Ezzouar, Alger.
8-CRTI (Centre de Recherche en Technologies Industrielles)
Technologies industrielles
Présentation :
Centre spécialisé dans les matériaux, la mécanique, la métallurgie et le contrôle non destructif.
But de la convention :
Développement de projets de recherche communs, encadrement des étudiants et valorisation scientifique.
💡 Proposition d’interface (ce que tu demandes pour les logos + popup)
Ton idée est très bonne. Voici comment la structurer proprement :
🔹 Affichage principal
Une grille de logos (cards) :
Logo centré
Nom en dessous
🔹 Interaction
Au clic sur un logo :
ouverture d’une fenêtre popup (modal)
🔹 Contenu du popup
Nom de l’institution
Présentation
But de la convention
Adresse
Bouton : “Site officiel” (lien externe)
