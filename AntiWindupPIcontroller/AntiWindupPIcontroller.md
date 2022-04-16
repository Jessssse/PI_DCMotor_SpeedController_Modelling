Model of Anti - Windup![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.001.png) PI controller for ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.002.png)BLDC Motor 

CORRECTEUR LINÉAIRE AVEC INDUCTANCE NÉGLIGÉE 

- **HYPOTHÈSE 1 :  ON NÉGLIGE L’INDUCTANCE DU MOTEUR  ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.003.png)**

CORRECTEUR LINÉAIRE AVEC INDUCTANCE NÉGLIGÉE 

Comportement  cible :    1

2 2 + 1 + 1

` `SE ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.004.jpeg)

TEMPS (S)

Paramètre de la fonction cible : Amortissement = 1 

𝑡95% = 3 = 40 ms   

Dimensionnement :

1. Trouver la forme de la fonction de transfert du correcteur
1. Identifier les coefficients à partir des grandeurs physiques et du cahier des charges
1. Vérification de la réponse en continu 
1. Passage du correcteur en discret Fonction de transfert moteur : 
- =

× + ( × + 2)

CORRECTEUR LINÉAIRE AVEC INDUCTANCE NÉGLIGÉE 

Comparaison entre le correcteur continu et discret ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.005.png)

` `SE  ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.006.jpeg)

3

TEMPS (S)


CORRECTEUR LINÉAIRE AVEC INDUCTANCE NÉGLIGÉE ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.007.png)

- **RÉSULTAT SUR LES 2 MODÈLES LINÉAIRES**

MODÈLE MOTEUR INDUCTANCE NÉGLIGÉE![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.008.jpeg)

VITESSE (RPM)

MODÈLE MOTEUR LINÉAIRE COMPLET

TEMPS (S)

CORRECTEUR LINÉAIRE COMPLET 
|<p>E :</p><p>E DE LA NSFERT DU </p><p>FFICIENTS </p><p>A RÉPONSE EN </p><p>ECTEUR EN URATION </p><p>RT MOTEUR : </p>|
| - |
|<p>2</p><p>- × + × +</p>|<p>2</p><p>- + ( × +</p>|
- **HYPOTHÈSE 2 : PRISE EN COMPTE DE L’INDUCTANCE** COMPORTEMENT  CIBLE :   K3P3 + 2 2 +K1 + 1

PAR AM

𝑡95% DIM

1. T F
1. I 3.

\4.

` `SE  5.

FON

- =

)

TEMPS (S)

MODÈLE MOTEUR LINÉAIRE COMPLET![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.009.jpeg)![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.010.png)

DISCRET CONTINU 

` `SE 

TEMPS (S)


ANTI-WINDUP GESTION DE LA SATURATION DE L’INTÉGRATEUR![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.011.png)

Anti-saturation en tension/courant (AntiWindup):  En boucle fermée, en rajoutant une saturation en sortie du bloc intégrateur, en cas d’atteinte de limite, la sortie est gelée.   Pour cela, il faut prendre en compte la saturation directement dans le bloc intégrateur.

Correcteur 

Erreur Correcteur Gain Bloc 

Intégrateur DC Intégrateur anti-windup

![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.012.png)

INTEGRATEUR MODELES SIMULINK![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.013.png)

Forward Euler method intégrateur simple : ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.014.jpeg)

y(n) = y(n-1) + K\*Te\*u(n-1)  avec Te = t(n) - t(n-1) y(n) : sortie de l’intégrateur  

Te = t(n) - t(n-1) : période d’echantillonnage, écart de temps  entre 2 point. 

K : gain  

Source : documentation Matlab

Ajout de la gestion de la saturation : ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.015.png)![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.016.png)![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.017.png)

Let's work ![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.005.png)![](Aspose.Words.40fd143d-7565-4654-8d92-95a99ee0839a.018.jpeg)linkedin together

16
