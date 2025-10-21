# Alias firewall UCVV
Alias globali per i firewall dell'Unione di Comuni Valdarno e Valdisieve, basta puntale un alias ti tipo URL (table) al file giusto e magicamente ogni variazione si propaga ad ogni PfSense.

Di default si aggiorna 1 volta al giorno, per cambiare il tempo fai un cronjob in PfSense:

*/5 	* 	* 	* 	* 	root 	/usr/bin/nice -n20 /etc/rc.update_urltables now forceupdate
