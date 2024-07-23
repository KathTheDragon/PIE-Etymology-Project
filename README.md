# PIE Etymology Project
A project to create etymological dictionaries for the PIE language family.


### Tags

These are the tags that will be recognised.

\\lex - required, begins a new entry and gives the citation form for the new lexeme. If there are multiple variant forms (e.g. a variable affix) they should be space-separated. If multiple homonymous lexemes need to be distinguished, place a number in brackets `()` after the citation form.
\\stem - optional, gives the stem(s) for the lexeme. If there are multiple stems, they should be space-separated.
\\morph - optional, gives a morphemic breakdown of the lexeme. Morphemes should be space-separated. If not given, the lexeme is assumed to be monomorphemic
\\class - required, gives the lexical class of the lexeme. This should fully identify the inflection, and ideally the syntactic type as well.
\\gloss - required, gives the English translation(s) of the lexeme. Markdown may be used for formatting.
\\from:{lang} - optional, gives the antecedent lexeme for an inherited word. {lang} should be an unambiguous identifier for the ancestor language. Try to be consistent.
\\loan:{lang} - optional, gives the donor lexeme for a loanword. {lang} should be an unambiguous identifier for the donor language. Try to be consistent.
\\base - optional, gives the derivational base(s) of the lexeme and the affix(es) used to derive it.
\\desc:{lang} - optional, gives a descendent lexeme. {lang} should be an unambiguous identifier for the descendent language. Try to be consistent.
\\cogn:{lang} - optional, gives a cognate lexeme within the same branch. This should not be used for long-range cognates. {lang} should be an unambiguous identifier for the sister language. Try to be consistent.
\\notes - prose discussion of the reconstruction, etymology, or similar topics. Markdown may be used for formatting. Line breaks can be used, so long as no line begins with \\; such lines will be interpreted as a tag and the notes field will end.
\\ref - required, gives a space-separated list of references. Each reference should be as detailed below.

If additional tags are required, talk to Kat.

### References

References should be detailed in separate `references.txt` files. While any dictionary can reference from any such file, regardless of location, it would be best to organise references by the primary branch they discuss. So, for example, an article talking mainly about Greek should be placed in `/Hellenic/references.txt`. If the reference talks about many branches, so that none of them can be considered primary, it should either be placed in `/PIE/references.txt` or `/references.txt`. Use your best judgement. Either way, try not to duplicate references if you can avoid it.

Each reference should be on a separate line, beginning with a unique identifier, then the author, year, title, link (if available), and any extra information. In the dictionary, references should be cited by their identifier. If a specific page is to be referenced (e.g. to identify a specific entry in an etymological dictionary), the page number can be appended to the identifier with a colon in between. e.g `EDHIL:161` for page 161 of the reference `EDHIL`.
