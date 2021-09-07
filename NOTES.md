# This is cool but it could be even a little cooler

Moving from flat ASCII text to structured data is a great idea.
Let's go one step further and make information discoverable, by
using RDF with a UNIX ontology. Some of the nouns and verbs in the
UNIX ontology would be things like

* file/directory
* name
* permission bits
* author/owner/group
* creation/modification/access date
* list of files/directories

If the next program in a pipeline knew how to parse RDF and refer
to ontologies, then we could get rid of all those "--ls", "--ifconfig",
etcetera command line options.

What I guess I would plan to do is add a "--rdf" option, and then it would
switch from generating JSON to generating RDF. In the interest of human
readability, it should be N3 or Turtle, not RDF/XML.
