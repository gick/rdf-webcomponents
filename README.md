# rdf-webcomponents
An attempt to use semantic for easier interfacing and prototyping of web components

Two distinct type of semantic web component pattern are proposed : 
## Semantic interface
 - A web component semantic interface pattern comports three specific attributes  : public-rdf-component, public-rdf-functions and public-rdf-propertie
 -public-rdf-component describes the type of web component that can/should be present in the same execution context, either through direct association or though event broadcast (ex : require a display component that can draw lines) 
 - public-rdf-functions describes public functions in terms of input (datatype property), output (sim), effect (concept of a WC ontology)
 -public-rdf-propeties will associate properties with datatype together with appropriate semantic (ex isa latitude, for a lat in degree)
 -
 
->An hosting component will allow to create a WC architecture based only on these interface, in a semantic Web Component repo

## Semantic model

- A semantic model pattern for web component imposes that the web component possess a consistent set of RDF statement from an OWL ontology. These statements describres the current state of affairs, **in terms of a domain (non webcomponent specific) ontology**. For instance it contains a list of instances of species with location in a botanical ontology.

- Operation on the semantic model web component are limited to legal operation over the model (adding legal statements, etc)

- The component exposes a minimal n3 version of its model

- A specific SPARQL web component allows to dynamic recover individuals property values

 -> An hosting component including SPARQL component will allow to create a WC architecture based on this model. This archictectures will specifies binding and constraint between different semantic model pattern. Exemple binding species from the previous ontology to rewards defined in a rewards web component describing way of rewarding in serious games.
 
 

For some perspective on this idea I wrote a little intro :
https://docs.google.com/document/d/e/2PACX-1vS_7NGqAHeT5LYzCNHFfROpGcnBPTKnOlkrl3CjBQC7yDPYnHv7NBwMZoF-dBu2On9oARISVmOL-Os0/pub
 
