pixie.fs
=============

The ``pixie.fs`` namespace provides functionality for interfacing with the file system.

pixie.fs.dir
###################

Returns a dir ``d`` if the path is a dir or does not exist. If a different filesystem object exists at the path an error will be thrown.

::

	(dir d)


Example usage

::

	(ns fs-test)

	(dir "/etc")
	;=> <Dir /etc>


pixie.fs.file
###################

Returns a file if the path ``p`` is a file or does not exist. If a different filesystem object exists at the path an error will be thrown.

::

	(file p)


Example usage

::

	(ns fs-test)

	(file "~/.bashrc")
	;=> <File /home/pixie/src/~/.bashrc>


pixie.fs.fspath
###################

Returns either a File or Dir ``fd`` if they exist at the path
::

	(fspath fd)


Example usage

::

	(ns fs-test)

	(fspath "/etc")
	;=> <Dir /etc>
	(fspath "~/.bashrc")
	;=> <File /home/pixie/src/~/.bashrc>

pixie.fs.rel-path
###################

Get the common root of the two paths, ``path1`` and ``path2``, and the bits that diverge

::

	(rel-path path1 path2)


Example usage

::

	(ns fs-test)

	;TODO