# Some Pig

## Description

Use Monte Carlo simulations to find the ultimate player of Pig Solitaire.

## Objectives

### Learning Objectives

After completing this assignment, you should understand:

* Modeling games and simulations

### Performance Objectives

After completing this assignment, you should be able to:

* Play Pig well
* Use subclasses
* Create Monte Carlo simulations

## Details

### Deliverables

* A Git repo called some-pig containing at least:
  * an IPython notebook
  * a `requirements.txt` file

### Requirements  

* At least 5 different charts

## The Rules of Pig Solitaire

In 7 turns, you are attempting to get the highest score possible.

Each turn, you have two choices:

* __Roll__. Roll a six-sided die. If it comes up one, your turn is over and
  you add nothing to your score. If it comes up two through six, you add that
  number to your turn total and choose again.
* __Hold__. If you hold, you add the turn total to your score.

An example:

    The first turn, I roll a 1 immediately. I receive no points.

    The second turn, I roll a 5. I choose to roll again. I roll a 3, for a
    turn total of 8. I choose to roll again. I roll a 3, for a turn total of
    11. I hold, receiving 11 points. My score is 11.

    The third turn, I roll a 5 again. I choose to roll again. I roll a 6, for
    a turn total of 11. I choose to roll again. I roll a 4, for a turn total of
    15. I decide to roll once more. I roll a 6, for a turn total of 21. I hold,
    receiving 21 points. My score is 32.

    The fourth turn, I roll a 6. I choose to roll again. I roll a 3, for a
    turn total of 9. I choose to roll again. I roll a 3, for a turn total of
    12. I choose to roll again. I roll a 4, for a turn total of 16. I hold,
    receiving 16 points. My score is 48.

    The fifth turn, I roll a 6. I choose to roll again. I roll a 6, for a turn
    total of 12. I choose to roll again. I roll a 3, for a turn total of 15. I
    choose to roll again. I roll a 4, for a turn total of 19. I choose to roll
    again. I roll a 6, for a turn total of 25. I hold, receiving 25 points. My
    score is 73.

    The sixth turn, I roll a 6. I choose to roll again. I roll a 1, and
    receive no points.

    The seventh turn, I roll a 5. I choose to roll again. I roll a 1, and
    receive no points.

    My final score is 73.

## Normal Mode

Create a simulation of different types of players of Pig Solitaire. You should
have a base Player class that only rolls once per turn. Then create Player
subclasses -- at least 2 -- that have different strategies. Create charts
showing how they do in a large number of trials. Attempt to create an optimal
player and back up your assertion with charts and data.

Your classes, findings, and charts should be in an IPython notebook.

## Hard Mode

In addition to the requirements from **Normal Mode**:

Once you have your optimal Pig Solitaire player, create a second simulation.
This could be in a separate notebook or the same one. This simulation will
be of the game of Pig. Pig works like Pig Solitaire, but you play against
another person, and are trying to be the first to score 100 points. There is
no round limit.

Create a new type of player for Pig. Your new player should play against the
strategy as your optimal Pig Solitaire player. (You will probably have a new
class for your optimal Pig Solitaire player, as playing Pig will need the class
to take in more data each turn.) Try to create an optimal competitive Pig
player, when the opponent is your optimal Pig Solitaire player. Back up your
assertions with charts and data.

## Additional Resources

* [Demonstration of how to give game state to simulated players](http://nbviewer.ipython.org/gist/cndreisbach/c2bad3de531e2b6122a9#)
