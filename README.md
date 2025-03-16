# Self-Similar Melodies

This repository contains implementations in Python and,
where possible,
in [PureData](https://puredata.info/),
of [Tom Johnson’s](https://en.wikipedia.org/wiki/Tom_Johnson_(composer)) algorithms as presented in _Self-Similar Melodies_ (Editions 75,
Paris 1996).
I strongly recommend reading the book,
because of Johnson’s straightforward and friendly manner.
However,
as a book written almost thirty years ago,
the technical implementation is sparse (and limited to BASIC),
so I am attempting to recreate the algorithms here.

Johnson has 24 chapters grouped into four sections: counting,
transforming,
mapping,
and self-replicating.
All of these provide techniques for generating [self-similar](https://en.wikipedia.org/wiki/Self-similarity) patterns.
For Johnson,
these are typically patterns of integers,
which are later mapped to pitches,
durations,
or rests.
I’m starting this project with making four Python notebooks,
in `notebooks/`,
where each is devoted to one of these groups.
Next steps include turning these into PureData abstractions or sub-patches.
I’m starting with the Python notebooks because I know Python better but also since on day one of this project I was already stumped on how to implement something in Pd.
Once I have the Python logic down,
porting will hopefully be easier.

To avoid simply copying Johnson’s work,
the algorithms are provided without any discussion or fanfare beyond a signature and an example with a page number,
taken from the book.
The return value of every function will always be a list of integers,
which can be saved to a text file for reading into a table in Pd. I hope to stick to this requirement, but I worry that it may harm the ability to work recursively.
