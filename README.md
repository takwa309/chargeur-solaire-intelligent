
# Chargeur Solaire Intelligent avec STM32 & FreeRTOS

# Projet de fin d'année – Systèmes Embarqués


Ce projet consiste à concevoir un chargeur solaire intelligent basé sur un microcontrôleur **STM32F446RE** avec **FreeRTOS**. Il permet de charger une batterie Li-ion en optimisant l'énergie du panneau solaire.

## 📦 Structure du Projet

**Le code source complet** (projet STM32CubeIDE) est disponible dans le fichier :  
`[PFA-20250609T185842Z-1-001.zip]`  

---
## 🛠️ Stack Technique

![Langage](https://img.shields.io/badge/Langage-C_embarqué_(STM32_HAL)-00599C?style=flat&logo=c&logoColor=white)
![IDE](https://img.shields.io/badge/IDE-STM32CubeIDE-03234B?logo=stmicroelectronics)
![Simulation](https://img.shields.io/badge/Simulation-Proteus-00AEEF)

## 🧠 Objectifs

- Lire les tensions et courants du panneau et de la batterie via **INA219**
- Implémenter un algorithme **MPPT** pour maximiser la puissance
- Gérer la commutation entre **source panneau** et **adaptateur secteur**
- Afficher les données sur un **écran OLED SSD1306 **
- Organiser le projet avec **FreeRTOS**
- afficher en temps réel les données de la batterie (tension et courant) dans une application mobile

---

## ⚙️ Matériel utilisé && Diagramme global de fonctionnement

![image](https://github.com/user-attachments/assets/74f7d634-4c27-4bd7-8688-d24acf8f7a5a)


---

## 🧵 Architecture logicielle (FreeRTOS)

- `TaskINA_Panneau`: Lecture tension/courant panneau
- `TaskINA_Battery`: Lecture tension/courant batterie
- `TaskMPPT`: Contrôle PWM pour MPPT
- `TaskDisplay`: Affichage OLED
- `TaskSourceSwitch`: Bascule source (panneau/adaptateur)
- `TaskCommunication`:  Communication via ESP8266

---


## 📸 Exemples visuels
![image](https://github.com/user-attachments/assets/0de707da-1ee0-4421-adac-29b8fb2b6754)

![image](https://github.com/user-attachments/assets/1c20f97c-6920-4ad1-be0b-1e609734400b)


---

## 📄 Auteurs

-  Jazi Takwa
-  Année : 2025

---
