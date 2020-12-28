# rdf-xsl
The program will innput an xsl file and transofrm an rdf to it to legacy rdf format
by default the rdf has these namespaces to describe that it is an xml document with dublin core (dc) terms and additional resources from example.com

<?xml version="1.0" encoding="utf-8"?>
<rdf:RDF
    xmlns:dc="http://purl.org/dc/elements/1.1/"
    xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
    xmlns="http://www.w3.org/1999/xhtml">
  <rdf:Description rdf:about="http://example.org/">
    <dc:description rdf:parseType="Literal">
        <p xmlns="http://www.w3.org/1999/xhtml"></p>
    </dc:description>
  </rdf:Description>
</rdf:RDF>


The smantic web rule language explained under 
https://owlready2.readthedocs.io/en/latest/rule.html

The program expects that you host a file in another web server so the uri

http://localhost/movies2.n3

can display the following mime

@prefix dc: <http://purl.org/dc/elements/1.1/> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .

<file://C://Users//ah0169313//downloads//movies.n3> dc:title "Movies viewed by John Doe" .

<file://C://Users//ah0169313//downloads//movies2.n3#author> a foaf:Person ;
    foaf:mbox "john@doe.org" ;
    foaf:name "John Doe" .
    
    
 this can be done using IIS etc.
