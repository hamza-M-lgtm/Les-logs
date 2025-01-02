# Les-logs
 configurations des logs d'un serveur web Apache 2 installé sur une machine virtuelle Linux.

## Installation et Configuration

### Apache 2
Pour installer Apache 2 sur une machine Linux :

1. sudo apt update
2.  sudo apt install apache2

3.  ![apache2](https://github.com/user-attachments/assets/7a6c1540-c0cb-48ef-95bb-09f10fd5b532)

une fois l'installation est finie et 
pour acceder a la configure de logging pour enregistrer les accès et les erreurs 
et pour cela il faux tapper :
<br>
 **cat /var/log/apache2/access.log**  
 
![log 1](https://github.com/user-attachments/assets/d1476db9-0f9a-4e07-a281-7fb7226a6033)

et pour l'analyse les logs générés et identifier :
<br>
Les requêtes réussies (code 200) => cat access.log | grep 200
<br>
Les erreurs 404 (page non trouvée) => cat access.log | grep 404
<br>
Les adresses IP les plus fréquentes
<br>
![cat](https://github.com/user-attachments/assets/58923841-5d8b-4c72-8f65-543393d2983d)
