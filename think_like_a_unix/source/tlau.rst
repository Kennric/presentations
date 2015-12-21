=================
Think Like a Unix
=================

Kenneth Lett
OSU Open Source Lab


A Wombat
========

.. figure:: /_static/wombat.jpg
    :align: center
    :width: 600

.. note::

	a philosophical talk
	Unix philosophy pervades software development and operations on every scale
	learning to think Unix-y will make your life easier

	What is UNIX?

Little Pieces
=============

.. rst-class:: build

* Simple commands
* Do one thing
* Do it well
* Plain text in, Plain text out

.. note::

	What is this philosphy?
	This is only part of it, the parts that scale to every level of computing
	Large, complex systems can be built and managed using small pieces
	that work together

	Not just text input, but text options and control 


The Philosphy At Work
=====================

**Tools**

.. rst-class:: build

* Files and text: ls, cat, awk, grep, sed, df, du
* Process and Memory: ps, free, lsof
* Network: ip, host, netstat, curl
* What about top?

.. note::

	The fabric of your userspace is made up of little tools that work
	together in Unix-y ways

	after first bullet, go to terminal


The Philosphy At Work
=====================

**Code**

.. rst-class:: build

* Functions, Classes, Methods
* Common data structures
* Modules
* Libraries
* Loose coupling

.. note::

	All these concepts are familiar from good programming practice
	note data structures a little more defined

	Is this the most efficient way to do things?


The Philosphy At Work
=====================

**The Web**

.. rst-class:: build

* Twitter, Instagram, Stack Exchange provide HTTP APIs
* Github is made of UNIX-y goodness
* Facebook?
* HTTP is the | of the Web
* What is the Plain Text of a UNIX-y Web?

.. note::

	Let's move to the web.

	Seems like a home run, unix-y web apps built of microservices, 
	but this is actually pretty new

	providing API's is good, but can the pieces be assembled?
	Github uses git, travis, oauth, etc, etc
	Google is a pile of pieces - some monlithic, some micro
	Facebook - like top? Do you know if it is made of pieces? Do you
	care?


Aside: What is an API?
======================

.. rst-class:: build

* Apple Proprietary IP?
* Autonomous Python Instance?
* Actually Pretty Important?
* Application Programming Interface?
* A Document
* A Contract
* What is the Plain Text of a Web API?

.. note::

	It's all about the API - tools tied together by api
	API tells you how to send 'plain text' and what to send
	API tells you what 'plain text' will come out
	API is what allows you to build complex systems out of small 
	pieces
	Not HTML, not pure HTTP - need to be able to pipe it around
	need more structure than plain text
	but not so much that it is hard to use

	show man page for curl, --help for something

The New Plain Text
==================

**XML?**


.. code-block:: xml

	<!DOCTYPE glossary PUBLIC "-//OASIS//DTD DocBook V3.1//EN">
	 <glossary>
	  <title>example glossary</title>
	  <GlossDiv>
	   <title>S</title>
	   <GlossList>
	    <GlossEntry ID="SGML" SortAs="SGML">
	     <GlossTerm>Standard Generalized Markup Language</GlossTerm>
	     <Acronym>SGML</Acronym>
	     <Abbrev>ISO 8879:1986</Abbrev>
	     <GlossDef>
	      <para>A meta-markup language, used to create markup languages such as DocBook.</para>
	      <GlossSeeAlso OtherTerm="GML">
	      <GlossSeeAlso OtherTerm="XML">
	     </GlossDef>
	     <GlossSee OtherTerm="markup">
	    </GlossEntry>
	   </GlossList>
	  </GlossDiv>
	 </glossary>

.. note::
	
	635k

	arbitrarily defined structure
	infinitely flexible structure
	-have- to define an arbitrary structure
	is xml unix-y?

The New Plain Text
==================

**JSON**

.. code-block:: json

	{
	 "glossary": {
	  "title": "example glossary",
	  "GlossDiv": {
	    "title": "S",
	    "GlossList": {
	     "GlossEntry": {
	      "ID": "SGML",
	      "SortAs": "SGML",
	      "GlossTerm": "Standard Generalized Markup Language",
	      "Acronym": "SGML",
	      "Abbrev": "ISO 8879:1986",
	      "GlossDef": {
	       "para": "A meta-markup language, used to create markup languages such as DocBook.",
	       "GlossSeeAlso": ["GML", "XML"]
	      },
	      "GlossSee": "markup"
	     }
	    }
	   }
	  }
	 }

.. note::
	
	515k

	easy to understand, no xslt needed, no special tags, just brackets
	infintitely flexible content

	is JSON Unix-y?

	JSON is the defacto language of Web APIs


A Digression 
============

**What is an Open API?**

.. rst-class:: build

* Accessible on the Public Internet?
* Accessible for Free?
* Accessible without an account?
* Free to implement?
* Open Source

.. note::

	Free to use is not Open
	Demo public data api here?
	There is no right answer, but the right answer is OS


Another Wombat
==============

.. figure:: /_static/wombat2.jpg
    :align: center

.. note::

	Mobile - now the interface is more removed, and more than
	one interface is needed - APIs FTW


What Else is UNIX-y?
====================

**The Cloud**

.. rst-class:: build

	* OpenStack: a pile of APIs
	* Ganeti
	* Docker?

.. note::

	Docker is a monolithic package made up of unixy parts, running as 
	single item in an API driven ecosystem


What Else is UNIX-y?
====================

**Configuration Management?**

.. rst-class:: build

	* Modules, Recipes, Cookbooks and Manifests
	* How do they communicate with each other?



In Conclusion
=============


.. figure:: /_static/wombat3.jpg
    :align: center


.. note::

	write unix-y code
	buld unix-y tools


Thank You
=========

Kenneth Lett
OSL Open Source Lab

Twitter: @KenLett
IRC: kennric on freenode