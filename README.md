# Prerequisites

* [Download and install Vagrant.](https://www.vagrantup.com/) [More info about Vagrant here.](https://www.vagrantup.com/docs/)
* [Virtualbox 5.0.X.](https://www.virtualbox.org/wiki/Download_Old_Builds_5_0)

# Installation

* `git clone git@github.com:BenHUET/eveseat-vagrant.git`
* `cd eveseat-vagrant`
* `vagrant up`. It can take some times since it's deploying a whole dev environnement (mysql, php, apache, composer...) and configuring SeAT.
* `vagrant ssh`
* `sudo /etc/apache2/sites-available/seat.conf` and edit the `ServerAlias` value by the correct address for this virtual machine
* `sudo apachectl restart`

# Usage

You can now connect to your SeAT instance by browsing to `http://{ip address of the VM}/`.

# Credentials

* SeAT `admin:password`
* MySQL `root:password` (remote access allowed)

# Troubleshooting

If the installation fails, execute `vagrant destroy` to rollback to a clean state.