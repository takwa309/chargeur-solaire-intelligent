
# Chargeur Solaire Intelligent avec STM32 & FreeRTOS

# Projet de fin d'année – Systèmes Embarqués
`Public`  

● **C embarqué (STM32 HAL)**  
● FreeRTOS  
● STM32CubeIDE  
● Proteus  

![Badge C embarqué](https://img.shields.io/badge/Embedded_C-STM32_HAL/LL-00599C?logo=c&logoColor=white)

Ce projet consiste à concevoir un chargeur solaire intelligent basé sur un microcontrôleur **STM32F446RE** avec **FreeRTOS**. Il permet de charger une batterie Li-ion en optimisant l'énergie du panneau solaire.



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

## 🗂️ Organisation du dépôt

- `/Core`, `/Drivers`, `/Middlewares` : Arborescence STM32CubeIDE
- `/Src`, `/Inc` : Code source principal et headers
- `/images` : Schémas Proteus, captures d’écran OLED
- `/docs` : Cahier des charges, rapports techniques

---

## 📸 Exemples visuels
![image](https://github.com/user-attachments/assets/0de707da-1ee0-4421-adac-29b8fb2b6754)

![image](https://github.com/user-attachments/assets/1c20f97c-6920-4ad1-be0b-1e609734400b)


---

## 📄 Auteurs

- 👩‍💻 Jazi Takwa
- 📅 Année : 2025

---
