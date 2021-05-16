#Updated Ubuntu 21.04

//--- Termux

1. Update termux: $apt-get update && apt-get upgrade
2. Install wget: $apt-get install wget
3. Install proot: $apt-get install proot
4. Install git: $apt-get install git
5. Go to HOME folder: $cd ~
6. Download script: $git clone https://github.com/aanhariyanto/ubuntu-app.git
7. Go to script folder: $cd ubuntu-app
8. Give execution permission: $chmod +x ubuntu.sh
9. Run the script: $./ubuntu.sh
10. Now just start ubuntu: $./startubuntu.sh

//--- Ubuntu

apt-get update && apt-get install language-pack-en-base && apt-get install sudo && apt-get install ssh && apt-get install net-tools && apt-get install ethtool && apt-get install wireless-tools && apt-get install ifupdown && apt-get install network-manager && apt-get install iputils-ping && apt-get install rsyslog && apt-get install htop && apt-get install vim

//--- Desktop

//apt-get install xinit xorg && apt-get install alsa-utils


// LAMP SERVER UBUNTU 21.04 TERMUX

apt-get install termux-am
apt-get install termux-api
apt-get install termux-apt-repo
apt-get install termux-create-package
apt-get install termux-elf-cleaner
apt-get install termux-tools
apt-get install termux-exec

# Termux Autostart
# Create/append to:  ~/.bashrc

cd ~ && touch .bashrc && chmod +x .bashrc && nano .bashrc

if ! pgrep -f "ubuntu" >/dev/null ; then echo "" && ubuntu-app/./startubuntu.sh; else echo ""; fi

// ----------------------------------------

exit

// ----------------------------------------

echo "localhost" > /etc/hostname
echo "127.0.0.1 localhost" >> /etc/hosts

apt-get update
apt-get upgrade
apt-get install sudo
apt-get install nano
apt-get install proot

// ----------------------------------------

// install apache2 & mysql (unfinish)

// ----------------------------------------

# Ubuntu-app Autostart
# Create/append to:  ~/.bash_profile

touch .bash_profile
chmod +x .bash_profile
nano .bash_profile

if ! pgrep -f "apache2" >/dev/null ; then echo "" && /etc/init.d/apache2 start; else echo ""; fi
if ! pgrep -f "mysql" >/dev/null ; then echo "" && /etc/init.d/mysql start; else echo ""; fi

// ----------------------------------------

cat /etc/issue

// ----------------------------------------

