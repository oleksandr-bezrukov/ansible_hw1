# ansible_hw1
на всех машинах должен быть установлен python2.7
sudo apt update && sudo apt install python2.7 mc nano net-tools wget curl -y
python-pip postgresql-server-dev-10 -y

sudo apt update
sudo apt install software-properties-common

sudo apt-add-repository ppa:ansible/ansible

sudo apt update
sudo apt install ansible python2.7 wget curl mc net-tools nano -y

/etc/ansible/ansible.cfg 
прописать путь к приватному ключу 
private_key_file = ~/ans-keys/rsa_pub

склонировать репозиторий
git clone https://github.com/oleksandr-bezrukov/ansible_hw1.git

перейти в папку репозитория и в файле ansible_hosts указать внутренние адреса серверов nginx web-application postgresql
и путь к интерпретатору python2.7

в файле external_vars.yaml
поменять переменные
nginx_fqdn: ec2-18-221-116-221.us-east-2.compute.amazonaws.com - fqdn сервера nginx
pg_host: 127.0.0.1 - ip сервера postgresql
web_app_host: "127.127.127.127" - ip сервера web-application
