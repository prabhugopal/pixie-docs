pixie.csp
=============

The ``pixie.csp`` namespace provides functionality for communicating sequential processes.

pixie.csp.close!
###################

Closes the channel ``c``, future writes will be rejected, future reads will drain the channel before returning nil.

::

	(close! c)


Example usage

::

	(ns csp-test)

	;TODO


pixie.csp.put!
###################

Puts the value ``v`` into the channel ``c``, calling the optional callback ``f`` when the operation has completed.

::

	(put! c v)
	(put! c v f)


Example usage

::

	(ns csp-test)

	;TODO

pixie.csp.take!
###################

"Takes a value from a channel ``c``, calling the provided callback ``f`` when completed"

::

	(take! c)
	(take! c f)


Example usage

::

	(ns csp-test)

	;TODO
	
pixie.csp.alts!
###################

No documentation

pixie.csp.>!
###################

No documentation

pixie.csp.<!
###################

No documentation