# vagrant-jenkins
Vagrant setup of a jenkins server VM based on a centos 7 box: https://app.vagrantup.com/centos/boxes/7

Uses the following ansible roles :
- [geerlingguy.java](https://github.com/geerlingguy/ansible-role-java)
- [geerlingguy.jenkins](https://github.com/geerlingguy/ansible-role-jenkins)

# Setup:

[Install VirtualBox](https://www.virtualbox.org)

[Install vagrant](https://www.vagrantup.com/downloads.html)

[Install ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html?extIdCarryOver=true&sc_cid=701f2000001OH7YAAW#installing-the-control-machine)

Clone repo
```
git clone https://github.com/jdlourenco/vagrant-jenkins.git
```

cd to main project dir:
```
cd vagrant-jenkins
```

Install required ansible roles from ansible-galaxy (may require sudo depending on how ansible was installed):
```
ansible-galaxy install -r requirements.yml
```

Run vagrant up
```
vagrant up
```

# Usage

Access admin interface at http://localhost:8080 using default credentials: `user: admin` and `password: admin`
