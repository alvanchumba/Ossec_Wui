📁 Installation Instructions

    Clone this repository into your web server directory:

git clone git@github.com:alvanchumba/Ossec_Wui.git /var/www/html/ossec

Install required packages (if not already installed):

sudo apt update
sudo apt install apache2 php php-cli unzip -y

Ensure OSSEC is installed and running on your server.

Set the correct permissions for the web directory:

sudo chown -R www-data:www-data /var/www/html/ossec
sudo chmod -R 755 /var/www/html/ossec

Configure OSSEC Web UI:

    Open the ossec_conf.php file:

    nano /var/www/html/ossec/ossec_conf.php

    Update log file paths and other settings to match your OSSEC installation.

Enable the site in Apache (if using Apache):

sudo a2enmod php
sudo systemctl restart apache2

Access the web interface:
Open your browser and navigate to:

http://<your-server-ip>/ossec
