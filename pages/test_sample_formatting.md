---
layout: "page"
title: Text Sample Formatting
nav_order: 11
---

# Text Sample Formatting
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

The Receptiviti API does not discriminate between upper- and lower-case letters. It can only count words contained in the LIWC2015 dictionary (the most recent version of LIWC). It it cannot accommodate the following:

- Misspellings

- Colloquialisms

- Foreign words

- Proper names

- Scientific or technical terms

- Most abbreviations

That said, occasional spelling mistakes are less problematic the more words a language sample contains. However, you should take time to correct any consistent misspellings.

## Spelling, Abbreviations, and Contractions

The Receptiviti API accommodates both United States and British English spelling. It can also accommodate common verb contractions including don’t, won’t, isn’t, shouldn’t, can’t, couldn’t, I’m, I’ll, I’d, we’re, we’d, you’re, he’s, and it’s. It will count most others as possessive nouns, as seen in a phrase such as “Sally’s shoes.” In the case of something like “Sally’s going to the store,” the results will be improved when changing “Sally’s” to “Sally is.”

## End-of-Sentence Markers and Hyphens

One of the scores returned from the Receptiviti API is the The Words Per Sentence (WPS) category. It counts the number of times that it detects end-of-sentence markers. These include punctuation such as periods, question marks, and exclamation points. However, common abbreviations (such as Dr., Mrs., U.S.A., D.O.A.) will be counted as multiple sentences unless you remove the periods.

NOTE: _Be careful that the removal of the periods doesn’t inadvertently create a new word. For example, U.S. (the United States) becomes US (first-person plural pronoun) when the periods are removed. In this case, change it to USA_.
{: .label .label-yellow }


When words start or end with hyphens, LIWC2015 interprets the hyphens as part of the word. Whereas LIWC2015 contains the word chit-chat, it would interpret a connected term like this-or-that as three separate words.

## Time Markers

When formatting the time markers a.m. and p.m., we recommend that you remove the space between the number and the marker since LIWC interprets a.m. as the first-person verb am (I am), e.g., 6:30am instead of 6:30 a.m.
