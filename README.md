# PatternParser

(En Français)
C'est projet a été devéloppé dans la cadre du course MGL843-01 season 2017 (École de Technologie Supérieure), du Prof. Christopher Fuhrman (https://github.com/fuhrmanator).

C'est un outil qui visualise le patron de conception adaptateur en utilisant la sortie du logiciel Tsantalis, la sortie de JDT2Famix, pharo (comme langage de programmation), MOOSE model et ROASSAL.

Modèle de Visualisation 

![Modele de Visualisation](https://github.com/tebo93/PatternParser/blob/master/imagen%20modelo%20de%20visualisation.PNG)

Afin de visualiser le patron adaptateur, il est utilisé le Tsantalis (https://users.encs.concordia.ca/~nikolaos/pattern_detection.html), qui génére un fichier XML à partir du code source du logiciel (avec tous les patrons détéctés). Avec JDT2Famix (https://github.com/girba/jdt2famix), il est généré un fichier .MSE (à partir du code source du logiciel) qui est importé dans MOOSE Model (http://www.moosetechnology.org/).

Finalement, en utilisant ROASSAL (http://agilevisualization.com/) et Pharo (http://pharo.org/), il est parsé le fichier généré par Tsantalis et il est visualisé chaque instance du patron.


![Captura 1](https://github.com/tebo93/PatternParser/blob/master/Capture%201.PNG)

![Captura 2](https://github.com/tebo93/PatternParser/blob/master/Captura%202.PNG)

Ici, on peut voir une petite demonstration

![Demonstration](https://raw.githubusercontent.com/tebo93/PatternParser/master/Demo.mp4)

Afin d'utiliser le code pharo à disposition, il faut changer le 'package' du projet, sur la ligne de code #4.

((each container mooseName beginsWith:'net::sourceforge' ) and: (each name beginsWith: '$' ) not )

pour

((each container mooseName beginsWith:'Le package de votre projet' ) and: (each name beginsWith: '$' ) not )

(In English)

This project was developped on MGL-843 course (École de Technologie Supérieure), taught by Prof. Christopher Fuhrman (https://github.com/fuhrmanator).

This tool parses the design pattern Adapter using the output generated by Tsantalis, the output generated JDT2Famix, pharo (as programming language), MOOSE model and ROASSAL.

Visualization Model

![Visualization Model](https://github.com/tebo93/PatternParser/blob/master/imagen%20modelo%20de%20visualisation.PNG)

In order to visualizate the pattern, the Tsantalis is used (https://users.encs.concordia.ca/~nikolaos/pattern_detection.html), for generating an XML file from the project's source code (which contains all patterns detected). With JDT2Famix (https://github.com/girba/jdt2famix), a .MSE file is generated (form the project's source code) which is imported within MOOSE Model(http://www.moosetechnology.org/).

Finally, ROASSAL (http://agilevisualization.com/) and Pharon (http://pharo.org/), for parsing the XML file generated by Tsantalis and visulize each instance of the pattern.

![Captura 1](https://github.com/tebo93/PatternParser/blob/master/Capture%201.PNG)

![Captura 2](https://github.com/tebo93/PatternParser/blob/master/Captura%202.PNG)

Here, we can see a demo.

![Demo](https://raw.githubusercontent.com/tebo93/PatternParser/master/Demo.mp4)

To use the code, you have to change the package of the project in the line of code #4.

((each container mooseName beginsWith:'net::sourceforge' ) and: (each name beginsWith: '$' ) not )

for

((each container mooseName beginsWith:'your project package' ) and: (each name beginsWith: '$' ) not )

