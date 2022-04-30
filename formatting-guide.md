# Formatting Guide

This file will describe in detail the suggested format for entries in the dictionary files. If you think a change should be made, write up a number of sample entries in both the old and new formats and show them to Kat, along with an explanation of why this is an improvement.

## Overall Layout

The overall layout of an entry is as follows:
```
lemma [class] "translation"
Derivatives:
- derivative
- ...
Descendants:
- Lang lemma [class] "translation"; ...
- ...
Cognates:
- Lang lemma [class] "translation"; ...
- ...
Etymology:
- etymology
- ...
Discussion: ...
References: reference, ...
```

## Lemma, Class, and Translation

The lemma should be given in some standardised form, though this may vary from language to language. If multiple paradigmatic stems need to be given, they should be separated by a tilde (`~`), e.g. "arai- ~ ari-". Alternating segments should be separated by a slash (`/`), e.g. "hame/ink", and optional segments should be enclosed in brackets (`(...)`), e.g. "as(sa)nu-". Any other set of alternate forms, including multiple paradigms, should be separated by commas (`,`), e.g. "ark-, ārk- ~ ark-". If the lemma is for a reconstructed language, it should be prefixed by an asterisk (`*`).

The class of a stem or paradigm should be given immediately after the form(s), and should include both information about the part of speech, and which inflection type the stem falls into, e.g. "apā- ~ apū- [pron]", "harsi- ~ harsai- [c. n]". If there are multiple stems or paradigms of different classes, each one should be marked with its own class, e.g. "hās- ~ hass- [i v], hēs- ~ hess- [zi v]". If variation in class is found, variants can be separated with a slash (`/`), e.g. "harnāu- ~ harnu- [c./n. n]". Uncertainty in class assignment should be indicated with a question mark (`?`), e.g. "akutalla- [? n]".

The translation of a stem should be given in double-quotes (`"..."`). Multiple senses of the same stem can be given separated by semicolons (`;`), and different expressions of the same sense can be given separated by commas (`,`), e.g. "business, trade; compensation, payment, price". Uncertainty in translation should be indicated with a question mark in brackets (`(?)`), e.g. "hallanna/i- [i v] "to trample down(?)"", unless the translation is entirely unknown, in which case the translation should be given as a question mark, e.g. "antaka- [? n] "?"". Morphemes expressing grammatical information should have their translation contained in markup indicating italics, e.g. "-an₁ [suff] "$i{dir.sg. ending of a-stems}"".

## Derivatives

If the word has any derivatives, they should be listed one derivative per line, with each line starting with "- ". Each derivative should be its own entry, linked to by a special markup tag. Its format is `@word[LANG lemma]`. `LANG` is a short (3-5 characters) code in all-caps referring to the language, while `lemma` is the chosen citation form of the word. Homonyms should be disambiguated by including a subscript numeral. Class and translation do not need to be provided with a link, as when the presentation forms of the dictionaries are generated, they will be inserted automatically.

## Cognates and Descendants

If the main entries are for a single exemplar language within a branch (e.g. Latin for Italic, or Hittite for Anatolian), typically because the other languages within the branch are not sufficiently well-attested to allow the branch's common ancestor to be used with certainty, then cognate lemmas from the other languages within the branch can be given in this part of an entry, with a class and translation formatted as detailed in the prior section, and separated by semicolons (`;`) if there are multiple relevant words. The language name (or an abbreviation thereof) should be at the beginning of the line. If the class or translation match those of the entry, then they can be left out.

Alternatively, if the main entries are for the reconstructed ancestor of the entire branch (e.g. Proto-Germanic or Proto-Celtic, or Proto-Indo-European itself), then the above can be followed except with all the languages within the branch.

## Etymology

For a derived word, the etymology should be given on its own line, beginning with "- ", linking to the derivational base using the same markup as in the derivatives section. For an underived word, if the etymology is known, it should be given as a link to a PIE entry, either for the immediate ancestor, or its derivational base if there is insufficient evidence to reconstruct the derived form for PIE. Additionally, if the lemma is for an exemplar language for its branch, a reconstruction of the branch's ancestor should be given if it can be reconstructed. In some cases only this latter reconstruction can be given, if a word is well-attested within a single branch but cannot be attributed to any PIE word. If both the immediate ancestor and PIE ancestor can be listed, they should appear on separate lines beginning with "- ".

## Discussion

The discussion of the word should exposit on important details regarding the form of the lemma, and on difficulties regarding the reconstruction, if there are either. In particular, if there are multiple competing reconstructions then all should be mentioned and appraised, before either giving reasons to prefer some specific reconstruction, or remaining agnostic if none can be accepted. This section should _not_ be a transcription of any source's discussion.

## References

The line containing the references should begin with the string "References: " and contain all the references used in the entry, separated by commas (`,`). References should be given in one of two formats: first, with the author's name (always surname, with first initial if necessary to disambiguate) and the year of publication (along with a letter to disambiguate if there are multiple cited publications in a single year); second, as an abbreviation for the paper's title. This latter method should only be used for highly cited major works, such as older etymological dictionaries. If the reference is to a specific portion of the text (mostly relevant for longer works) then the relevant page number or range can be given after a colon (e.g. "EDHIL: 273"). If the reference is to a specific entry in an etymological dictionary, the lemma should be cited as written in source, using markup as necessary to achieve the same formatting used, e.g. "EDHIL: 273 "$word{ḫalii̯e/a-$sup{zi}}"".
