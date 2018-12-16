#Item Catalog

This is the fourth project of Udacity's [Full Stack Web Developer Nanodegree](https://in.udacity.com/course/full-stack-web-developer-nanodegree--nd004/?).

The main objective is to develop a RESTful web application using the Python framework Flask along with implementing third-party OAuth authentication.

### Getting Started
#### Setup VM
* Install [Vagrant](https://www.vagrantup.com/downloads.html)
* Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* Clone the [Vagrant Configuration Repository](https://github.com/udacity/fullstack-nanodegree-vm)
* cd into vagrant folder and run the command `vagrant up` in your terminal to install the operating system as per the Vagrantfile.
* To connect to VM, simply run the command `vagrant ssh`.

#### Setup Project
* First ssh into the VM.
* Clone the [repository](https://github.com/rajgiridhar1995/Item-Catalog) inside the vagrant folder.
* cd into the cloned repository folder.
* Setup the database by running the command `python database_setup.py`.
* To fill the database with mock data, run the command `python lotsofmenu.py`.
* Finally start the web application by running the command `python application.py`.

#### API Documentation
* `/api/v1/restaurant/JSON` - to obtain a list of all restaurant.
* `/api/v1/restaurant/<int:restaurant_id>/menu/JSON` - to obtain the menu of particular restaurant.
* `/api/v1/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON` - to obtain details of a particular item from the menu.
