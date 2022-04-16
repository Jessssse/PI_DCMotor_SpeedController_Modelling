# PI_DCMotor_SpeedController_Modelling

L'objectif de ce projet est de dimensionner un système d'asservissement en vitesse (régulation de la consigne)pour Moteur DC ( et équivalent BLDC). 

Les fonctions de transferts ont été calculés sur le logiciel WxMaxima : 
http://wxmaxima-developers.github.io/wxmaxima/

Les simulations sur Matlab/Simulink : 
https://fr.mathworks.com/


[correcteur 1e ordre](Calculs_correcteur/correcteur_1eordre_continu.wxmx) 
![correcteur 1e ordre](/images/Slide2.JPG)
![simulation correcteur modele moteur basique](/images/Slide3.JPG)
![simulation correcteur modele moteur ordre 2](/images/Slide4.JPG)
![correcteur 3e ordre](/images/Slide5.JPG)
![simulation correcteur modele moteur ordre 2](/images/Slide6.JPG)
![Intégrateur anti wind-up](/images/Slide7.JPG)
![Modéle Simulink anti-windup](/images/Slide8.JPG)

