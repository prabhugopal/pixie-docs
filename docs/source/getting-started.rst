.. _here: https://github.com/pixie-lang/pixie/releases

Getting started
===============

Pixie implements its own virtual machine therefore in order to use Pixie the Pixie-VM is required. Pixie-VM may either be built from source or a release may be downloaded. 


Quickstart
----------

The latest Pixie-VM (PVM) is available binary is available `here`_. The PVM is currently in alpha.

Building from source
--------------------

Building from source is currently possible on 4 platforms:

#. Arch

#. Debian

#. FreeBSD

#. OS X

Builing on Arch
^^^^^^^^^^^^^^^
::

	pacman -S libuv libffi python2
	mkdir ~/projects/pixie-lang
	cd ~/projects/pixie-lang
	git clone https://github.com/pixie-lang/pixie.git
	cd pixie
	PYTHON="/usr/bin/python2" make build_with_jit
	mkdir ~/bin
	cd ~/bin

Building on Debian
^^^^^^^^^^^^^^^^^^
::

	sudo apt-get install build-essential pkg-config 
	sudo apt-get install curl libffi-dev libedit-dev 
	sudo apt-get install libboost-all-dev
	sudo apt-get install libuv-dev 
	git clone https://github.com/pixie-lang/pixie.git
	cd pixie
	make build_with_jit

Building on FreeBSD 10.1
^^^^^^^^^^^^^^^^^^^^^^^^
::

	pkg install libuv libffi gmake readline python
	git clone https://github.com/pixie-lang/pixie.git
	cd pixie
	make build_with_jit

Building on OS X via Homebrew
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
::

	brew install libuv libffi boost
	git clone https://github.com/pixie-lang/pixie.git
	cd pixie
	make build_with_jit


Installation
------------

Once the PVM has been obtained it is advised that a symbolic link from the PVM to the */usr/bin/pixie* directory be created. 

**This documentation assumes that an alias (pixie) to the PVM has been created**

Verify the installion of Pixie by entering the following in the terminal:

::
	
	$ pixie -v

If installed correctly the installed version of pixie will echoed.
