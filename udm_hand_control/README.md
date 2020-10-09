# udm_hand_control

Dans ce projet il y a deux launchfile un pour lancer les services qui utilisent la cinematique direct et l'autre qui utilise la cinematique inverse.

Pour les utiliser il faut s'assurer que vous avez lancer le demo.launch qui se trouve dans le moveit config que vous avez genere avec le setup assistant

Vous devez vous assurer que les group_name qui est en parametre concorde avec les groupes que vous avez configurer avec le movit setup assistant.

```sh
roslaunch udm_hand_control direct.launch

OR

roslaunch udm_hand_control indirect.launch
```
