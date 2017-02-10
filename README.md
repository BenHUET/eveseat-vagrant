# Usage

* [Download and install Vagrant](https://www.vagrantup.com/)
* `git clone git@github.com:BenHUET/eveseat-vagrant.git`
* `cd eveseat-vagrant`
* `vagrant up`. It can take some times since it's deploying a whole dev environnement (mysql, php, apache, composer...) and configuring SeAT.
* `vagrant ssh`
* `sudo /etc/apache2/sites-available/seat.conf` and edit the `ServerAlias` value by the correct address for this virtual machine
* `sudo apachectl restart`

You can now connect to your SeAT instance by browsing to `http://{ip address of the VM}/`.

[More info about Vagrant here.](https://www.vagrantup.com/docs/)