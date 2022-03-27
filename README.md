<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->





<!-- ABOUT THE PROJECT -->
## About SCMPlotThreadDemo

This is a demo to demonstrate the concept of using Source Control Management as a way to model plot threads developing in tabletop roleplaying games.

## Threads

The core idea of this system is that a plot is composed of "Threads". These are modelled as git Branches, but for the sake of consistency, they will be referred to as threads. 

A thread is a collection of connected events, usually pertaining to a specific person, place, object, or other topic. The start of a thread can come either through the actions of the players, or can have been set in motion before the start of an adventue, such as part of a historical event. In the case of the latter, a GM could technically make up events chaining all the way back to the beginning of the universe, but for simplicity's sake, often a particularly major event can be considered the start of its own thread.

### Developing Threads.
When something happens that impacts the state of a thread, the thread develops. This can be a result of actions taken by the player, or can be the result of offscreen goings-on.

Threads can develop any number of times, but are NEVER closed. If the players save a village, the village still exists even after they move on to bigger and better things. Further developments could involve the fallout of exactly how they saved the village, or might involve the player's being sent a thank you gift for all that they've done, for example.

In addition, Threads can develop randomly. The chance of doing so greatly decreases as its state becomes more stable, but is NEVER 0. Every so often, a d20 roll is made to see if the Thread develops, and if it does, another D20 roll is made to see how positive or negative this development is.

#### Stability

The roll to see if the thread develops is modified by it's Stability. Stability is a value between -10 and +10, with a -10 being a guarantee that something will happen, but nobody knows what, and a +10 being (practically) a guarantee that nothing unexpected will happen.

After rolling a d20 and adding/subtracting the stability modifier, a result of -1 or lower means that the thread develops. If Stability is +10, then on a roll of of 1 on the die, the thread develops. This is the only case in which a 1 guarantees a thread will develop, and otherwise rolls of 1 or 20 have no special effect on whether a thread develops.

Whether a thread stabilizes or not is independent of its danger, there can be a highly stable thread that balances on a knife's edge between prosperity and ruin, and a highly unstable thread with only good things to come. If the danger of a thread is at a minimum, it might even be better to keep stability low, to cash in on positive developments. And conversely, stabilizing a particularly dangerous threat will, at the very least, mitigate it from getting worse.

#### Danger

If a thread develops, how it develops is based on its Danger. Like Stability, Danger is a value between -20 and 0, with a -20 meaning that any development will be bad. and 0 meaning that any developments will (probably) be good. Unlike Stability, Danger has four different outcomes: (Note that despite the resemblance, this is not 100% equivalent to Pathfinder 2E's 4 degrees of success, in order to make all 4 outcomes have the same range of results)

* Critical Failure (-11 or lower): Disaster has struck. The Dam has broken and the village wil be flooded within minutes. Timmy fell down the well. The lead actor fell and broke their leg and can't perform in the premiere tonight. Whatever the outcome, this warrants an immediate response, or even more disaster will follow.
* Failure (-1 to -10): Something worrying has happened. The inspector has found some critical structural weaknesses in the dam. Timmy is missing and nobody has seen him. The lead actor is uncharacteristically late to rehersal. This outcome may or may not have immediate consequences, but if it isn't addressed quickly there's going to be a very real problem on everyone's hands.
* Success (0-9): Positive progress is being made, or if everything was already going well, the status quo is maintained. We've hired expert masons to fill in the cracks in the dam. Someone heard a child crying down the well and saw Timmy at the bottom. The understudy has been located and has been diligently rehearsing in case something like this happened.
* Critical Success (10+) Everything went better than expected, and everyone is probably celebrating. The masons finished repairing the dam weeks ahead of schedule. Timmy has been rescued from the well. The understudy absolutely killed it at the premiere, and arguably did a better job than the original actor would have done.

### Branching and Merging

Actions do not always have a 1-to-1 correlation. One action can impact many different threads, and many different actions can impact the same thread.

In the case of the former, additional threads are created that branch off the action in question, each of which then has its own title, description, stability, danger, and can develop independently of the original thread.

In the case of the latter, an existing thread is affected by the developments of a completely different thread, possibly altering it drastically. If several different developments would all affect the thread at the same time, the result of thread is the sum of the net changes in all the contributing actions. This can be done by adding up the result of how each thread developed. For example, say you're part of a group projectm today is the due date, and:
1. Paula straight up didn't do her part of the project (-8)
2. You rushed to finish your part in the hour before school started (-2)
3. Kevin has actually been working on his part for about a week (10)
4. Daniel gave it his best shot, but didn't quite get the idea (4)

By adding those all together, we have 10+4-2-8=4, which is ultimately a success overall.

## Demo

In this repository, threads are modelled by text files. The Title of each file briefly describes the thread. First, each file contains at the top a brief description of the current state of the thread, as well as its current Stability and Danger. Below that is a log of actions that were taken that impacted the thread, to provide traceability to how the thread got to where it is.

The examples given in this readme and repository are going to model the events and threads shown in season 1 of Avatar: The Last Airbender. The end of the season is tagged with the current state of the story; tabletop campaigns. can do a similar thing by tagging the end of a book/adventure.

The current state of the files/threads is as they exist at the end of season 1. To view how the threads develop over time, look to the repository's commit history.
