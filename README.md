Ce projet s'inscrit dans le Bloc 2 de l'Académie de Programmation IFRI, consacré au génie logiciel. Le module porte sur l'architecture logicielle et la modularité : apprendre à organiser un projet pour qu'il reste lisible, maintenable et extensible même quand il grossit.

Le point de départ est le code du Module 1 — la page DevStart Agency. L'objectif est de le réorganiser selon un principe simple : une partie du code, une seule responsabilité . Au lieu d'un seul fichier style.cssqui gère la navigation, le héros, les cartes, les témoignages et le footer en même temps, chaque section de la page prend son propre fichier CSS. La page doit rester visuellement identique après la réorganisation — aucune régression n'est tolérée.

Le travail s'est déroulé en trois phases. La première est la cartographie de l'existant : comprendre ce qui est là avant de toucher à quoi que ce soit. La deuxième est la conception de l'architecture cible : planifier la nouvelle structure sur papier avant de créer le moindre fichier. La troisième est l'implémentation : créer la structure réelle, découper le CSS, vérifier que tout fonctionne, puis pousser le résultat sur GitHub.

La branche mainconserve le code original du Module 1, non modifié. La branche module2contient le code réorganisé selon l'architecture conçue par le groupe. Les commits sont réguliers et chaque message décrit clairement ce qui a été fait.

Euloge SOZAN — Chef de groupe. Il a piloté le projet de bout en bout, créé le dépôt GitHub, ouvert la branche module2, maintenu le README et coordonné les échanges entre les membres. Il a également rédigé l'introduction du document d'architecture et assuré l'ouverture et la conclusion de la présentation orale.

Iréti Folakè Thérèsa Sarah BADOU — Cartographie HTML. Elle a ouvert le fichier index.htmldu Module 1 et identifié toutes les sections de la page : en-tête, héros, services, à propos, témoignages, contact et pied de page. Pour chaque section, elle a documenté ce qu'elle affiche et les ressources dont elle dépend. Elle a ensuite produit le schéma de cartographie HTML et rédigé la section correspondante dans le document d'architecture.

SOSSOU Merveilles de Dieu — Cartographie CSS. Il a analysé le fichier style.cssen profondeur, listé toutes les règles et les a regroupées par section logique. Il a identifié les styles globaux destinés à devenir base.css— variables de couleurs, polices, réinitialiser — et repéré les duplications existantes. Il a produit le tableau de cartographie CSS et a rédigé la section correspondante dans le rapport.

Aristote Léon Egnon HOUNTONDJI — Conception de l'architecture. À partir des cartographies d'Iréti et Merveilles, il a conçu la structure de dossiers cibles avec tous ses sous-dossiers : styles/, components/, pages/, assets/. Pour chaque fichier CSS prévu, il a défini son nom, sa responsabilité en une phrase et les éléments HTML qu'il allait gérer. Il a également anticipé l'intégration des futures pages Portfolio, Blog et Espace Client, et justifié chaque choix dans le document d'architecture.

Houéfa Immaculée Christelle AHOLOU — Implémentation et vérification. Elle a créé la structure de dossiers réels sur la machine selon le plan d'Aristote, découpés style.cssen fichiers séparés, mis à jour les balises <link>dans index.htmlet vérifiés que la page s'affiche identiquement après le découpage. Elle a poussé le code sur la branche module2avec des engagements clairs, réalisé la conclusion du rapport et assuré la démonstration en direct lors de la soutenance.

Les livrables du groupe sont un document d'architecture en PDF, le code CSS découpé disponible sur la branche module2et une présentation orale de 12 minutes devant l'académie.
