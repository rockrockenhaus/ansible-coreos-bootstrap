First, on the developer machine, install Vagrant and VirtualBox:

(assume we're on a Mac)

Install brew:

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Install VirtualBox:

brew cask install virtualbox

Install Vagrant

brew cask install vagrant



Once you have installed VirualBox and Vagrant, you need to provision your instances.  

Ansible requires Python, we will use pypy, no need to reinvent wheel (ansible-galaxy install defunctzombie.coreos-bootstrap)

Create an ansible hosts file (etc/ansible/hosts)

Install pypy by running "ansible-galaxy install defunctzombie.coreos-bootstrap"

You must run the playbooks in this order:


