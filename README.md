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

ansible-playbook ecc_bootstrap.yml

az login 
# follow instructions...

cd /cluster/lib/ecc
source venv/bin/activate
./bin/ecc-cli add ecc-node 

cd -
ansible-playbook ecc_bootstrap.yml



```
