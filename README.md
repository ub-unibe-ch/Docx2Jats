# Docx2Jats

.docx to jats via pandoc:

command-line: pandoc -s -t jats example.docx -o example.xml



.docx to .md via pandoc:

command line: pandoc --standalone --to markdown --metadata-file=example.yaml --atx-headers -o example-raw.md example.docx 



.md to jats via pandoc:

command line: pandoc --standalone --to jats -o example.xml example.md

