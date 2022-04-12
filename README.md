# Docx2Jats

Requirements
- admin rights on your device
- pandoc installed https://pandoc.org/installing.html

Preperation of the .docx file (see article.docx)
- delete metadata (authors, abstract, publication dates, ...). Metadata have to be added manually after conversion
- tag headings consequently (until 3 Levels)
- insert footnotes in MS Word

Converting .docx to Jats xml
- save the prepared .docx file(s) in a directory where you want to do the conversions
- open cmd shell
- navigate to the specific folder (for example on a Windows system `C:\>cd \Users\name\documents\conversions` )
- there you convert the wanted file by entering the following pandoc command: `pandoc -s -t jats example.docx -o example.xml` . the xml file will be automatically created

Post-Processing
- open the created xml file in an xml editor (for example https://notepad-plus-plus.org/ )
- add metadata manually into the `<front></front>` element. See article_withBibliographyAndMetadata.xml as an orientation. 
- if your article has a bibliography you have to put the references into `<ref><mixed-citations></mixed-citations></ref>` elements with a unique ID attribute. Afterwards you link the refs out of the text using the `<xref></xref>` element. See article_withBibliographyAndMetadata.xml


