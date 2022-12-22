# Activite-Pratique-du-Controle
<h1><i>1-Objectif de l'Atelier:</i><h1>
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
<h1><i>2-Architecture de l'atelier :</i><h1>
<img src="https://user-images.githubusercontent.com/48455549/206859150-63e5c806-86a2-4937-8791-9a7ce2464316.PNG">
<h1><i>3-La simulation :</i><h1>
<img src="https://user-images.githubusercontent.com/80590096/209091463-0fe25b5b-b8fe-4331-a200-0b466f0af665.PNG"/>
 <img src="(https://user-images.githubusercontent.com/80590096/209091588-0c40b8de-3c4d-466c-a334-74d1cd32cd69.PNG"/>  
<img src="https://user-images.githubusercontent.com/80590096/209092073-a368fc23-1777-4570-9764-2d584f1406a3.PNG"/>  
<img src="https://user-images.githubusercontent.com/80590096/209092256-7701818a-37c5-428d-b900-c5c16539141c.PNG"/>  
<img src="https://user-images.githubusercontent.com/80590096/209092280-93dda850-784c-4f6b-af2b-8b8ae3b986f0.PNG"/>  
<img src="(https://user-images.githubusercontent.com/80590096/209092313-d013f233-633a-4758-938a-3662844d8216.PNG"/> 
<img src="https://user-images.githubusercontent.com/80590096/209092704-00b1f166-702e-42b9-b37f-21565e6e81ea.PNG"/>  
<h1><i>4-Partie Front (Angular) :</i><h1>
<ul>Liste des produits</ul>
<img src="https://user-images.githubusercontent.com/74361043/207729026-68fa772c-384a-4246-bdb4-5f1573f86feb.png">
<ul>Liste des clients</ul>
<img src="https://user-images.githubusercontent.com/74361043/207729271-aa8da8c7-f7a3-4bd0-9817-348e9a474264.png">
<ul>Liste des factures d'un client</ul>
<img src="https://user-images.githubusercontent.com/74361043/207729424-62d6c16f-f472-4761-b8a3-f1ca9b540eb6.png">
<ul>Details d'une facture d'un client</ul>
<img src="https://user-images.githubusercontent.com/74361043/207732271-9d842f44-6c78-4f27-bfe6-716928e6966e.png">
  
  
 
