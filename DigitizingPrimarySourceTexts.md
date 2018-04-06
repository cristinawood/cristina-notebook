## Digitizing Primary Source Texts - workshop with Constance Crompton

What is Text Encoding? 
https://owncloud.westgrid.ca/index.php/s/s8dIehamxX8iXSh slides! 

Using TEI XML (language) to tell computers what we know about a text. 
- organizing the chaos of plaintext 

### Hands on: Drawing boxes
- Draw boxes around content on the page that attracts your attention! 
- TEI there to help us say what matters to us! 
- letter sample: drawing boxes around what kind of things you want to have stand out to the computer! 
- style of letterhead, could highlight images/logos for aggregation
- Some of the things you might want to represent
  - ref's to people, places, events, orgs
  - physical document with dimensions, damages,
  - linguistic analysis showing parts of speech, phrasing, clauses
  - metadata record with details of authorship, date of creation, provenance, genre
  - vector analysis of handwriting shapes and position of marks on the page
  - paragraphing and document structure

### XML Markup is Everywhere
- eXtensible Mark-up Language
- KML in Maps
- TEI (editions) - to work with text, designed, english lit background
- WordprocessingML
- etc. 

### XML Anatomy
- ```<location>uOttawa</location>```
- ```<location type="university">uOttawa</location>```

### Elements, Nesting, One Root
- XML docs all have elements, attributes, and values. 
- All XML-based languages' elements ***nest*** and **never overlap**
- have a single ***root element*** and can be expressed as a hierarchy, or tree

### What is the Text Encoding Initiative?
- predates HTML! 
- hardware and software independent
- computationally tractable
- formal 
- reusable - for different applications! 
- useful standard in Digital Humanities

### TEI-XML
- XML gives us the syntax to describe things to a computer - opening tags and closing tags
- TEI gives us the language, the vocabulary and grammar

### When is TEI Knowledge Useful? 
#### Single encoding, multiple outputs. 
- write scripts to produce different outputs! 
- XLST script! 
- encode once, pull things from document that output formats need.
#### Close Reading and Patterns at Scale
- you can see different patterns, as well as looking really closely
- Julia Flanders & Matt Jockers
#### Aggregation, Peer Review, Grants
- Evaluating others' DH projects
- grants (agencies like to see that projects will use disciplinary standards)

### How the TEI represents texts
``` 
<?xml version="1.0" encoding="UTF-8"?>
<TEI>
 <teiHeader> <!- this is where the information about the encoded document goes--> </teiHeader>
 <text>
 <body>
 inlcude that 
 </body
 </text>
</TEI>
```
Can demarcate ```<foreign xml:lang="fr">sang froid</foreign>```
Walt Whitman archive can give you TEI files, stripping some details. 
Python script to prepopulate some things! 
#### Poetry terms
- lg for line groups, quatrain etc. 
#### Theatre terms
- stage entrances and exits etc. 
#### Letters
```
<opener>
 <dateline>
  <date when=1846
 </dateline>
</opener>
```
### Beyond Drawing Boxes
- segmentation
- linking
- referencing

### In practice
- knightlab can grab info and populate with it, on a map
- gephi to visualize networks/connections
- oXygen - to check your documents against the ones online

### TEI Guidelines
- http://www.tei-c.org/release/doc/tei-p5-doc/en/html/index.html
- DHSite.org to follow up on those events!
