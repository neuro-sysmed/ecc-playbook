# ecc-playbook
Playbooks for ecc


Install

```
sudo yum install -y git
git clone 
python3 -m venv venv
source venv/bin/activate
pip3 install wheel -q
pip install -U pip

git clone https://github.com/neuromics/ecc-playbook

cd ecc-playbook

pip install -r requirements.txt

ansible-galaxy install -p roles -r requirements.yml


ssh-keygen -q -t rsa -N '' -f ~/.ssh/id_rsa <<<y

cp ~/.ssh/id_rsa.pub ~/.ssh/authorized_keys

ansible-playbook ecc.yml

az login 
# follow instructions...


```
