# version2_files
A Repository for all the files to be converted for the new DAT site

## Using Pandoc

If you need to convert files from one markup format into another, [Pandoc](https://pandoc.org/) is your swiss-army knife. Pandoc can convert between the following formats:

(← = conversion from; → = conversion to; ↔︎ = conversion from and to)

### Installing

[Pandoc - Installing pandoc](https://pandoc.org/installing.html)

#### Using command line

Coverting files **.docx** to **.html**

`find ./ -iname "*.docx" -type f -exec sh -c 'pandoc "${0}" -t html --wrap=none -o "${0%.docx}.html"' {} \;`

Coverting files **.docx** to **.md**

`find ./ -iname "*.docx" -type f -exec sh -c 'pandoc "${0}" -t gfm --wrap=none -o "${0%.docx}.md"' {} \;`

