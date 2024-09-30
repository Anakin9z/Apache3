# Apache3

PREMIÈRE PARTIE – MODULE MULTI-PROCESSUS (MPM) - (10 POINTS)

1. Les pages Web de ce TP devront être dans le répertoire /var/www/html_tp3
2. Placez un lien vers toutes les pages Web de ce TP dans le fichier
/var/www/html_tp3/master_tp3.html. (Vous trouverez un exemple à la dernière
page).
3. Configurez votre serveur Web pour utiliser :
➢ 12 serveurs httpd au démarrage du service;
➢ Un minimum de 6 serveurs libres en tout temps;
➢ Un maximum de 12 serveurs libres en tout temps;
➢ Un maximum de 180 requêtes de clients en même temps;
➢ Un maximum de 100 requêtes dans la liste en attente de traitement lorsque
le maximum de 180 requêtes est atteint;
➢ Les connexions persistantes avec un maximum de 50 requêtes consécutives
et un délai de latence entre 2 requêtes du même client, de 20 secondes;
➢ Un maximum de 55 secondes pour la durée d’une requête client.

DEUXIÈME PARTIE – ÉTAT DU SERVEUR APACHE - (10 POINTS)

1. En utilisant le mode ExtendedStatus
➢ Configurez le handler server-status d’Apache pour les utilisateurs du sousréseau 192.168.1.0/24.
➢ Configurez le handler server-info d’Apache pour les utilisateurs du sousréseau 192.168.1.0/24.

TROISIÈME PARTIE – SSI (10 POINTS)

1. Configurez votre serveur Web pour utiliser les SSI pour les pages dont l’extension est
« .shtml ».
➢ Écrivez une page Web /var/www/html_tp3/q3/index.shtml qui s'affiche,
lorsqu'on tape www.ssi.com dans la barre d'adresse du navigateur.
Note : Utilisez l’adresse IP : 10.35.16.1 pour www.ssi.com
➢ Cette page affiche le texte "www.ssi.com" et affiche au-bas de la page le
contenu de la page bas_page.shtml (qui est décrite au point suivant), en
utilisant les directives SSI d’inclusion.
Travail pratique #3 420-4G6-MO
3 | P a g e
➢ Écrivez une page Web bas_page.shtml qui affiche la liste détaillée de fichiers
du répertoire /var/www/html_tp3/q3/ et qui affiche en plus séparément la
taille du fichier index.shtml.

QUATRIÈME PARTIE – CGI - (10 POINTS)

1. Configurez votre serveur Web pour utiliser les cgi-bin.
2. Créez un script en Perl qui affiche du texte dans le logiciel de navigation.
3. Placez ce script dans le répertoire /var/www/cgi-bin.
   
CINQUIÈME PARTIE – PHP - (10 POINTS)

1. Configurez votre serveur Web pour utiliser PHP.
2. Créez une page Web en PHP qui affiche le message "Bonjour mon ami" à
l’utilisateur si son adresse IP est dans le sous-réseau 192.168.100.0/24 ou qui
affiche le message "Bonjour étranger" aux autres utilisateurs.
3. Placez cette page Web dans le répertoire /var/www/html_tp3/q5/.
   
SIXIÈME PARTIE – BASE DE DONNÉES (15 POINTS)

1. Installez MySQL et créez une table « employes » qui contient un nom et un salaire.
2. Insérez quelques valeurs dans la table et consultez le contenu de la table avec votre
programme.
3. Créez une page Web en PHP qui permet de se connecter à cette base de données et
d’afficher le contenu de la table employes.
4. Placez cette page Web dans le répertoire /var/www/html_tp3/q6/.
   
SEPTIÈME PARTIE – SSL (10 POINTS)

1. Configurez votre serveur Web pour utiliser SSL.
2. Testez l’accès à votre serveur en utilisant le protocole sécuritaire https.
https://serveurX (où X est le numéro de votre serveur).
HUITIÈME PARTIE – FANCY INDEXING (10 POINTS)
1. Pour le répertoire /var/www/html_tp3/q8/, faire en sorte que l'affichage des
fichiers se fasse selon le format suivant (utilisation de FancyIndexing).
Travail pratique #3 420-4G6-MO
4 | P a g e
2. Précisions:
➢ Vous devez obtenir le même affichage que dans l'exemple ci-dessus avec les
mêmes fichiers que ceux listés.
➢ Le message au début de l'index provient du fichier HEADER.html
➢ Le message à la fin provient du fichier README.html
➢ Les icônes sont disponibles dans le dossier /icones du serveur Apache.
➢ Les répertoires utilisent l'icône du globe terrestre.
➢ Les fichiers de type "texte" utilisent l'icône "bombe".
➢ Les fichiers de type image en PNG utilisent l'icône "main droite".
➢ Les fichiers de type image en GIF utilisent l'icône "explosion".
➢ Les autres fichiers utilisent l'icône "?".
➢ Les répertoires doivent se retrouver au début de l'index.
➢ Les commentaires à droite des fichiers catalogue.html et catalogue2.html
sont montrés sur l'image.
Travail pratique #3 420-4G6-MO
5 | P a g e
