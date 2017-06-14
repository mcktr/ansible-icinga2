# Ansible Playbooks

#### Default Passwords

|	Username	|	Password	|	Service		 		|
|	---			|	---			|	---			 		|
| root			| sqlroot			| MariaDB root User 		|
| icinga2			| sqlicinga2		| MariaDB icinga2 User 	    	|
| icingaweb2		| sqlicingaweb2	| MariaDB icingaweb2 User	|
| icingaadmin		| icinga			| Icinga Web 2				|

You can modify the file `roles/shared-variables/defaults/main.yml` to set your own usernames and passwords. The credentails are set as a variable at every needed location while deployment.

The credentials for the `icingadmin` user can changed by modifing the file `roles/icingaweb2/templates/icingaweb2_user.sql.j2` For more details see the [offical Icinga Web 2 documentation](https://github.com/Icinga/icingaweb2/blob/master/doc/05-Authentication.md) 