Servers Info
----------------------------------------------------------------------------------------------------
Ip address: 13.233.62.155
SSH port: 2200
complete URL: http://13.233.62.155.xip.io

Installed software and configuration changes
----------------------------------------------------------------------------------------------------
1. install finger.
	* created a user called grader.
	* made grader into a sudoer.
2. fire wall changes.
	* block all incoming requests from all posts except:
		1. port 80 (www).
		2. port 2200 (for ssh).
		3  port 123 (NAT).
	* allow all outgoing requests from all posts.
3. reconfigured the time zone to be Riyadh (+3) through sudo dpkg-reconfigure tzdata.
4. clone github repositories "[item-catalog-project](https://github.com/FarisALSaleem/item-catalog-project)" to /var/www/
5. install python3-pip.
	* install sqlalchemy.
	* install flask.
	* install oauth2client.
	* install requests.
	* install httplib2.
	* install psycopg2.
	* install psycopy2-binary.
6. install apache2.
	* a2dissite 000-default.conf
	* created flask.conf
	* a2ensite flask.conf
7. install postgresql.
	* created a user and a db called grader.
8. install libapache2-mod-wsgi-py3.

Third-party Resources
----------------------------------------------------------------------------------------------------
"[How to deploying python flask on apache2 ubuntu 16.04](https://www.youtube.com/watch?v=wq0saslschw)" by Python Web Turorial on Youtube






