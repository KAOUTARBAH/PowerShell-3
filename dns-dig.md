# Requêter DNS avec dig

Utilise la commande dig pour récupérer les informations suivantes :

- les adresses IP version 4 du site web de la Wild Code School ! www.wildcodeschool.com
***dig www.wildcodeschool.com A***
***dig www.wildcodeschool.com***
![adresses IP 4](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/adresseip4.png)

- les adresses IP version 6 d'odyssey et en déduire l'hébergeur de ton fournisseur de quête préféré
**Toutes les adresses IPv6 d'odyssey.wildcodeschool.com ont été trouvées**
***dig odyssey.wildcodeschool.com AAAA***
![adresses IP 6](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/adresseip6.png)

**l'hébergeur de ton fournisseur de quête préféré**
***whois <adresse_IP>***
![whois](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/whois.png)

- (Bonus) les noms des serveurs de noms faisant autorité sur le domaine wildcodeschool.com et le serveur primaire.
***dig wildcodeschool.com NS***
![nom serveurs](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/domaine.png)

**le serveur primaire.**
***dig wildcodeschool.com NS +short***
![serveur primaire](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/domaineP.png)

- (Bonus) Refaire les requêtes précédentes en précisant l'utilisation du serveur récursif quad9 (9.9.9.9 ou 2620:fe::9)

***dig @9.9.9.9 www.wildcodeschool.com A***
![serveur récursif ip4](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/dns9.png)

***dig @9.9.9.9 odyssey.wildcodeschool.com AAAA***
![serveur récursif ip6](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/dns6.png)

***dig @9.9.9.9 wildcodeschool.com NS***
![serveur récursif nom serveur](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/dnsns.png)

***dig @9.9.9.9 wildcodeschool.com NS +short***
![serveur récursif nom serveur](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imageDig/dnsnssh.png)
