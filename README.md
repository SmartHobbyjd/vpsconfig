# vpsconfig

systemctl start firewalld

systemctl status firewalld

systemctl enable firewalld

firewall-cmd --zone=public --add-port=443/tcp --permanent

firewall-cmd --zone=public --add-port=80/tcp --permanent

firewall-cmd --zone=public --add-port=8000/tcp --permanent

firewall-cmd --zone=public --add-port=8080/tcp --permanent

firewall-cmd --zone=public --add-port=9000/tcp --permanent

firewall-cmd --zone=public --add-port=9090/tcp --permanent

firewall-cmd --zone=public --add-port=4000/tcp --permanent

firewall-cmd --zone=public --add-port=3000/tcp --permanent

firewall-cmd --zone=public --add-port=3002/tcp --permanent

firewall-cmd --zone=public --add-port=3004/tcp --permanent

firewall-cmd --zone=public --add-port=3006/tcp --permanent

firewall-cmd --zone=public --add-port=3008/tcp --permanent

firewall-cmd --zone=public --add-port=5000/tcp --permanent

firewall-cmd --zone=public --add-port=8585/tcp --permanent

firewall-cmd --zone=public --add-port=27017/tcp --permanent

firewall-cmd --zone=public --add-port=5432/tcp --permanent

firewall-cmd --zone=public --add-port=3306/tcp --permanent

firewall-cmd --permanent --add-service=http

firewall-cmd --permanent --add-service=https

firewall-cmd --reload

firewall-cmd --list-services --zone=public

ss -tulpn

############

yum install git

git --version

git config --global user.name smarthobbyjd

git config --global user.email smarthobbyjd@gmail.com

git config --list

###########

adduser

passwd

userdel

usermod -aG wheel

############

wget

curl

cal 

touch

vi 

ls -l

cd ..
cd/
cd

rm -rf

tar -C
-xzf
yum install -y tar

tee  <<EOF
EOF

##################
wget https://go.dev/dl/go1.20.4.linux-amd64.tar.gz
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.20.4.linux-amd64.tar.gz
export PATH=$PATH:/usr/local/go/bin
go env
go env GOPATH
go version

#################

dnf install -y gcc-c++ make
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.20.4.linux-amd64.tar.gz
curl -sL https://rpm.nodesource.com/setup_16.x | sudo -E bash -

dnf install nodejs 
node -v 
npm -v
npm install --global yarn
yarn --version

################

yum repolist

hostname -I | awk '{print $1}'


################

Config directory – /etc/nginx/
Maibn global config file – /etc/nginx/nginx.conf
TCP ports opened by Nginx – 80 (HTTP), 443 (HTTPS)
Default web document root directory – /usr/share/nginx/html
Access log file – /var/log/nginx/access.log
Error log file – /var/log/nginx/error.log
