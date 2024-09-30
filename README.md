# int-gration-continue

ThomasB / MaxenceP / AstinL

Pré-requis :
  Installer Vagrant


La création de certificat n'est pas automatisée :
```
sudo mkdir -p /etc/gitlab/ssl
```
sudo openssl req -newkey rsa:2048 -nodes -keyout /etc/gitlab/ssl/gitlab.debian.vm.key -x509 -days 365 -out /etc/gitlab/ssl/gitlab.debian.vm.crt

sudo nano /etc/gitlab/gitlab.rb

nginx['ssl_certificate'] = "/etc/gitlab/ssl/gitlab.debian.vm.crt"
nginx['ssl_certificate_key'] = "/etc/gitlab/ssl/gitlab.debian.vm.key"

sudo gitlab-ctl reconfigure

sudo gitlab-ctl restart

