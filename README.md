# SmartSensorTracker
SmartSensor Tracker : Système IoT de collecte et d’analyse en temps réel


# SmartSensorTracker : Simulateur de capteurs (PYTHON) + Base NoSql (MONGODB) + Interface API (Serveur Node.js) + Dashboard Web (ReactJS)
 
Le projet SmartSensor Tracker, conçu pour collecter, stocker et visualiser en temps réel des données issues de capteurs IoT. Le système utilise une base NoSQL MongoDB, un déclencheur périodique pour les mesures, et un tableau de bord interactif pour l’analyse. La digitalisation industrielle nécessite une surveillance précise des paramètres comme la température, l’humidité et la lumière. SmartSensor Tracker répond à ces besoins avec une collecte rapide, un stockage évolutif et une consultation en temps réel.
Objectifs :
- Collecte rapide de données hétérogènes provenant de milliers de capteurs
- Stockage évolutif et flexible
- Requêtes analytiques sur des périodes glissantes
- Monitoring temps réel

## 1. Cahier de charges

>  * Objectifs fonctionnels

- Enregistrement des mesures toutes les 10 secondes
- Consultation par site, capteur ou plage de dates
- Alerte en cas de dépassement de seuil
- Affichage graphique des tendances
- Export des données en CSV

  * Modèle de données NoSQL

Type de base : MongoDB (orientée document)

Structure des documents :
{
  "capteur_id": "SENS1234",
  "site": "Usine Nord",
  "type": "température",
  "mesures": [
{ "timestamp": "2025-05-01T08:00:00Z", "valeur": 23.4 },
{ "timestamp": "2025-05-01T08:00:10Z", "valeur": 23.6 }
]
}

Modélisation : Embedding des mesures dans les documents capteurs, ou referencing selon la volumétrie.

  * Spécifications techniques

- 10 000 capteurs actifs
- 1 mesure toutes les 10 secondes => ~86 millions de mesures/jour
- Temps de réponse attendu < 150 ms sur les dernières 24h
- Stockage sur MongoDB Atlas (Cloud), cluster M10

## 2. Application/outil utilisés
## 3. Dataset
## 4. Objectif
## 5. Architecture (cf. image.png)
## 5. Resultat
