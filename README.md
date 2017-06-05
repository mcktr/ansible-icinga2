# Ansible Playbooks

#### Default Passwords

|	Username	|	Password	|	Service		 		|
|	---			|	---			|	---			 		|
| root			| sqlroot			| MariaDB root User 		|
| icinga2			| sqlicinga2		| MariaDB icinga2 User 	    	|
| icingaweb2		| sqlicingaweb2	| MariaDB icingaweb2 User	|
| icingaadmin		| icinga			| Icinga Web 2				|

You can modify the file `roles/icinga2-master/vars/main.yml` to set your own usernames and passwords. The credentials are set as a variable at every needed location. 

The credentials for the `icingadmin` user can changed by modify the file `roles/icinga2-master/templates/mariadb/icingaweb2_user.sql.j2` For more details see the [offical Icinga Web 2 documentation](https://github.com/Icinga/icingaweb2/blob/master/doc/05-Authentication.md) 