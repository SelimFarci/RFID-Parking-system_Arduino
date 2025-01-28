RFID-Parking System  
=========================  

Description :  
--------------  
Ce projet implémente un système de gestion de parking basé sur un Arduino, un lecteur RFID, des cartes/tags RFID, deux écrans LCD et un clavier. Le système permet d'identifier les utilisateurs et  de suivre leurs temps de stationnement et de gérer les paiements automatiquement ou manuellement.  

Fonctionnalités principales :  
-----------------------------  
1. **Entrée dans le parking :**  
   - L'utilisateur scanne sa carte/tag RFID.  
   - Si la carte est reconnue :  
     - Le système vérifie le solde de la carte.  
     - Si le solde est inférieur à 50 Rs, un rechargement de 100 Rs est demandé.  
     - Sinon, l'entrée est autorisée.  
   - Si la carte n'est pas enregistrée :  
     - La carte doit être ajoutée dans la base de données par le gestionnaire du parking.  

2. **Sortie du parking :**  
   - L'utilisateur scanne sa carte RFID ou entre un identifiant (UserID) donné par le gestionnaire à l'entrée.  
   - Le système calcule le temps de stationnement et déduit le montant du solde de la carte ou demande un paiement manuel.  

3. **Suivi des places disponibles :**  
   - Un compteur surveille le nombre de véhicules présents dans le parking.  
   - Une LED verte s'allume si des places sont disponibles. Si le parking est plein, une LED rouge s'allume.  

Matériel utilisé :  
------------------  
- Arduino  
- Lecteur RFID  
- Cartes/tags RFID    
- Deux écrans LCD  
- LEDs (verte et rouge)  
- Compteur 2 bits  

Pour plus de détails, consultez le code et les fichiers associés dans ce dépôt.  
