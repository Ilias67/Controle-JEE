# Controle-JEE-MAMOUNY_ILIAS-G2
<h1><i>1-L'Objectif de l'Atelier:</i><h1>
<h3>Créer une application basée sur une architecture micro-service qui permet de gérer les factures contenant des produits et appartenant à un client.</h3>
<ol>
  <li>Micro-service customer-service qui permet de gérer les client</li>
  <li>Micro-service inventory-service qui permet de gérer les produits</li>
  <li>Gateway Spring cloud Gateway avec une Configuration statique du système de routage</li>
  <li>Annuaire Eureka Discrovery Service</li>
  <li>Configuration dynamique des routes de la gateway</li>
  <li>Service de facturation Billing-Service en utilisant Open Feign</li>
  <li>Client Web Angular (Clients, Produits, Factures)</li>
  <li>Déployer le serveur keycloak :</li>
  <dl>
  <dt>- Créer un Realm</dt>
  <dt>- Créer un client à sécuriser</dt>
  <dt>- Créer des utilisateurs</dt>
  <dt>- Créer des rôles</dt>
  <dt>- Affecter les rôles aux utilisateurs</dt>
  <dt>- Tester les différents modes d'authentification avec Postman en montrant les contenus de Access-Token, Refresh Token</dt>
  </dl>
  <li>Sécuriser les micro-services et le frontend angular en déployant les adaptateurs Keycloak</li>
</ol>
<h1><i>2-La simulation :</i><h1>
<img src="https://user-images.githubusercontent.com/80590096/209091463-0fe25b5b-b8fe-4331-a200-0b466f0af665.PNG"/>
<img src="https://user-images.githubusercontent.com/80590096/209091588-0c40b8de-3c4d-466c-a334-74d1cd32cd69.PNG"/>  
<img src="https://user-images.githubusercontent.com/80590096/209092073-a368fc23-1777-4570-9764-2d584f1406a3.PNG"/>  
<img src="https://user-images.githubusercontent.com/80590096/209092256-7701818a-37c5-428d-b900-c5c16539141c.PNG"/>  
<img src="https://user-images.githubusercontent.com/80590096/209092280-93dda850-784c-4f6b-af2b-8b8ae3b986f0.PNG"/>  
<img src="https://user-images.githubusercontent.com/80590096/209092313-d013f233-633a-4758-938a-3662844d8216.PNG"/> 
<img src="https://user-images.githubusercontent.com/80590096/209092704-00b1f166-702e-42b9-b37f-21565e6e81ea.PNG"/>  
<h1><i>3-Partie Front (Angular) :</i><h1>
<ul>Liste des clients</ul>
<img src="https://user-images.githubusercontent.com/80590096/209116003-cf232ef6-101b-42df-9345-24611eab3d48.PNG">
<ul>Liste des produits</ul>
<img src="https://user-images.githubusercontent.com/80590096/209116024-e72c8391-6671-494f-9279-15a4d757c45d.PNG">
<ul>Details d'une facture d'un client</ul>
<img src="https://user-images.githubusercontent.com/80590096/209116954-7f01aac1-d872-4d83-81c8-b20a14ce40eb.PNG">

<h1><i>4-Keycloak :</i><h1>
<img src="https://user-images.githubusercontent.com/80590096/219802758-19ecf45e-bf99-4815-8078-c866f422254c.PNG">

<img src="https://user-images.githubusercontent.com/80590096/219804348-7e47e649-79bb-47e9-bcaf-805f399b328a.PNG">



<img src="https://user-images.githubusercontent.com/80590096/219804715-5f9b9dd2-420b-46fd-a81f-c8903ef2c28c.PNG">

<h1 id="kafka">KAFKA</h1>
<h2 id="-tape-1-int-gration-du-bocker-kafka">Étape 1 : Intégration du Bocker KAFKA</h2>
<p>Le projet commence par l&#39;intégration de Bocker KAFKA. Kafka est une plateforme de streaming distribuée qui permet de gérer des flux de données en temps réel. Cette étape permet d&#39;installer et de configurer Kafka dans le projet.</p>
<h2 id="-tape-2-cr-ation-d-un-micro-service-de-facturation">Étape 2 : Création d&#39;un micro-service de facturation</h2>
<p>Ensuite, un micro-service de facturation a été développé. Ce service génère aléatoirement des factures et les publie dans un Topic Kafka. Ce service est responsable de la production des factures à des fins de démonstration.</p>
<h2 id="-tape-3-int-gration-du-micro-service-de-facturation-dans-billing-service">Étape 3 : Intégration du micro-service de facturation dans BILLING-SERVICE</h2>
<p>Le micro-service de facturation a été intégré dans BILLING-SERVICE. Ce service consomme les factures publiées dans le Topic Kafka et les enregistre dans sa base de données.</p>
<h2 id="-tape-4-cr-ation-d-un-micro-service-de-data-analytics">Étape 4 : Création d&#39;un micro-service de Data Analytics</h2>
<p>Un micro-service de Data Analytics a été créé pour traiter les flux de données en temps réel. Ce service utilise l&#39;API KAFKA Streams pour effectuer du Real Time Stream Processing en consommant les flux de factures publiées dans le Topic Kafka.</p>
<h2 id="-tape-5-cr-ation-d-une-page-frontend-pour-afficher-les-r-sultats">Étape 5 : Création d&#39;une page Frontend pour afficher les résultats</h2>
<p>Une page Frontend a été développée pour afficher les résultats produits par le service de Data Analytics en temps réel. Cette page présente les courbes qui montrent les résultats produits par le service du Data Analytics.</p>
<h2 id="-tape-6-d-ploiement-de-l-application-en-utilisant-docker">Étape 6 : Déploiement de l&#39;application en utilisant Docker</h2>
<p>L&#39;ensemble des services de l&#39;application ont été déployés en utilisant Docker. Des images Docker ont été créées pour chaque service et un fichier Docker-compose.yml a été mis en place pour déployer l&#39;ensemble de l&#39;application.</p>
<h2 id="s-curisation-des-micro-services-et-du-frontend-avec-les-adaptateurs-keycloak">Sécurisation des micro-services et du frontend avec les adaptateurs Keycloak</h2>
<p>Pour renforcer la sécurité des micro-services et du frontend Angular, des adaptateurs Keycloak ont été déployés. Keycloak est une plateforme open source d&#39;authentification et d&#39;autorisation, qui permet de protéger les applications contre les attaques.</p>
<p>Les adaptateurs Keycloak ont été intégrés à l&#39;ensemble des micro-services de l&#39;application. Ils permettent de sécuriser l&#39;accès aux données en mettant en place une authentification et une autorisation renforcée.</p>
<h2 id="conclusion">Conclusion</h2>
<p>En conclusion, ce projet a sécurisé avec succès les micro-services et le frontend Angular en déployant les adaptateurs Keycloak. En intégrant Keycloak, une plateforme d&#39;authentification et d&#39;autorisation open source, nous avons pu protéger l&#39;application contre les attaques et garantir que les données sont sécurisées.</p>
<p>Au cours des différentes étapes du projet, nous avons intégré Kafka, créé un micro-service pour générer des factures aléatoires, intégré ce service à BILLING-SERVICE, créé un service d&#39;analyse de données à l&#39;aide de Kafka streams, développé une page frontend pour afficher les résultats en temps réel produits par le service d&#39;analyse de données. Enfin, nous avons déployé tous les services à l&#39;aide de Docker et les avons sécurisés avec Keycloak.</p>
<p>Dans l&#39;ensemble, ce projet a démontré l&#39;importance de sécuriser les micro-services et le frontend d&#39;une application, en particulier dans les scénarios où des données sensibles sont impliquées. Le déploiement réussi des adaptateurs Keycloak dans ce projet est une manière efficace de garantir que les données restent sécurisées et que l&#39;accès non autorisé est empêché.</p>


