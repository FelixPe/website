---
home: true
heroImage: /hero.png
heroText: RDF on Elixir
tagline: "Linked Data ❤ Elixir"
actionText: Get Started →
actionLink: /rdf-ex/
features:
- title: RDF.ex
  details: >-
    Data structures to build RDF graphs and datasets; load and store RDF graphs and datasets in the most popular serializations formats - N-Triples, Turtle, JSON-LD
- title: SPARQL.ex
  details: >-
    Perform SPARQL queries against the data in your RDF.ex data structures
- title: SPARQL.Client
  details: >-
    Perform SPARQL queries against any SPARQL service - Wikidata, Dbpedia, you name it 
footer: MIT Licensed | Copyright © 2017-present Marcel Otto
---

```elixir
def schema_org_description do
  ~I<https://rdf-elixir.dev>
  |> RDF.type(Schema.Website)
  |> Schema.about(TODO)
  |> JSON.LD.write_file!("description.jsonld")
end
````
