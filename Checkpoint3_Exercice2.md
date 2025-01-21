# Exercice 2 : Manipulations pratiques sur VM Linux  
  
## Partie 1 : Gestion des utilisateurs  

**Q.2.1.1**  
  
![image](https://github.com/user-attachments/assets/d5c22687-3064-4d0b-9f3b-f1759d20ccde)  
  
----  
**Q.2.1.2**  
  
Créer un espace personnel de travail, lui configurer un mot de passe robuste dès la création  
  
----
## Partie 2 : Configuration de SSH    
  
**Q.2.2.1**  
  
➡️ Éditer le fichier suivant avec la commande : `nano /etc/ssh/sshd_config`  
  
➡️ Décommenter la ligne "PermitRootLogin" et la modifier en `PermitRootLogin no`  
  
![image](https://github.com/user-attachments/assets/abf9729d-299c-4c4d-afb0-9d0efc474672)  
  
➡️ Redémarrer le service SSH avec la commande `systemctl restart sshd`  
  
----  
  
**Q.2.2.2**  
  
A la fin du fichier **/etc/ssh/sshd_config**, ajouter une ligne `AllowUsers checkpoint`  
  
![image](https://github.com/user-attachments/assets/1e686693-6f7d-4614-bc42-8a4e31d05806)  
  
**Q.2.2.3**  
  
Création de clé avec la commande `ssh-keygen -t ecdsa`  
  
![image](https://github.com/user-attachments/assets/3204e065-cee8-4962-bffc-1649afca6ea1)  
  
![image](https://github.com/user-attachments/assets/4022f342-fafb-44ca-81ce-c4035d26aec6)
  
Envoi de la clé crée sur la machine serveur :  
  
➡️ Création du dossier `.ssh` et du fichier `authorized_keys` sur le serveur :  
  
![image](https://github.com/user-attachments/assets/5c6264fb-9b64-40ab-9287-3b80013f892c)  
  
➡️ Après la commande `nano`, on aura à coller dans le fichier `authorized_keys` la clé ssh préalablement créée et copiée  
  
![image](https://github.com/user-attachments/assets/b7d63821-4202-4a60-b6b2-cab3b4ac7015)
  
-----  
## Partie 3 : Analyse du stockage  
  
**Q.2.3.1**  
  
![image](https://github.com/user-attachments/assets/10a035b9-baa4-4f25-bf98-d81194544395)  
  
**Q.2.3.2**  
  
Les types de systèmes de stockage utilisés sont RAID et LVM  
  
**Q.2.3.3**  
  
![image](https://github.com/user-attachments/assets/82403429-5060-4b58-98f4-2c20cb524abe)  
  
![image](https://github.com/user-attachments/assets/6ed26926-d7cc-4bb5-aeb3-20dab777e9e7)




  


----
  
## Partie 4 : Sauvegardes  
  
**Q.2.4.1**  
  
- `bareos-dir` : Planifie et supervise toutes les opérations de sauvegarde, de restauration, de vérification et d'archivage.  
  
- `bareos-sd` : Chargé, à la demande du directeur Bareos, d'accepter les données d'un daemon de fichiers Bareos et de stocker les attributs et les données des fichiers sur les supports ou volumes de sauvegarde physique.  
  
- `bareos-fd` : À la demande du directeur Bareos, il recherche les fichiers à sauvegarder et envoie leurs données au daemon de stockage Bareos.  
  
----
  
## Partie 5 : Filtrage et analyse réseau  
  
**Q.2.5.1**  
  
Les règles actuellement appliquées sur Netfilter sont les suivantes :  
  
![image](https://github.com/user-attachments/assets/74822015-fdb9-41a4-bd51-79734ebf10e5)

