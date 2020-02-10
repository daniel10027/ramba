```
sudo apt install ***********************
affiche :

E: Could not get lock /var/lib/dpkg/lock-frontend - open (11: Resource temporarily unavailable)  
E: Unable to acquire the dpkg frontend lock (/var/lib/dpkg/lock-frontend),   
 is another process using it?
sudo killall apt apt-get

Solution:

sudo rm /var/lib/apt/lists/lock
sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock*
sudo dpkg --configure -a

and

sudo apt update
```

```
Tuer un procesus kibana s'il a étéb ajouté depuis le path
faire : ps -ef | grep '.*node/bin/node.*src/cli'   #une ligne est retournée avec 6 chiffre au debut 
faire : kill -9 les 6 chiffre # exemple kill -9 124578
```
