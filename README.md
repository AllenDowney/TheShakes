# The Shakes

A Bayesian dice game for 2-6 players.

by Allen Downey

If you try this game, [please use this survey to tell me what you think](https://forms.gle/NPNSKJ5uv9EvZFRQ7).


## Objective

A deadly disease is sweeping through the Six-Sided Kingdom -- the people call it The Shakes.

The king has summoned a team of maesters to propose treatments for the new disease and put them to the test.

The object of the game is to choose the most effective treatments and save as many patients as possible.


## Equipment 

* Lots of six-sided dice, 

* A deck of cards,

* About 10 tokens of some kind, to keep score.


## Setup

Each player chooses one of the following treatments:

* hot mustard

* dragon peppers

* wine with snake venom

* hot bath

* vegetables

* raw fish

* meat

* blood

* smoke

* wall of fire

No two players can choose the same treatment, but the names of the treatments don't actually affect the outcome, so don't argue about it… yet.

Give one die to each player.  Also:

* If you have 2-3 players, put 12 dice on the table.

* If you have 4 or more players, put 18 dice on the table.

These dice represent the patients you will treat.

Also give one die to each player.


## Efficacy

Each treatment has an efficacy that determines the probability that the patient survives.  For example, if the efficacy of a treatment is 2, it has a 2 in 6 chance of saving the patient.

The efficacies of the treatments depend on the number of players:

* Six players: 4, 2, 2, 2, 1, 1

* Five players: 4, 2, 2, 1, 1

* Four players:  4, 2, 1, 1

* Three players: 4, 1, 1

* Two players: 3, 1

To determine which treatment has which efficacy, select cards from the deck to denote the efficacies.  For example, if there are four players, select a 4, a 2, and two aces.

Shuffle the cards and deal one to each player.  Look at your own card and remember the efficacy of your treatment, but don't tell the other players.

The average efficacy is 2, so if we choose treatments at random, we expect to save 2 out of 6 patients, on average.



## The Argument

During each round of play, a new patient arrives and the maesters argue about what treatment to use.

Maesters are perfectly dogmatic, so each argues in favor of their preferred treatment, regardless of evidence or reason.

Players argue by rolling dice.  The outcome determines the strength of their argument.

Players can argue all at once or one at a time, in any order.

When it is your turn to argue:

1. Roll one die plus one additional die for every patient you have treated.

2. Remove one die for every patient you have saved, starting with the lowest die and working up.

3. Keep the lowest remaining die.  The value of this die is the strength of your argument. 

For example, if you have treated three patients and two survived, you roll 4 dice and remove the lowest 2.

If the results are 1, 2, 2, and 4, you remove the 1 and one of the 2s; the remaining 2 is the strength of your argument.

Once everyone has argued, the maester with the strongest argument treats the patient.

In case of a tie, the maesters with the strongest argument roll again as before, repeating until the tie is broken.


## Treatment

If you won the argument, take a die from the table and roll it.  

If the outcome is less than or equal to the efficacy of your treatment, the patient recovers.  
In that case, take one of the tokens that represents a saved patient.

Keep the die you just rolled so that you always have one die for each patient you have treated, plus the die you started with.


## Winning

With 2 or 3 players, continue until 12 patients have been treated.  The team wins if 5 or more patients survive.

With 4 or more players, continue until 18 patients have been treated.  The team wins if 7 or more patients survive.


## Competitive Variation

In this variation, none of the treatments are effective, but 3 out of 6 patients recover anyway.

Set all efficacies to 3 and play as in the cooperative variation.  

The first player to save 3 patients wins.


## Background

This game demonstrates Bayesian medical testing.  

When a patient arrives, they are assigned a treatment at random, but not with equal probability.
Rather, each treatment is chosen with the probability that it is most effective.
These probabilities are estimated based on past performance: the number of patients treated and the number that recovered.

When the actual efficacy of the treatments is unknown, this strategy is optimal in the sense that it 
maximizes the number of patients saved.

For more information about the strategy, which is call Thompson sampling, see [this Wikipedia page](https://en.wikipedia.org/wiki/Thompson_sampling).

For an explanation of how the game implements the strategy, see [this Jupyter notebook](https://colab.research.google.com/github/AllenDowney/TheShakes/blob/main/shakes.ipynb).


## Credit

The premise of this game is inspired by "the shivers", a disease in George R. R. Martin's *Blood and Fire* (see [here](https://awoiaf.westeros.org/index.php/Shivers)).

Copyright 2020, License: [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)


