# PDP-Tracking

## Dépendances

Le système de build repose sur [catkin_tools](https://catkin-tools.readthedocs.io).

Il peut être installé avec des droits utilisateurs au cremi:

    pip install -U catkin_tools

Vous pourrez trouver un récapitulatif des commandes de `catkin-tools` sur le
[site officiel](https://catkin-tools.readthedocs.io/en/latest/cheat_sheet.html).

Si nécessaire, modifiez votre `.bashrc` pour ajouter le dossier contenant catkin
à votre `PATH`, par exemple:

    export PATH=$PATH:~/.local/bin

## Initialisation du dépôt

Après avoir cloné le dépôt, initialiser les sous-module:

    git submodule init
    git submodule update

Pour créer un profile de compilation vous pouvez exécuter la commande suivante:

    catkin config --profile release -x _release --cmake-args -DCMAKE_BUILD_TYPE=Release
    
Ensuite pour compiler l'ensemble du projet, il suffit d'exécuter la commande suivante:

    catkin build --profile release


L'outil de labelling en cours de développement sera accessible au chemin suivant:
`devel_release/lib/hl_labelling/gtk_labelling_tool`.

## Données

Afin de pouvoir travailler sur des données réalistes, vous pouvez télécharger
les [logs de la première mi-temps de la finale 2019](http://ludovic.hofer.emi.u-bordeaux.fr/Finale_2019_1st_half.tar.gz)
