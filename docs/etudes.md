---
layout: default
nav_order: 4
title: Études et choix techniques
---

## Études et Choix Techniques

Dans le cadre du développement de Co'b, plusieurs choix techniques ont été réalisés afin de garantir une intégration optimale des différentes technologies et une performance maximale du dispositif. Voici un aperçu des principales décisions technologiques :

### Infrastructure et Gestion des Contextes

1. **Docker et Portainer :**
   - **Rationale :** Pour faciliter la gestion des conteneurs et déployer facilement nos services, nous avons opté pour Docker, accompagné de Portainer pour une interface de gestion intuitive. Cette solution nous permet de maintenir une architecture modulaire et scalable.
   - **Avantages :** Isolation des services, facilité de déploiement, gestion simplifiée des mises à jour et des versions.

2. **Orion Context Broker :**
   - **Rationale :** Nous utilisons Orion Context Broker pour une gestion avancée des contextes en temps réel. Il nous permet de collecter, gérer et fournir des données contextuelles à partir de divers capteurs et dispositifs connectés.
   - **Avantages :** Flexibilité, temps réel, interopérabilité avec d'autres composants FIWARE.

### Intégration des Capteurs

3. **IoT Agents :**
   - **Rationale :** Pour une meilleure intégration des différentes technologies de capteurs, nous avons intégré des IoT Agents. Ceux-ci facilitent la communication entre les capteurs et Orion Context Broker en traduisant les protocoles spécifiques des capteurs en formats compatibles avec FIWARE.
   - **Avantages :** Compatibilité accrue, facilité d'intégration, gestion unifiée des capteurs.

### Analyse Temporelle et Traitement de Données

4. **QuantumLeap et CrateDB :**
   - **Rationale :** Pour effectuer une analyse temporelle approfondie des données, nous avons choisi QuantumLeap en combinaison avec CrateDB. QuantumLeap permet de transformer les données contextuelles en séries temporelles, tandis que CrateDB offre une base de données adaptée au stockage et à l'analyse des séries temporelles.
   - **Avantages :** Performance, scalabilité, efficacité dans le traitement des séries temporelles.

5. **Cygnus :**
   - **Rationale :** Pour la gestion des flux de données entre les différents composants FIWARE et les bases de données externes, nous avons intégré Cygnus. Cygnus facilite le transfert des données collectées vers divers systèmes de stockage et de traitement.
   - **Avantages :** Interopérabilité, gestion efficace des flux de données, compatibilité avec divers systèmes de stockage.

### Protocole de Communication

6. **Protocole MQTT :**
   - **Rationale :** Pour la communication entre le Raspberry Pi 3 et les IoT Agents, nous utilisons le protocole MQTT (Message Queuing Telemetry Transport). MQTT est un protocole de messagerie léger conçu pour les connexions de machine à machine (M2M) et les environnements de l'Internet des objets (IoT).
   - **Avantages :** Faible bande passante, fiabilité, efficacité dans les environnements à faible latence, compatibilité avec les capteurs IoT.

### Choix Matériels

7. **Raspberry Pi 3 :**
   - **Rationale :** Nous avons choisi le Raspberry Pi 3 plutôt qu'une carte Pycom pour notre projet. Le Raspberry Pi 3 offre une puissance de calcul suffisante, une large communauté de support, et une compatibilité avec divers modules et capteurs.
   - **Avantages :** Coût abordable, flexibilité, large support communautaire, facilité d'intégration.

8. **Capteur de Distance :**
   - **Rationale :** Pour détecter le passage du ballon dans l'arceau, nous utilisons un capteur de distance. Ce capteur permet de mesurer avec précision la distance entre le ballon et le panier, fournissant des données essentielles pour l'analyse des tirs.
   - **Avantages :** Précision, fiabilité, facilité d'intégration avec le Raspberry Pi.

### Conclusion

Les choix techniques réalisés pour le projet Co'b visent à assurer une intégration fluide et une performance optimale du système. En combinant des technologies avancées de gestion des contextes, d'intégration des capteurs, d'analyse temporelle et de traitement des flux de données, nous avons construit une solution robuste et évolutive pour l'entraînement au basketball. L'utilisation du Raspberry Pi 3 et des capteurs de distance garantit une solution matérielle efficace et abordable, adaptée aux besoins de notre projet.
