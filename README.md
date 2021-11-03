# ecc-playbook

Have been integrated into neuro-sysmed infrastructure-playbook 



Playbooks for ecc


Install head nodes
==================

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
ansible-galaxy collection install -r requirements.yml

ansible-playbook ecc_bootstrap.yml

az login 
# follow instructions...

/usr/local/bin/ecc-cli add ecc-node 

ansible-playbook ecc_bootstrap.yml

```

Create images
------------

This is to be done with both the ecc-head and ecc-node vms


go to the azure portal 
select ecc-node (in virtual machines )
Top bar click capture (?)
share in gallery
Auto delete after creation (?)
Keep default name (ecc-node-image-datetime)
tags:
createdBy: Your name

review & create
Once create view resource and note the resource id!











