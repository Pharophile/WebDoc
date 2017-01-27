Pharo WebDoc
============

Pharo webdoc provides a way to export HTML documentation as static files out of a Pharo image.
Pharo webdoc also allows an image to serve the same content right from the image with the webdoc handler.


Loading WebDoc
--------------

    Gofer it 
	smalltalkhubUser: 'PharoExtras' project: 'WebDoc';
	package:'ConfigurationOfWebDoc';
	load.
	
    (#ConfigurationOfWebDoc asClass project version: #development) load.

Exporting WebDoc content
------------------------

    (WebDocExporter packages: {RPackageOrganizer default packageNamed: 'MyPackage' "packages"}) exportTo: './doc' asFileReference.

Serve WebDoc content
--------------------

    ./pharo-ui Some.image webdoc --server=8089 


Still lots of things to do here, but that is the basic stuff.

Scripts are in this folder for one to customize.


