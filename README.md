# Docx2Jats

.docx to .md via pandoc

command line: pandoc --standalone --to markdown --metadata-file=article_neu.yaml --atx-headers -o article_neu-raw.md article_neu.docx 



.md to jats via pandoc

command line: pandoc --standalone --to jats -o article_neu.xml article_neu.md

