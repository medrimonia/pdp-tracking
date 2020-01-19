# PDP-Tracking

## Initialisation du dépôt

Après avoir cloné le dépôt, initialiser les sous-module:

    git submodule update

Le système de build repose sur [catkin_tools](https://catkin-tools.readthedocs.io).
Pour créer un profile de compilation vous pouvez exécuter la commande suivante:

    catkin config --profile release -x _release --cmake-args -DCMAKE_BUILD_TYPE=Release
    
Ensuite pour compiler l'ensemble du projet, il suffit d'exécuter la commande suivante:

    catkin build --profile release

Vous pourrez trouver un récapitulatif des commandes de `catkin-tools` sur le
[site officiel](https://catkin-tools.readthedocs.io/en/latest/cheat_sheet.html).

L'outil de labelling en cours de développement sera accessible au chemin suivant:
`devel_release/lib/hl_labelling/gtk_labelling_tool`.

