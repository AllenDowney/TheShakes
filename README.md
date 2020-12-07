# The Shakes

A Bayesian dice game for 2-6 players.

by Allen Downey

Copyright 2020, License: [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)


## Objective

A deadly disease is sweeping through the Six-Sided Kingdom -- the people call it The Shakes.

The king has summoned a team of maesters to propose treatments for the new disease and put them to the test.

The object of the game is to choose the most effective treatments and save as many patients as possible.


## Equipment 

* About 10 six-sided dice, 

* A score sheet ([download here](https://docs.google.com/document/d/1etO0GQx5NPhdEl3UKsbu50JPhfDieaOHCbmyEH95KA0/copy
)).  You can print a copy or edit it on screen.


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

On the score sheet, write the name of each player and the treatment each one chose.


## Efficacy

Each treatment has an efficacy that determines the probability that the patient survives.  For example, if the efficacy of a treatment is 2, it has a 2 in 6 chance of saving the patient.

The efficacies of the treatments depend on the number of players:

* Six players: 4, 2, 2, 2, 1, 1

* Five players: 4, 2, 2, 1, 1

* Four players:  4, 2, 1, 1

* Three players: 4, 1, 1

* Two players: 3, 1

To determine which treatment has which of these efficacies, each player rolls two dice.  The player with the highest total gets the highest efficacy; the player with the next highest total gets the next highest, and so on.  If two or more players are tied, they roll again to break the tie.

For each treatment, write its efficacy on the score sheet.

The average efficacy is 2, so if we choose treatments at random, we expect to save 2 out of 6 patients, on average.


## The Argument  

Each time a patient arrives, the maesters argue about what treatment to use.  
Maesters are perfectly dogmatic, so each of them always argues in favor of their preferred treatment, regardless of evidence or reason.

Each player rolls dice to determine the strength of their argument; the player with the strongest argument gets to treat the patient.

When it is your turn to argue:

1. Roll one die plus one additional die for every patient you have treated.

2. Remove one die for every patient you have saved, starting with the lowest die and working up.

3. Keep the lowest remaining die.

For example, suppose you have treated three patients and two survived.  You roll 4 dice.

If the results are 1, 2, 2, and 4, you remove the 1 and one of the 2s, and keep the other 2.

Once everyone has rolled, the player with the highest result gets to treat the patient.

In case of a tie, the maesters with the strongest argument roll again as before, repeating until the tie is broken.


## Treatment

If you won the argument, roll one die.  

If it is less than or equal to the efficacy of your treatment, the patient recovers.  

Add 1 to the number of patients you have treated, and if the patient recovered, add 1 to the number of patients you have saved.

You might find it convenient to use tally marks.


## Winning

With 2 or 3 players, continue until 12 patients have been treated.  The team wins if 5 or more patients survive.

With 4 or more players, continue until 18 patients have been treated.  The team wins if 7 or more patients survive.


## Competitive Variation

It turns out that none of the treatments are effective, but 2 out of 6 patients recover, regardless of treatment.

Set all efficacies to 2 and play as in the cooperative variation.  

The first player to save 4 patients wins.


## Background

This game demonstrates Bayesian medical testing.  

When a patient arrives, they are assigned a treatment at random, but not with equal probability.

Rather, each treatment is chosen with the probability, based on past performance, that it is most effective.  

When the efficacy of the treatments is unknown, this strategy is optimal in the sense that it maximizes the number of patients saved.

For more information about the strategy, which is call Thompson sampling, see [this Wikipedia page](https://en.wikipedia.org/wiki/Thompson_sampling).

For more information about how the rules of this game implement the strategy, see [this Jupyter notebook](https://colab.research.google.com/github/AllenDowney/TheShakes/blob/main/shakes.ipynb).


## Credit

The premise of this game is inspired by "The Shivers", a disease in George R. R. Martin's *Blood and Fire* (see [here](https://awoiaf.westeros.org/index.php/Shivers)).

