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
