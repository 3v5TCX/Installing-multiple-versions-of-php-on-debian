
# default version in APT repo
sudo apt show php -a
# currently 7.3 2021

sudo apt-get update && sudo apt-get upgrade
sudo apt install php
sudo apt install software-properties-common
wget -q https://packages.sury.org/php/apt.gpg -O- | sudo apt-key add -
echo "deb https://packages.sury.org/php/ stretch main" | sudo tee /etc/apt/sources.list.d/php.list
sudo apt update
sudo apt install php5.6 
sudo apt install php7.0
sudo apt install php7.1
sudo apt install php7.2
sudo apt install php7.3
sudo apt install php7.4
sudo apt install php8.0
sudo apt install php8.1

# Magento 2 requirements
sudo apt install php7.1 php7.1-curl php7.1-mbstring php7.1-bcmath php7.1-bz2 php7.1-gd php7.1-gmp php7.1-imap php7.1-intl php7.1-ldap php7.1-opcache php7.1-mysql php7.1-pspell php7.1-recode php7.1-soap php7.1-tidy php7.1-xml php7.1-xsl php7.1-zip php7.1-common
sudo apt install php7.2 php7.2-curl php7.2-mbstring php7.2-bcmath php7.2-bz2 php7.2-gd php7.2-gmp php7.2-imap php7.2-intl php7.2-ldap php7.2-opcache php7.2-mysql php7.2-pspell php7.2-recode php7.2-soap php7.2-tidy php7.2-xml php7.2-xsl php7.2-zip php7.2-common
sudo apt install php7.3 php7.3-curl php7.3-mbstring php7.3-bcmath php7.3-bz2 php7.3-gd php7.3-gmp php7.3-imap php7.3-intl php7.3-ldap php7.3-opcache php7.3-mysql php7.3-pspell php7.3-recode php7.3-soap php7.3-tidy php7.3-xml php7.3-xsl php7.3-zip php7.3-common
sudo apt install php7.4 php7.4-curl php7.4-mbstring php7.4-bcmath php7.4-bz2 php7.4-gd php7.4-gmp php7.4-imap php7.4-intl php7.4-ldap php7.4-opcache php7.4-mysql php7.4-pspell php7.4-soap php7.4-tidy php7.4-xml php7.4-xsl php7.4-zip php7.4-common
sudo apt install php8.0 php8.0-curl php8.0-mbstring php8.0-bcmath php8.0-bz2 php8.0-gd php8.0-gmp php8.0-imap php8.0-intl php8.0-ldap php8.0-opcache php8.0-mysql php8.0-pspell php8.0-soap php8.0-tidy php8.0-xml php8.0-xsl php8.0-zip php8.0-common
sudo apt install php8.1 php8.1-curl php8.1-mbstring php8.1-bcmath php8.1-bz2 php8.1-gd php8.1-gmp php8.1-imap php8.1-intl php8.1-ldap php8.1-opcache php8.1-mysql php8.1-pspell php8.1-soap php8.1-tidy php8.1-xml php8.1-xsl php8.1-zip php8.1-common


# Updated instructions
sudo apt install -y lsb-release ca-certificates apt-transport-https software-properties-common gnupg2
echo "deb https://packages.sury.org/php/ $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/sury-php.list
wget -qO - https://packages.sury.org/php/apt.gpg | sudo apt-key add -
