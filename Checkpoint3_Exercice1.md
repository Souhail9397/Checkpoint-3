# Exercice 1 : Manipulations pratiques sur VM Windows  
  
## Partie 1 : Gestion des utilisateurs  
  
**Q.1.1.1**  
  
➡️ Ouvrir `Active Directory Users and Computers`  
  
➡️ Dérouler l'OU `DirectionDesRessourcesHumaines`, on y trouve Kelly Rhameur  
  
➡️ Clic droit sur `Kelly.Rhameur` puis `Copy`  
  
➡️ Entrer les informations du nouvel utilisateur Lionel Lemarchand :  
  
![image](https://github.com/user-attachments/assets/72ef9b47-61f6-4fb0-a5ba-2162f1874960) ![image](https://github.com/user-attachments/assets/ec8f9423-8359-4712-9b87-84028ee4474a)  
  
----
**Q.1.1.2**  
  
➡️ Clic droit sur `Kelly.Rhameur` puis sur `Disable Account` pour le désactiver  
  
![image](https://github.com/user-attachments/assets/44f86264-11fb-4864-ae03-03f576037453)  
  
➡️ Nommer l'OU `DesactivatedUsers`  
  
➡️ Clic droit sur `Kelly.Rhameur` puis sur `Move..`  
  
➡️ Naviguer jusqu'à l'OU créée et y déplacer l'utilisateur Kelly.Rhameur  
  
![image](https://github.com/user-attachments/assets/1eabe648-0505-4917-8d29-4fc2f8382943)  
  
----
**Q.1.1.3**  
  
➡️ Dans l'OU `DirectionDesRessourcesHumaines`, faire un clic droit sur `GrpUsersDirectionDesRessourcesHumaines`, cliquer sur `Properties` puis se rendre dans l'onglet `Members`  
  
![image](https://github.com/user-attachments/assets/54141635-849b-431b-acc8-4d7e943d9c40)  
  
➡️ Cliquer sur `Remove`  
  
----
**Q.1.1.4**  
  
➡️ Ouvrir l'**Explorateur de Fichiers** et se rendre dans `DossiersIndividuels (F:)`  
  
➡️ Créer un nouveau dossier "lionel.lemarchand" et renommer le dossier de kelly.rhameur en "kelly.rhameur-ARCHIVE"  
  
![image](https://github.com/user-attachments/assets/6f89659a-2249-4cb2-9e5a-782632745b7a)  
  
----
## Partie 2 : Restriction utilisateurs  
  
**Q.1.2.1**  
  
➡️ Active Directory Users and Computers -> LabUsers -> DirectionFinancière -> Finance  
  
➡️ Clic droit sur `Gabriel.Guhl`, cliquer sur `Properties`, aller dans l'onglet `Account` et cliquer sur `Logon Hours`  
  
➡️ Cocher `Logon Denied` dans un premier temps  
  
➡️ Séléctionner la plage du Lundi au Vendredi de 7h00 à 17h00  
  
➡️ Cocher `Logon Permitted`  
  
![image](https://github.com/user-attachments/assets/b7f55a26-1dfa-428a-9abb-cee1da3343c5)  
  
---  
**Q.1.2.2**  
  
➡️ Clic droit sur `Gabriel.Guhl`, cliquer sur `Properties`, aller dans l'onglet `Account` et cliquer sur `Log On To...`  
  
➡️ Dans la fenêtre qui s'ouvre, cocher `The following computers` et dans la case `Computer name:`, entrer "CLIENT01", puis cliquer sur `Add`  
  
![image](https://github.com/user-attachments/assets/890a4b5e-c49f-43cb-b2ee-6ebf652e8289)  
  
----  
**Q.1.2.3**  
  
➡️ Dans Server Manager, cliquer sur `Tools` puis sur `Group Policy Management`  
  
![image](https://github.com/user-attachments/assets/6525b62e-a519-49e4-b0f6-30c08da16904)  
  
➡️ Donner un nom à la GPO, par exemple "Mot de passe"  
  
➡️ Clic droit sur la GPO créée, cliquer sur `Edit`  
  
Naviguer jusqu'à la GPO comme dans la capture d'écran ci-dessous, et configurer les paramètres de sécurité de mot de passe  
  
![image](https://github.com/user-attachments/assets/29babe96-9680-4a41-b21b-be5391d4b781)  
  
💾 Pour être certain que la GPO créée soit enregistrée et appliquée, on peut ouvrir un PowerShell et taper la commande suivante :   
`gpupdate /force`  
  
----  
## Partie 3 : Lecteurs réseaux  
  
**Q.1.3.1**  
  
![image](https://github.com/user-attachments/assets/2f2b6446-9ba2-4d9f-a515-ed6bb759fd31)  
  
Montage des lecteurs E: et F:  
  
![image](https://github.com/user-attachments/assets/4c7edfad-8e9f-456a-a84e-f06a877f522d) ![image](https://github.com/user-attachments/assets/1d6abf4b-8b5a-417b-8fb4-619bc7c7fda4)  
  
![image](https://github.com/user-attachments/assets/462bab04-8655-4c52-90ce-3de06ed494eb)







  

  











  





