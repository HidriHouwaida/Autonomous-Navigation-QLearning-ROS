# 🚀 Projet de Navigation Autonome avec Q-Learning sur ROS

**Mise en œuvre d'algorithmes intelligents pour la navigation d'un robot Mini-Lab dans Gazebo**

## 📌 Aperçu
Ce projet implémente un système de navigation autonome basé sur le **Q-learning** pour le robot Mini-Lab, simulé dans **ROS/Gazebo**. Il combine :
- Apprentissage par renforcement (Q-learning)
- Traitement des données Lidar/odométrie
- Contrôle des mouvements via ROS


## 🛠️ Prérequis
- **ROS Noetic** 
- **Gazebo** 
- **Python 3** avec bibliothèques :
  ```bash
  pip install numpy pandas matplotlib rospy

🧠 Fonctionnalités Clés

Apprentissage en temps réel : <br>
Adaptation dynamique aux obstacles <br>

Visualisation : <br>
Graphiques des récompenses cumulées
Trajectoire du robot en 2D <br>

Sécurité : <br>
Détection de collision via Lidar

📊 Résultats Attendus  <br>
Navigation autonome vers une cible définie <br>
Évitement d'obstacles intelligent <br>
Fichiers CSV historisant les états/apprentissages



## 📝 Fichiers Importants

| Fichier                | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `Q_Learning.py`        | Implémente la table Q, la politique d'action et le contrôle ROS via `cmd_vel` |
| `SensorDataLogger.py`  | Enregistre en temps réel les données des capteurs (Lidar/Odométrie/IR) dans des CSV |
| `Odometre_Data.csv`    | Historique des positions (x,y,z) et orientations (quaternions) du robot      |
| `Lidar_Data.csv`       | Mesures des obstacles (angles + distances), valeurs infinies remplacées par 1000 |
| `Ultrason_Data.csv`    | Données des capteurs IR (5 capteurs) pour la détection rapprochée            |
