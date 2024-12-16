# Les logs
## Composants pour l'exercice
- Un serveur Debian 12 (192.168.1.85)
- Un client Mint 22 (192.168.1.180) avec navigateur Firefox
- Un client Windows 10 (192.168.1.202) avec navigateur Chrome

## Installation d'un serveur nginx
1. Installer le paquet nginx  
   `apt install nginx -y`  
2. Vérifier la version installé  
   `nginx -v`  
3. Controler l'état du service  
   `systemctl status nginx.service`  
4. Activer le service  
   `systemctl enable nginx.service`  

## Génération de logs
1. Accéder au site depuis la machine client avec Firefox  
   `http://192.168.1.85`  
2. Accéder au site depuis la machine client avec Chrome  
   `http://192.168.1.85`  

## Controler les logs
1. Access.log

![image](https://github.com/user-attachments/assets/e885e0fa-21e5-41a2-b463-754d2754ff3e)  
Sur l'image ci-dessus, l'on observe les logs générés par la connection `192.168.1.180` depuis le navigateur `Firefox 133.0` via un system `Linux`  

![image](https://github.com/user-attachments/assets/19bbf47d-1a6b-4b53-8677-b1ed2217e35e)  
Sur l'image ci-dessus, l'on observe les logs générés par la connection `192.168.1.202` depuis le navigateur `Chrome 129.0` via un system `Windows`  
