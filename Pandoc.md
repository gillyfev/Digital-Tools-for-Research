https://pandoc.org/

https://davepwsmith.github.io/academic-scrivener-howto/

# Set up
To set up:
+ Install BetterBibTex plugin
+ Export bibliographic library 
+ Install Pandoc 
+ Download CSL file 
+ Create reference document 

# Creating documents
1. Export from Scrivener 
- Compile for: Multi markdown 
2. Process through Pandoc: 
- Close all Word files! 
- Cmd 
- Get to directory:

cd <full_file_path>

cd C:\Users\gilefevr\OneDrive - University of Edinburgh\Doctorate\Papers\pandoc 
- Run Pandoc script:
  
pandoc workingpaper.md -s --citeproc -M reference-section-title="Bibliography" --bibliography Hippolytus.bib --csl turabian-no-ibid.csl -o output.docx --reference-doc=custom-reference.docx --from=markdown-example_lists
3. Open Word and check styles 

## Breakdown of pandoc command

## Reference doc
## CSL

https://www.zotero.org/styles
https://github.com/citation-style-language/styles/pull/7424
