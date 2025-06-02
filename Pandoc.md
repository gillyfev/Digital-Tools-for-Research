https://pandoc.org/

https://davepwsmith.github.io/academic-scrivener-howto/

# Set up
To set up:
+ Install BetterBibTex plugin in Zotero
+ Export bibliographic library from Zotero to working folder
+ Install Pandoc onto your PC
+ Download CSL file to working folder
+ Create reference document in working folder

# Creating documents
1. Export from Scrivener 
- Compile for: Multi markdown 
2. Process through Pandoc: 
- Close all Word files! 
- Open Cmd window 
- Get to directory:

> cd <full_file_path> {working folder}

> cd C:\Users\gilefevr\OneDrive - University of Edinburgh\Doctorate\Papers\pandoc 
- Run Pandoc script:
  
> pandoc workingpaper.md -s --citeproc -M reference-section-title="Bibliography" --bibliography Hippolytus.bib --csl turabian-no-ibid.csl -o output.docx --reference-doc=custom-reference.docx --from=markdown-example_lists

3. Open Word and check styles 

## Breakdown of pandoc command
<table>
<tr><td>pandoc </td> <td> start the process </td></tr>
<tr><td> workingpaper.md </td> <td> name of the input file (compiled by Scrivener) </td></tr>
<tr><td>-s</td><td>produce a stand-alone document</td></tr>
<tr><td>--citeproc</td><td>Process the citations in the file</td></tr>
<tr><td>-M reference-section-title="Bibliography"</td><td>what to call my bibliography</td></tr>
<tr><td>--bibliography Hippolytus.bib</td><td>name and location of my bibliographical file</td></tr>
<tr><td>--csl turabian-no-ibid.csl</td><td>name and location of my citation style format file</td></tr>
<tr><td>-o output.docx</td><td>what to call my output file</td></tr>
<tr><td>--reference-doc=custom-reference.docx</td><td>use the file as a reference style guide</td></tr>
<tr><td>--from=markdown-example_lists</td><td>Enables citations without page numbers</td></tr>
</table>

## Reference doc

Pandoc documentation: https://pandoc.org/MANUAL.html

## CSL
Zotero style sheets: https://www.zotero.org/styles

Beta Chicago 18th: https://github.com/citation-style-language/styles/pull/7424
