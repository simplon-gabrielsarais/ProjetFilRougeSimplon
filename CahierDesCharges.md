# Cahier des charges - Déploiement de n8n, Rocket.Chat, Prometheus et Grafana sur AKS avec scaling horizontal

## Contexte
L'objectif de ce projet est de déployer les applications n8n, Rocket.Chat, Prometheus et Grafana dans une infrastructure Kubernetes sur Azure Kubernetes Service (AKS) en utilisant le scaling horizontal. L'objectif final est de mettre en place un système de notification dans Rocket.Chat à l'aide de n8n. Prometheus et Grafana seront également installés pour offrir une supervision de l'infrastructure.

## Objectifs
Les objectifs spécifiques de ce projet sont les suivants:
1. Déployer une infrastructure Kubernetes sur AKS.
2. Déployer n8n sur l'infrastructure Kubernetes pour automatiser les workflows et les notifications.
3. Déployer Rocket.Chat sur l'infrastructure Kubernetes pour fournir une plateforme de communication.
4. Configurer n8n pour envoyer des notifications vers Rocket.Chat.
5. Installer Prometheus pour collecter les métriques.
6. Configurer Grafana pour afficher des tableaux de bord avec les métriques.
7. Mettre en place le scaling horizontal pour les services n8n, Rocket.Chat.

## Spécifications techniques
1. L'infrastructure Kubernetes sera déployée sur Azure Kubernetes Service (AKS).
2. Le déploiement des applications sera réalisé en utilisant des manifestes Kubernetes (fichiers YAML).
3. Les services n8n et Rocket.Chat seront déployés en utilisant des déploiements Kubernetes.
4. Les pods des déploiements seront configurés pour fonctionner avec un nombre de répliques initial et une politique de scaling horizontal.
5. n8n sera configuré pour envoyer des notifications vers Rocket.Chat en utilisant les webhooks.
6. Prometheus sera installé pour collecter les métriques de base des services et des pods.
7. Grafana sera installé pour afficher des tableaux de bord basiques avec les métriques collectées par Prometheus.

## Livrables
Les livrables attendus pour ce projet sont les suivants:
1. Les manifestes Kubernetes pour le déploiement de l'infrastructure et des applications.
2. Les configurations de n8n pour les workflows et les notifications vers Rocket.Chat.
3. Un rapport de déploiement décrivant les étapes de déploiement, les configurations réalisées et les résultats obtenus.

## Contraintes
Les contraintes suivantes doivent être prises en compte dans ce projet:
1. Utilisation d'Azure Kubernetes Service (AKS) comme plateforme de déploiement.
2. Respecter les bonnes pratiques de sécurité pour les déploiements Kubernetes.
3. Assurer la haute disponibilité et la résilience des applications déployées.
4. Configurer les ressources de manière optimale pour permettre le scaling horizontal efficace.
5. Documenter les procédures d'installation, de configuration et de maintenance des applications.

## Échéancier
L'échéancier prévisionnel pour ce projet est le suivant:
1. Phase de planification et de conception: 1 semaine.
2. Phase de déploiement initial de l'infrastructure Kubernetes: 1 semaine.
3. Phase de déploiement des applications n8n, Rocket.Chat: 2 semaines.
4. Phase de configuration et de tests des intégrations entre n8n et Rocket.Chat: 1 semaine.
5. Phase de documentation et de rédaction du rapport de déploiement: 1 semaine.

Veuillez noter que l'échéancier peut être sujet à des ajustements en fonction des contraintes et des imprévus rencontrés tout au long du projet.
