
Hello World
===========

The most basic Pixie program

::

	;Pixie comments are preceded by a semicolon. 
	;This whole line is a comment

	(println "Hello Neverland")

The following program highlights some functions in Pixie

::

	;This code snippet highlights a basic program in Pixie

	(ns hello-neverland) ;declare the namespace

	(print "Goodbye world!\n")	
	;print does not terminate the output with a new line

	(loop [x 5]					
	;a basic loop
	  (when (> x 0)				
	  ;this loop runs while x > 0
	    (print (str x "\n"))	
	    ;string can be built using (str string1 string2 ... stringN)
	    (recur (- x 1))))		
	    ;x is decremented on each interation

	(println "Hello Neverland!")
	;println terminate the output with a new line