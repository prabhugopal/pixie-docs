pixie.buffers
=============

The ``pixie.buffers`` namespace provides functionality relating to the use of `pixie.stdlib.Buffer`

pixie.buffers.acopy
###################

Copies ``len`` elements from the source buffer (``src``) starting at the ``nth`` element to the destination buffer (``dest``) starting at the ``mth`` element

::

	(acopy src nth dest mth len)


Example usage

::

	(ns buffer-test)

	;TODO