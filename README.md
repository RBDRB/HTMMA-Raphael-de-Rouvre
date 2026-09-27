# HTMMA-Raphael-de-Rouvre
## Traqueur GPS Hors-ligne
Le PCB est destiné à construire un GPS de randonnée hors ligne.
L'objectif n'est pas de reproduire une smartwatch ou un GPS de navigation complet, mais de faire un petit appareil simple et autonome (sauf affichage externe en wifi sur l'ESP) pour l'exécution d'une trace GPX et le suivi d'une trace GPX.

### Choix des composants 

- Calculateur : Pour faire fonctionner les composants entre eux, traiter le GPX et l'interface graphique, et la transmettre en wifi
-> XIAO ESP 32 S3 : Celui à disposition, mais qui s'est avéré parfait pour le projet avec sa taille réduite et ses nombreux GPIO
  
- GPS : Pour récuperer la position en temps réel de l'appareil
-> ATGM336H : Module GNSS peu coûteux, compact, faible consommation par rapport à de nombreuses solutions GNSS plus complexes, sortie UART simple
  
- Mesure d'altitude
-> BMP280 : Très petit, très faible consommation et interface I²C/SPI simple

- Contrôles : Pour naviguer sans écran tactile
-> EC11

- Buzzer : Pour les alertes

- Stockage : Pour conserver les GPX
-> Port à carte Micro-SD

- Condensateurs : Stabiliser 
 

<img width="498" height="314" alt="image" src="https://github.com/user-attachments/assets/cd4f560d-caed-43cd-b3c7-fa0f0a40ed6f" />

### Disposition 

Port USB-C de l'ESP 32 et port Micro SD accessibles 

<img width="416" height="283" alt="image" src="https://github.com/user-attachments/assets/62ac223b-32ca-4e3c-9e3e-7ed891bef9df" />

### Rendu 3D : 

Affichage et Alimentation à part 

<img width="384" height="254" alt="image" src="https://github.com/user-attachments/assets/d9a1e306-4964-4eab-a945-d08d16d2dfb6" />
