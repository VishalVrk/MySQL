# MYSQL DEBUGGING

mysqld_safe —skip-grant-tables

MYSQL DEBUGGING

mysqld_safe —skip-grant-tables


/usr/local/bin/mysql.server stop

UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;

mysql -h localhost -u admin -p admin


ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/tmp/mysql.sock' (2)

Remove MySQL completely per 
	•	ps -ax | grep mysql
	•	stop and kill any MySQL processes
	•	brew remove mysql
	•	brew cleanup
	•	sudo rm /usr/local/mysql
	•	sudo rm -rf /usr/local/var/mysql
	•	sudo rm -rf /usr/local/mysql*
	•	sudo rm ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
	•	sudo rm -rf /Library/StartupItems/MySQLCOM
	•	sudo rm -rf /Library/PreferencePanes/My*
	•	launchctl unload -w ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
	•	edit /etc/hostconfig and remove the line MYSQLCOM=-YES-
	•	rm -rf ~/Library/PreferencePanes/My*
	•	sudo rm -rf /Library/Receipts/mysql*
	•	sudo rm -rf /Library/Receipts/MySQL*
	•	sudo rm -rf /private/var/db/receipts/*mysql*
	•	restart your computer just to ensure any MySQL processes are killed
	•	try to run mysql, it shouldn't work
