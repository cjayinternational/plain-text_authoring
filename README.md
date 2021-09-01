# Asciidoc localization
Localization resources for Asciidoc

This repository includes the following resources:
- English Asciidoc files
- machine translations into Spanish
- HTML conversion of the translated Asciidoc files
- parser (memoQ)
- XLIFF files (memoQ)
- TMX

The parser for memoQ is regex-based. It has been created based on the English Asciidoc files included in this repository. When using it to translate another set of Asciidoc files, it might need to be modified. The parser deals with many delicate things in Asciidoc such as:
- alt text in images
- comments
- footnotes
- formatting
- hyperlinks
- paragraph delimiters
- xrefs

Note that it is very important to write Asciidoc files with localization in mind. These are a couple of things that technical writers should do to ensure a clean import of the Asciidoc files into memoQ using the provided parser:
- avoid multi-line comments
- avoid unnecessary newlines
- start every file with a title
- start paragraphs after comments with a delimiter
