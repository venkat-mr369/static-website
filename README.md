# static-website, Copy this in startup-script section

#!/bin/bash
sudo apt update -y
sudo apt install apache2 git -y
sudo git clone https://github.com/venkat-mr369/static-website.git
sudo rm -rf /var/www/html/index.html
sudo cp -r static-website/* /var/www/html/
