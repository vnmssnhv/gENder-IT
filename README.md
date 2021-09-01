# gENder-IT
- Licensed under the CC BY-NC-ND 3.0 License.
- gENder-IT is an English--Italian challenge set focusing on the resolution of natural gender phenomena by providing word-level gender tags on the English source side and multiple gender alternative translations, where needed, on the Italian target side. 



| Column ID     | Column label  | Explanation  |
| ------------- |:-------------:| ------------:|
| A             | ID            |Sentence ID - Some our sentences have ID's that start with “split” indicating that we split the original MuST-SHE entry into multiple sentences. | 
| B             | ENGLISH       |   English version annotated with tags indicating whether a referent, given the sentential context, is male (\<M\>), female (\<F\>) or ambiguous (\<A\>). If multiple referents are ambiguous, we distinguish between them by using an additional index (\<A1\>, \<A2\>...) |
| C | ONE CORRECT (GENDER) TRANSLATION (original MuST-SHE)      | The Italian translation of sentences that are not ambiguous, i.e. there is only one correct translation in terms of gender. These sentences are identical to the original ones presented in MuST-SHE (Bentivogli et al. 2020)|
| D-M | MULTIPLE CORRECT GENDER TRANSLATIONS      | When a sentence is ambiguous in terms of the gender of a referent and this leads to multiple correct gender translations in Italian, all the possible translations are listed.  |
| N | Number of Alternatives      | Sentences can have 2, 4, 8 … possible translations depending on the amount of ambiguous referents and the Italian translation. The number of alternatives is indicated in this column. |
| O | Type of Alternatives      | A sequence that indicates the gender of the referents in the alternatives. ( see example below)|
| P | Ambiguous Referent      | The final column, indicates which referents in the original English sentences have been disambiguated in the Italian translations. (see example below)| 

 

## EXAMPLE

### Type of Alternatives

For the following English sentence (ID: split it-0239)
 
- English: "Do you \<A1\> remember that patient \<A2\> you sent home?" the other nurse \<A3\> asked matter-of-factly. 

There are 4 correct gender-alternative Italian translations:


- Alternative 1: “Si ricorda quel paziente che ha mandato a casa? " mi ha chiesto l'altro infermiere.

- Alternative 2: “Si ricorda quel paziente che ha mandato a casa? " mi ha chiesto l'altra infermiera.

- Alternative 3: “Si ricorda quella paziente che ha mandato a casa? " mi ha chiesto l'altra infermiera.

- Alternative 4: “Si ricorda quella paziente che ha mandato a casa? " mi ha chiesto l'altro infermiere.

The type of alternative for these sentences is defined as:

- MM - MF - FF - FM

Where:

- MM: refers to the fact that in the first alternative, both ambiguous entities are translated into the male form.

- MF: for the second alternative, the first ambiguous entity is translated into a male form, and the second into the female form.

- FF: in the third alternative, both entities have been translated into the female form.

- FM: the fourth alternative translates the first disambiguated referent into a female form and second into a male form.


### Ambiguous Referents

The ambiguous referents are listed as:

- \<A2\>, \<A3\>

Together with the info on the type of alternatives generated you can infer that
- Alternative 1: the referents \<A2\> and \<A3\> are translated into the male forms.
- Alternative 2: the referent \<A2\> is translated into a male form, while \<A3\> is translated into the female form.
- Alternative 3: the referents \<A2\> and \<A3\> are translated into the female forms.
- Alternative 4: the referent \<A2\> is translated into the female form, while \<A3\> is translated into the male form.
 
 
### When using gENder-IT please cite the following papers:

Vanmassenhove, Eva, and Johanna Monti. "gENder-IT: An Annotated English–Italian Parallel Challenge Set for Cross-Linguistic Natural Gender Phenomena." GeBNLP 2021 (2021): 1.

Bentivogli, Luisa, et al. "Gender in Danger? Evaluating Speech Translation Technology on the MuST-SHE Corpus." Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics. 2020.


### References

Bentivogli, Luisa, et al. "Gender in Danger? Evaluating Speech Translation Technology on the MuST-SHE Corpus." Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics. 2020.

Saunders, Danielle, Rosie Sallis, and Bill Byrne. "Neural Machine Translation Doesn’t Translate Gender Coreference Right Unless You Make It." Proceedings of the Second Workshop on Gender Bias in Natural Language Processing. 2020.

Vanmassenhove, Eva. On the integration of linguistic features into statistical and neural machine translation. Diss. Dublin City University, 2019.

Vanmassenhove, Eva, and Johanna Monti. "gENder-IT: An Annotated English–Italian Parallel Challenge Set for Cross-Linguistic Natural Gender Phenomena." GeBNLP 2021 (2021): 1.
 
