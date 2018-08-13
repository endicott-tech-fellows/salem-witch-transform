# salem-witch-transform
This is a web app that transforms network data about the Salem witch trials from one format to another that is more useful with Gephi.

## To begin
Open `update-edges.html` in any browser. Follow the instructions on the page.

## Input
The input file should be a comma separated values (CSV) file with at least five columns:

  * Source (a node id)
  * Target (a node id)
  * Type (directed, undirected, or blank)
  * Weight (a number, can be blank)
  * Relationship (a number where 1=Accuser, 2=Court Official, 3=Hearsay, 4=Witness for, 5=Witness against, 6=Co-accused, and 99=Unknown)

## Output
The output of this process is a zip file containing the following files:

  * accuser-edges.csv
  * court-official-edges.csv
  * witness-for-edges.csv
  * co-accused-edges.csv
  * uknown-edges.csv
  * all-edges.csv


Each of these have six columns:

  * Source (a node id)
  * Target (a node id)
  * Type (directed, undirected based on the relationship type)
  * Weight (a number&mdash;always 1)
  * Relationship (a number where 1=Accuser, 2=Court Official, 3=Hearsay, 4=Witness for, 5=Witness against, 6=Co-accused, and 99=Unknown)
  * Label (the label that corresponds to the relationship value)
