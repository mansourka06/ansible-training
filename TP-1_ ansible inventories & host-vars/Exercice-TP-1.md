# TP-1_ansible inventory

### Action réalisées :

- **Créez un cluster (1 ansible et 1 client)**

- **Créez un fichier hosts.ini au format .ini** avec les modalités d’inventaire suivant
    * Tous les hôtes via le groupe « all » devront avoir pour login user admin
    * Le client devra faire partie d’un groupe appeler « prod »
    * Le mot de passe à utiliser pour toutes connexion ssh devra être admin pour toutes les machines du groupe « prod »
    * La variable « env » devra être égale à « production » pour toutes les machines du groupe « prod »

- **Créez en suite un fichier inventory.yml, version yaml du fichier .ini**

- **Testez les commandes ad-hoc de ping et setup avec les deux fichiers d’inventaire**
