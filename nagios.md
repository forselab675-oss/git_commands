# NAGIOS COMMANDS

```bash
sudo apt update

sudo apt upgrade -y

sudo apt install -y autoconf gcc libc6 make wget unzip apache2 php libapache2-mod-php libgd-dev libssl-dev

sudo systemctl start apache2

sudo systemctl enable apache2

sudo systemctl status apache2

sudo systemctl start nagios

sudo systemctl enable nagios

sudo systemctl status nagios

sudo systemctl restart nagios

sudo systemctl stop nagios

sudo /usr/local/nagios/bin/nagios -v /usr/local/nagios/etc/nagios.cfg

sudo systemctl restart apache2

sudo systemctl restart nagios
```

**Access Nagios Web Interface:**

```text
http://localhost/nagios
```

**Check services:**

```bash
systemctl status nagios
systemctl status apache2
```

**View configuration:**

```bash
sudo nano /usr/local/nagios/etc/nagios.cfg
sudo nano /usr/local/nagios/etc/objects/localhost.cfg
```

**View logs:**

```bash
sudo tail -f /usr/local/nagios/var/nagios.log
```
