Mehdi Meguenani										                                                                                                                              3ICS


Compte Rendu TP1

# Exercice 2. Prise en main de l’interpréteur de commandes
### Manuel : 
1. La commande which permet de trouver le chemin des commandes éxécutable. En faisant la commande « which  ls » j’obtiens le chemin d’accès de la commande ls qui est « usr/bin/ls »
2. Afin de rechercher un terme quand on consulte une page du manuel il faut faire «/nomduterme » par exemple pour on cherche le terme optios il faut faire « /options »
3. Afin de de sortir du manuel il faut écrire « q » puis taper sur entrée 
4. La section 6 décrit les les jeux et d’autre programme amusant disponible 
### Navigation dans l’arborescence des fichiers : 
1.	Afin d’accèder au dossier var/log il faut effectuer la commande « cd var/log »
2.	Pour remonter au dossier parent il faut utiliser la commande cd /var
3.	Pour retourner au dossier personnel il faut faire « cd $Home » ou bien juste « cd »
4.	Afin de revenir au dossier précédent il faut faire « cd -»
5.	Il n’est pas possible de faire le « cd /root » nous n’avons pas la permission
6. La commande initial « sudo cd /root » n’est pas autorisé il faut donc dans un premier temps effectué « sudo su » afin de pouvoir utilisé « sudo »
8. A l’aide de la commande rm le Fichier 1 peut être supprimé sans soucis au contraire du Dossier 1 la commande ne fonctionne pas car c’est un dossier 
9. La commande qui permet de supprimer un dossier est « Rmdir »
10. La commande « Rmdir » ne peut pas être effectué car le dossier n’est pas vide 
11. Afin de supprimer en une seul commande le dossier 2 il faut faire « rm – r »
### Commandes importantes : 
1.	La commande qui permet d’afficher la date est « date » . La commande time permet de voir le temps d’exécution d’une commande.
2.	La commande « ls » permet d’afficher une partie des fichier et dossier. Alors que la commande « la » affiche tous les dossier et fichier même ceux caché. Les fichiers avec des point sont des fichiers cachés
3.	Le programme ls se situe « usr/bin/ls »
4.	Il n’existe pas d’entré manuel pour ll. La commande « ll » est un raccourci de la commande ls –alF. La commande allias permet donc d’afficher le raccourci de la commande 
5.	La commande qui permet d’afficher le contenu dossier bin est « ls /bin »
6.	La commande « ls .. » permet de voir le contenu du dossier précédent 
7.	 La commande qui permet d’afficher le chemin complet est « pwd » 
8.	La commande « echo 'bip' > plop  » permet de créer un fichier. Quand elle est exécuté deux fois elle écrase le fichier précédent du même nom 
9.	La commabde « echo 'bip' > > plop » permet d’ajouter du contenu au fichier plop 
10.	 La commande sleep 10 | echo 'toto' permet de mettre un temp d’éxécution a la commande echo 
11.	 Grace a la  commande « file » on identifie le type du fichier 
12.	 On observe que le lien_phy est mis à jour. Le contenu est gardé même quand le fichier original est supprimé 
13.	 Le fichier lien_sym se met a jour comme pour la commande précédente. Par contre une fois le fichier lien_phy supprimer alors les le lien_smy est aussi supprimer 
14.	 Le raccourci qui permet cela est Ctrl + S
15.	 La commande pour afficher  les 15 derniere ligne du fichier est « tail –n15 /var/log/syslog »
16.	 
17.	 Le fichier passwd permet stocke les informations de connexion au système et les utilisateurs 
18.	  
19.	 La commande qui permet d’afficher les utilisateurs est wc –l /etc/passwd
20.	 
21.  Pour trouver tous les fichier ayant pour nom passw il faut effectuer la commande " find / -iname "passwd" " 
22.  Afin d'enregistré les fichiers trouvé dans un fichier précis il faut faire " find / -iname "passwd" >> list_passwd_files.txt ". Pour redirifer les erreurs la commande est " find / -iname "passwd" 2>> /dev/null " 
23.  
24. Le fichier history.log se trouvre dans " /var/log/apt/history.log "
25. La commande locate recherhce les fichiers dans une base de donnée, le fichier tout juste créer n'est pas encore prénsent dans la BD il faut donc l'actualiser a l'aide de la commande "updatedb".
# Exercice 3. Découverte de l’éditeur de texte nano
1. Afin de copier le fihcier il faut faire " cp /var/log/syslog log.txt " puis nano log.txt pour afficher 
2. Afin de remplacer le mot kernel il faut faire  Alt Gr + 8 
3. On peut se situer au début du fichier avec "Ctrl + Fleche du haut" ensuite Ctrl + K pour couper le fichier. On se met a la fin du fichier avec Ctrl + Fleche du bas puis on colle avec Ctrl + U 
4. Pour annuler l'action il faut faire Alt + U 
5. Pour sauvegarder Ctrl + X puis Y 
# Exercice 4. Personnalisation du shell

