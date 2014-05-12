lion-rent
=========


## Requirements

* [pyenv](https://github.com/yyuu/pyenv)
* [Ansible](http://www.ansible.com/home)

## Requirements Install

Requirement Tool install tutorial


### OSX installration

requirements [Homebrew](http://brew.sh/)

### Homebrew (OSX Only)

----

```
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
brew doctor
```

### homebrew-cask (OSX Only)

----

[homebrew-cask](https://github.com/caskroom/homebrew-cask)

> a CLI workflow for the administration of Mac applications distributed as binaries 
http://caskroom.io

```
brew tap caskroom/cask
brew install brew-cask
```

### Linux installration

### Pyenv

----

* pyenv install

```
brew install pyenv
echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bash_profile
source ~/.bash_profile
```

* python2.x install

```
pyenv install 2.7.6
pyenv rehash
python --version
# install Python complate!!
Python 2.7.6
```

### Ansible

----

[about-ansible](http://docs.ansible.com/#about-ansible)

> Ansible is an IT automation tool. It can configure systems, deploy software, and orchestrate more advanced IT tasks such as continuous deployments or zero downtime rolling updates.

* ansible install

```
pip install paramiko PyYAML jinja2 httplib2 ansible
```

## Usage


### First only one local machine installration (OSX)



```
ansible-playbook -i lion-rent-ansible/inventories/osx -c local --ask-sudo-pass lion-rent-ansible/site.yml
```

