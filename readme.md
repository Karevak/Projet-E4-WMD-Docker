# Multi-Application Docker Deployment Project



Ce projet démontre le déploiement de 5 applications web différentes utilisant Docker et Nginx comme reverse proxy. Le projet inclut la configuration de haute disponibilité, l'optimisation des images Docker et l'automatisation du déploiement.



## 🚀 Applications déployées



- docs-django-grafana (Port: 9005)

- docs-django-react (Port: 9001)

- ecommerce-flask-stripe (Port: 9002)

- flask-soft-ui-design (Port: 9003)

- rocket-ecommerce (Port: 9004)



## 📋 Prérequis



- Docker

- Docker Compose

- Git



## 🛠️ Installation



1. Cloner le repository :

```bash

git clone https://github.com/votre-username/docker-apps-deployment.git

cd docker-apps-deployment

```



2. Lancer les applications :

```bash

docker-compose up -d

```



## 🔍 Architecture



Le projet est structuré de la manière suivante :

```

docker-apps-deployment/

├── apps/

│   ├── docs-django-grafana/

│   ├── docs-django-react/

│   ├── ecommerce-flask-stripe/

│   ├── flask-soft-ui-design/

│   └── rocket-ecommerce/

├── nginx/

│   └── nginx.conf

└── docker-compose.yml

```



## 🌐 Accès aux applications



- docs-django-grafana : http://localhost:9005

- docs-django-react : http://localhost:9001

- ecommerce-flask-stripe : http://localhost:9002

- flask-soft-ui-design : http://localhost:9003

- rocket-ecommerce : http://localhost:9004 (accès direct sans reverse proxy)



Via Nginx (port 80) :

- /grafana/

- /react/

- /stripe/

- /ui/



## 🔄 CI/CD Workflow



Le projet utilise GitHub Actions pour l'intégration et le déploiement continus. Le workflow comprend :



1. Tests automatisés

2. Construction des images Docker

3. Publication sur Docker Hub

4. Déploiement automatique



## 📦 Images Docker



Toutes les images sont disponibles sur Docker Hub :

- `votre-username/docs-django-grafana`

- `votre-username/docs-django-react`

- `votre-username/ecommerce-flask-stripe`

- `votre-username/flask-soft-ui-design`

- `votre-username/rocket-ecommerce`



## ⚙️ Configuration



La configuration de chaque application peut être personnalisée via des variables d'environnement dans le fichier `docker-compose.yml`.



## 📈 Monitoring et résilience



- L'application docs-django-grafana est déployée avec 5 replicas pour assurer la haute disponibilité

- Nginx gère la répartition de charge pour les applications

- Grafana est utilisé pour la surveillance des métriques



## 🤝 Contribution



Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou une pull request.



## 📝 License



Ce projet est sous licence MIT.

