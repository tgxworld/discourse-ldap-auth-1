# Discourse ldap auth
* This plugin is used for authentication with active directory.
* This is working version and work with my corporate network.


## Why do I specify a binding DN and password in settings
The above requirement is as omniauth-ldap does a search for DN for the username(or email) provided in login form.
If your AD allows anonymous search then we dont need these settings. But most AD nowadays donot allow that.
Hence in pluin settings, we have to specify distinguished name and password.

##FUTURE
See if ldap search can be handle without prioving a binding dn and password. 
Usually DN can be derived from email/username. We should ideally form credentials for both ldap search and bind.

