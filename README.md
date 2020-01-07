# PyTorch test script
This originally began as a (slightly altered) run-through of the pytorch recurrent neural network tutorial that can be found at https://pytorch.org/tutorials/intermediate/char_rnn_classification_tutorial.html.

However, upon further reflection, I think that this will serve as a good place to dump a variety of initial pilot scripts for the project. We can add a more formal development repo to the GDD org at a later date.

## Phase I
The first phase was simply to recreate the basic tutorial as is and get it up and running. I made some slight changes to the namespace to make it more case-specific/logical, but otherwise left it mostly unaltered. The test was a success and the basic script can be found in [tutorial.py](/tutorial.py).

This script takes multiple .txt files of different surname and language tuples, stored in the [languages](/languages) subdirectory. It then trains a neural network to "guess" what language a name is.

This tutorial deviates from a proper ML exercise in that there is no separation of the data into *test* and *training* subsets, so there is no real model validation.

## Phase II
I have compiled an excel dictionary of name and categories tuples. The categories are

1. surname (i.e., last names of people in various languages)
2. locality
3. county
4. countries
5. continents
6. units (i.e., names of geologic units/rock bodies)

I want to see if we can use the same basic model to make good guesses as name-type. Obviously, many places, people, and units share the same name - i.e., a place named after a person or a unit named after a nearby town. I suspect that it won't work, but let's give it a try. It's a pretty hefty training set!

## Phase III
Move on to words2vec

## Phase IV
Move on to docs2vec

## Phase V
Move on to neural co-ref
