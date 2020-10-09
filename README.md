# TP3
D'abord il faut commence par importer nos fichier, et pour cela on va commencer par créer les répertoires par les commandes suivantes :
```
mkdir catkin_ws
cd catkin_ws
mkdir src
cd src
git clone https://github.com/ferio06/TP3.git
```
Après on procède par l'installation de MoveIt, pour cela ouvrir un terminal
et taper : 
```
sudo apt-get install ros-melodic-moveit
```
Une fois que c'est fait, il faudra maintenant lancer le build des packages qu'on vient de télécharger,pour cela ouvrir un terminal dans le repertoire catkin_ws et lancer la commande : 
```
catkin build
source devel/setup.bash
```

Maintenant on peut lancer le package qui nous permet controller les mouvements de notre robot par le package qu'on a créer precedement par le service :
```
roslaunch moveit_setup_assistant setup_assistant.launch
```
Pour cela on lance la commande :
```
roslaunch udm_hand_moveit_configs demo.launch
```
On laisse le service se lancer puis on ouvre un autre terminale dans le même dossier catkin_ws pour lancer le service pour le package udm_hand_control pour contrôler les mouvents de la main robot par cinematique direct et indirect par les commandes :
```
roslaunch udm_hand_control direct.launch
```
```
roslaunch udm_hand_control indirect.launch
```


