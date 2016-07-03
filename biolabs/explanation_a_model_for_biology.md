A Model for Biology
===================

High Level Biological Ontology
-------------------------------

Proteins are comprised of folded up strands of amino acids,
which are translated from RNA, which are transcribed from DNA.

Protein <- amino acid strand <- RNA <- DNA


Proteins are the Actors
-----------------------

Proteins are molecular actors (I'll assume you know what a molecule is,
it shouldn't be too difficult to figure out, if not).
If something is done at the scale of molecules, it's a protein that does it.
If someone uses a verb at this scale, you can assume there is a protein performing the verb.

Proteins are probably the most important thing in biology.
They can work in isolation (float around and do a job) or be combined together
to construct larger things like the wall of a cell.


Proteins are Folded "Polypeptide Strands"
-----------------------------------------

Proteins are made out of amino acids chained together.
The chain of amino acids is called a "polypeptide strand".
The polypeptide strand is not stable, it winds up folding in on itself,
as a string might if you placed it in water.
When it folds in on itself, it winds up in a particular configuration,
due to the forces of chemistry (eg ionic bonding, covalent bonding, hydrogen bonding).
In the same way that a ball, placed on a hill will roll down it,
the strand will wind up folding into a specific low-energy configuration.

The structure that a given polypeptide strand will fold into is not generally known,
humans are good enough pattern matchers to figure it out,
algorithms are not generally good at this yet.


Polypeptide Strands are Chains of Amino Acids
---------------------------------------------

The polypeptide strand is emitted by the protein Ribosome,
as it walks along something called RNA. The sequence of RNA
tells it which amino acids to emit into the strand.

As it traverses the RNA, other proteins will bring it the
building blocks that it needs to make the amino acids.


RNA is a Sequence of Nucleotides
--------------------------------

Like the polypeptide strand, RNA is a sequence (I think the chemical term for this is "polymer").
Instead of amino acids, it holds "nucleotides".
The nucleotides are one of the molecules guanine, uracil, adenine, and cytosine,
In RNA, these are abbreviated to just "G", "U", "A" and "C".
So RNA might look like "GUACAGAGACAUUAAACG".

When Ribosome walks along the RNA, to make amino acids for the polypeptide strand,
it looks at the nucleotides 3 at a time. So our RNA would be broken up like this:
"GUA-CAG-AGA-CAU-UAA-ACG". These groups of 3 nucleotides are called a codon.

Each codon has a [specific meaning](https://en.wikipedia.org/wiki/Genetic_code),
our first codon, "GUA" means to emit the amino acid Valine.
Our second, "CAG" means to emit the amino acid Glutamine.
Our second to last, "UAA" means to stop translating codons into Amino Acids,
so it wouldn't look at the last codon "ACG".


RNA is Transcribed From DNA
---------------------------

Like RNA, DNA is a sequence of nucleotides.
It shares the same set of nucleotides, except instead of uracil ("U"),
it has thymine ("T").

RNA's GUAC are "transcribed" from DNA's GTAC by a protein called "RNA Polymerase".
You can remember this, because it's making RNA, which is a polymer (a sequence of
molecules). The suffix "ase" is attached to certain types of proteins called enzymes.
So RNA Polymerase is an enzyme (type of protein) that makes the RNA polymer.
The rate of transcription is modulated by another protein called a "transcription factor".

```
So our RNA sequence:               GUA-CAG-AGA-CAU-UAA-ACG
Would come from this DNA sequence: GTA-CAG-AGA-CAT-TAA-ACG
```

Note that I broke the sequence into codons to make it easier to read,
but I don't think there is anything physically present in the RNA or DNA
which corresponds to this (I think it's the structure of the Ribosome).


DNA is in the Nucleus, RNA Takes the Information to the Cytoplasm
-----------------------------------------------------------------

Since the RNA is just an intermediate step between the DNA and
the polypeptide strand, why have it at all? The reason is because
the Ribosome, which makes the polypeptide strand, is in the cell's
cytoplasm, outside the nucleus. But the DNA is stored inside the
nucleus where there is better protection.

The DNA can't go through the nucleus' membrane, but the RNA can.
Thus the RNA transports the information to the Ribosome so that
it can be synthesized into a protein.


DNA's Nucleotide Sequences (GTAC) are Paired
--------------------------------------------

Each nucleotide can pair with another nucleotide.
The A pairs with T.
The G pairs with C.
So a strand of DNA will usually have an adjacent strand of paired DNA
From our previous example, then, the DNA would look like this:

```
G-T-A-C-A-G-A-G-A-C-A-T-T-A-A-A-C-G
| | | | | | | | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
C-A-T-G-T-C-T-C-T-G-T-A-A-T-T-T-G-C
```

So our first "G" in the top sequence is paired with the first "C" in the bottom sequence.

The RNA that RNA Polymerase transcribes it into, on the other hand, would not be paired.
This is one of the reasons RNA can get through the wall of the nucleus, it's just smaller.
It would look like this:

```
G-U-A-C-A-G-A-G-A-C-A-U-U-A-A-A-C-G
```


If you have one side of DNA or RNA, you have both sides
-------------------------------------------------------

Because A always pairs with T and C always pairs with G,
you can infer either side of the from the other.
That is, in fact, how I made the above sequence,
I randomly typed letters for a bit, then I matched them
with their appropriate pairs.


DNA is Double Helixed (in Humans, at Least)
-------------------------------------------

In humans, the ladder looking DNA structure actually twists around itself,
this is called a "double helix".
So our above example would actually look more like this:

```
G-T-A.   .C-T-C.   .A-T-T.   .T-G-C
| | | C.T | | | T.C | | | A.T | | |
| | | G'A | | | A'G | | | T'A | | |
C-A-T'   'G-A-G'   'T-A-A'   'A-C-G
```


Human DNA is Very Long
----------------------

Human DNA comes in a big long strand, like 3 billion base pairs.
Only a portion of that is transcribed into RNA, so the RNA is much
shorter, another reason that RNA can leave the nucleus and get to the Ribosome.


Human DNA is Wound Up Into 23 Chromosome Pairs
----------------------------------------------

While it is very long, it is wound up tightly, we call the wound structure a "chromosome".
Chromosomes come in pairs, and we have 23 of them.

To make the RNA, RNA Polymerase loosens the DNA from the chromosome
and cuts down the middle of the ladder to separate the base pairs.
It then traverses the DNA to transcribe each nucleotide.
And finally, it seals the base pairs back up.

This massive chromosomal structure is what prevents it from leaving the nucleus,
RNA, however, is just a single nucleotide strand.

Summary
-------

So Proteins are folded polypeptide strands,<br />
Which are amino acids linked together,<br />
Which are created based on the sequence of RNA nucleotides,<br />
Which are created based on the sequence of DNA nucleotides.

DNA, then, is a specification for building proteins.


Reverse Summary
---------------

DNA stays in the nucleus where it is safer.
To work with it, it gets transcribed into RNA,
which allows it to get out of the nucleus and into the cytoplasm.
Once there, the RNA is translated, a codon (3 nucleotides) at a time,
into a polypeptide strand. The polypeptide strand folds into a stabler structure,
which is the structure of our protein.

These proteins can then go do whatever they do, eg if it was an RNA Polymerase,
then it could go transcribe DNA into RNA, continuing the cycle that created it.


Resources
---------

* Chart of codons https://en.wikipedia.org/wiki/Genetic_code
* Absolutely wonderful SVGs showing protein synthesis
  * https://en.wikipedia.org/wiki/Protein_synthesis
  * https://en.wikipedia.org/wiki/Protein_biosynthesis