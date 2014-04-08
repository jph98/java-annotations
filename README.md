java-annotations
================

There's some useful stuff that can be done with annotations.

Marker Interfaces
-----------------

First-up is marker interfaces which just allow you to mark a class, package or other construct as belonging to something or meant for a particular purpose.

Google exposes the @VisibleForTesting to indicate that something (e.g. a method) has been made package-private to enable testing.  Not a great practice for greenfield development, but very good for working with legacy code.

Some example I provide here in this project are:
* @WorkInProgress - for a partially complete class or method that you need to checkin.  You can find that

Good intro here on this - http://isagoksu.com/2009/development/java/creating-custom-annotations-and-making-use-of-them/

Code Generation
---------------

AOP is the standard way to do this (bit heavyweight and overkill), but you can also use the following to inject code at compile and runtime:

* Reflections - https://github.com/ronmamo/reflections
* JavaDude Annotations - https://code.google.com/p/javadude/wiki/Annotations

More articles here:
* http://deors.wordpress.com/2011/09/26/annotation-types/
