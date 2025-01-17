# Exercice 2 : Manipulations pratiques sur VM Linux  
  
## Partie 1 : Gestion des utilisateurs  

**Q.2.1.1**  
  
![image](https://github.com/user-attachments/assets/d5c22687-3064-4d0b-9f3b-f1759d20ccde)  
  
----  
**Q.2.1.2**  
  
Créer un espace personnel de travail, lui configurer un mot de passe dès la création  
  
----
  
**Q.2.2.1**  
  
➡️ Éditer le fichier suivant avec la commande : `nano /etc/ssh/sshd_config`  
  
➡️ Décommenter la ligne "PermitRootLogin" et la modifier en `PermitRootLogin no`  
  
![image](https://github.com/user-attachments/assets/abf9729d-299c-4c4d-afb0-9d0efc474672)  
  
➡️ Redémarrer le service SSH avec la commande `service ssh restart`  
  
----  
  
**Q.2.2.2**  
  
A la fin du fichier **/etc/ssh/sshd_config**, ajouter une ligne `AllowUsers checkpoint`  
  
![image](https://github.com/user-attachments/assets/1e686693-6f7d-4614-bc42-8a4e31d05806)  
  
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

