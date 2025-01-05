# PIE Etymology Project
A project to create etymological dictionaries for the PIE language family.


### Tags

These are the tags that will be recognised.

\\lex - required, begins a new entry and gives the citation form for the new lexeme. If there are multiple variant forms (e.g. a variable affix) they should be space-separated. If multiple homonymous lexemes need to be distinguished, place a number in brackets `()` after the citation form.
\\stem - optional, gives the stem(s) for the lexeme. If there are multiple stems, they should be space-separated.
\\morph - optional, gives a morphemic breakdown of the lexeme. Morphemes should be space-separated. If not given, the lexeme is assumed to be monomorphemic
\\class - required, gives the lexical class of the lexeme. This should fully identify the inflection, and ideally the syntactic type as well. \\class may be given more than once, if a word is multi-functional, and each instance can have its own \\gloss.
\\gloss - required, gives the English translation(s) of the lexeme. Markdown may be used for formatting.
\\from:{lang} - optional, gives the antecedent lexeme for an inherited word. {lang} must be one of the identifiers from the `/languages.txt` file, indicating the parent language.
\\loan:{lang} - optional, gives the donor lexeme for a loanword. {lang} must be one of the identifiers from the `/languages.txt` file, indicating the donor language.
\\base - optional, gives the derivational base(s) of the lexeme and the affix(es) used to derive it.
\\desc:{lang} - optional, gives a descendent lexeme. {lang} must be one of the identifiers from the `/languages.txt` file, indicating the daughter language. Only to be used when the daughter language doesn't have its own file.
\\cogn:{lang} - optional, gives a cognate lexeme within the same branch. Inexact cognates should be accompanied by a gloss. This should not be used for long-range cognates. {lang} must be one of the identifiers from the `/languages.txt` file, indicating the sister language. Only to be used when the sister language doesn't have its own file.
\\notes - prose discussion of the reconstruction, etymology, or similar topics. Markdown may be used for formatting. Line breaks can be used, so long as no line begins with \\; such lines will be interpreted as a tag and the notes field will end.
\\ref - required, gives a space-separated list of references. Each reference should be as detailed below.

If additional tags are required, talk to Kat.

### References

References should be detailed in the `/references.txt` file. Each reference should be on a separate line, beginning with a unique identifier, then the author, year, title, link (if available), and any extra information. A good identifier will be the author's surname in lower-case (plus any additional letters from forenames to disambiguate), followed by the year of publication, then a letter to disambiguate multiple publications from the same author in one year. Alternatively, for significant reference works (such as older dictionaries), an abbreviation of the title can be used. To prevent unnecessary reference duplication, try to insert references in sorted order, and never change an identifier after the fact.

In the dictionary, references should be cited by their identifier. If a specific page is to be referenced (e.g. to identify a specific entry in an etymological dictionary), the page number can be appended to the identifier with a colon in between. e.g `EDHIL:161` for page 161 of the reference `EDHIL`.
