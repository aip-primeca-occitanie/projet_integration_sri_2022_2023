Le package sri_tiago_pick permet de lancer une opération de saisie dans la simulation du monde. Celle-ci est basée sur le tutoriel de pick de tiago mais légèrement modifié pour qu'il soit adapté au monde groix_porquerolles.world. 

Une démo peut être lancée en utilisant trois terminaux différents (voir README.md de la branche principale). Celle-ci fait apparaître le robot devant une table du monde et lance une opération de pick. Le robot doit d'abord détecter le cube via son QR-Code puis déplace son bras avec une opération de saisie que le robot choisi. La position en x est légèrement modifiée dans le code afin de calibrer la position de saisie par rapport à la réelle position du cube. Sans cette calibration, le bras du robot était mal placé et poussait le cube. Lorsque le robot a bien saisi le cube, il le soulève et la démo se termine. Précédemment, le robot posait juste après le cube au même endroit qu'il se trouvait, mais cette partie "place" se fait via le package tiago_place.