# Formatting Guide

This file will describe in detail the suggested format for entries in the dictionary files. If you think a change should be made, write up a number of sample entries in both the old and new formats and show them to Kat, along with an explanation of why this is an improvement.

## Overall Layout

The overall layout of an entry is as follows:
- lemma, class, and translation
- derivatives (if applicable)
- cognates (if the entry is for a "primary" attested language within its branch) / descendents (if the entry is for a reconstructed language)
- ancestry (if an etymology is accepted)
- discussion of the word and its etymology
- references

As the current files use markdown, each line needs to be ended with a space and a backslash (` \`) in order to add a line break. Additionally, attested forms should be written with italics (`_text_`) and links (`[text](link)`) used to reference other entries elsewhere in the dictionary. References to other sources should be done as endnotes (`[label]: link "Title"` at the end of the file, `[label]` in text) with a link to a references document, where the source is given in full. The entry heading should contain an html `<a>` element which has its `id` attribute set to some specific representation of the lemma with punctuation removed. For example, the id for "_-a(ri)_, _-at(i)_" is `"ari"`, and for "_ariye/a-_" is `"ariye"`. Unicode letters do not need to be converted to ASCII.

## Lemma, Class, and Translation

The lemma should be given in some standardised form, though this may vary from language to language. If multiple paradigmatic stems need to be given, they should be separated by a tilde (`~`), e.g. "_arai-_ ~ _ari-_". Alternating segments should be separated by a slash (`/`), e.g. "_hame/ink_", and optional segments should be enclosded in brackets (`(...)`), e.g. "_as(sa)nu-_". Any other set of alternate forms, including multiple paradigms, should be separated by commas (`,`), e.g. "_ark-_, _ārk-_ ~ _ark-_". If the lemma is for a reconstructed language, it should be prefixed by an escaped asterisk (`\*`).

The class of a stem or paradigm should be given immediately after the form(s), and should include both information about the part of speech, and which inflection type the stem falls into, e.g. "_apā-_ ~ _apū-_ [pron]", "_harsi-_ ~ _harsai-_ [c. n]". If there are multiple stems or paradigms of different classes, each one should be marked with its own class, e.g. "_hās-_ ~ _hass-_ [i v], _hēs-_ ~ _hess-_ [zi v]". If variation in class is found, variants can be separated with a slash (`/`), e.g. "_harnāu-_ ~ _harnu-_ [c./n. n]".

The translation of a stem should be given in double-quotes (`"..."`). Multiple senses of the same stem can be given separated by semicolons (`;`), and different expressions of the same sense can be given separated by commas (`,`), e.g. "business, trade; compensation, payment, price".

## Derivatives

The line containing any derivatives of the word in question should begin with the string "Derivatives: ". Derivatives should be given separated by semicolons (`;`), and should be given with a lemma, class, and translation as detailed in the previous section; alternatively, if the derivative exists as an entry, it may be provided simply as a link, whose text is the lemma and a short gloss.

## Cognates or Descendents

If the main entries are for a single exemplar language within a branch (e.g. Latin for Italic, or Hittite for Anatolian), typically because the other languages within the branch are not sufficiently well-attested to allow the branch's common ancestor to be used with certainty, then cognate lemmas from the other languages within the branch can be given in this part of an entry, with a class and translation formatted as detailed in the prior section, and separated by semicolons (`;`) if there are multiple relevant words. The language name (or an abbreviation thereof) should be at the beginning of the line.

Alternatively, if the main entries are for the reconstructed ancestor of the entire branch (e.g. Proto-Germanic or Proto-Celtic, or Proto-Indo-European itself), then the above can be followed except with all the languages within the branch.

## Ancestry

If the etymology of a lemma is known, it should be given as a link to a PIE entry, either for the immediate ancestor, or its derivational base if there is insufficient evidence to reconstruct the derived form for PIE. Additionally, if the lemma is for an exemplar language for its branch, a reconstruction of the branch's ancestor should be given if it can be reconstructed. In some cases only this latter reconstruction can be given, if a word is well-attested within a single branch but cannot be attributed to any PIE word.

## Discussion

The discussion of the word should exposit on important details regarding the form of the lemma, and on difficulties regarding the reconstruction, if there are either. In particular, if there are multiple competing reconstructions then all should be mentioned and appraised, before either giving reasons to prefer some specific reconstruction, or remaining agnostic if none can be accepted. This section should _not_ be a transcription of any source's discussion.

## References

The line containing the references should begin with the string "References: " and contain all the references used in the entry, separated by commas (`,`). References should be linked in end-note style, i.e. `[label]`, with the label defined at the end of the file, as `[label]: link "Title"`. If the reference is to a specific entry in an etymological dictionary, the link should be followed by an escaped colon (`\:`), the page number of the beginning of the entry, and then the lemma as written and formatted (if possible) in the source, e.g. `[EDHIL]\: 233 "_eḫu_"`.
