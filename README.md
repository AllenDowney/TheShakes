# The Shakes

a game by Allen Downey

Copyright 2020, License: [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

2-6 players, ages 12+

### Objective

A deadly disease is sweeping through the Six-Sided Kingdom -- the people call it The Shakes.

The king has summoned a team of maesters to propose treatments for the new disease and put them to the test.

The object of the game is to choose the most effective treatments and save as many patients as possible.


## Equipment 

* About 10 six-sided dice (sometimes more), 

* A score sheet ([download](https://docs.google.com/document/d/1etO0GQx5NPhdEl3UKsbu50JPhfDieaOHCbmyEH95KA0/copy
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

To determine which treatment has which of these efficacies, each player rolls two dice.  The player with the highest total gets the highest efficacy; the player with the next highest total gets the next highest, etc.  If two or more players are tied, they roll again to break the tie.

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

For example, suppose you have treated three patients and two survived.  You would roll 4 dice.  
Suppose the results are 1, 2, 2, and 4.  You would remove the 1 and one of the 2s, and keep the other 2.

Once everyone has rolled, the player with the highest result gets to treat the patient.


## Treatment

If you won the argument, roll one die.  
If it is less than or equal to the efficacy of your treatment, the patient recovers.  

Add 1 to the number of patients you have treated, and if the patient recovered, add 1 to the number of patients you have saved.


## Winning

With 2 or 3 players, continue until you have treated 12 patients.  You win if you save more than 4 of them.

With 4 or more players, continue until you have treated 18 patients.  You win if you save more than 6 of them.


## Background

This game demonstrates Bayesian medical testing.  When a patient arrives, they are assigned a treatment at random, where the probability of choosing each treatment is the probability that it is most effective, based on past performance.  

When the efficacy of the treatments is unknown, this strategy is optimal in the sense that it maximizes the number of patients saved.

For more information about the strategy, which is call Thompson sampling, see [this Wikipedia page](https://en.wikipedia.org/wiki/Thompson_sampling).

For more information about how the rules of this game implement the strategy, see [this Jupyter notebook]().


## Credit

The premise of this game is inspired by "The Shivers", a disease in George R. R. Martin's *Blood and Fire* (see [here](https://awoiaf.westeros.org/index.php/Shivers)).

