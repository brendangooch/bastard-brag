# bastard-brag

a mobile-first, web-based, *single player* vs *computer* game based on a seemingly simple yet addictive poker-style card game played by myself and my friends.

## the game

The **game** is played with a full **deck** of 52 standard **playing cards**.  Each **player** starts with an agreed number of **lives**.  The **game** consists of **rounds** and at the end of each **round** the **player** or **players** with the worst **hand** *loses* a *life*.  The aim of the **game** is therefore to preserve one's **lives**.  The last **player** standing wins and the **game** ends.

Any number of **jokers** can be added to the **deck** (usually 0-2) and act as *wild* cards representing any value that the **player** holding the **joker** chooses.  In reality this *always* means the **card** that enables the **player** to make the strongest **hand** possible.

At the start of the **game** the **playing cards** are *dealt* (by any player), one at a time, to each **player** until a **player** receives either a **jack** or a **joker**.  That player becomes **dealer** and play beings.  The **dealer** deals 3 **cards** face down to each **player** and 3 **cards** in the middle of the table, 2 of which are face up and 1 face down.  One interesting quirk is that the **cards** can be *dealt* in *any* order the **dealer** chooses.  At the end of each **round** the **player** to the left of the current **dealer** becomes the new **dealer** and the next **round** begins.

After the **cards** are *dealt*, the **round** begins and the **player** to the left of the **dealer** plays their **turn**.  **Players** have 3 choices when it's their **turn**.  Normally a **player** selects one of the **cards** in their **hand** and *swaps* it with a **card** in the middle of the table.  Under certain circumstances it may be beneficial to *swap all 3* **cards** with the **cards** in the middle, which is the *second* option.  

The third move a **player** can make is to *knock*.  A **player** can only *knock* if nobody else has already *knocked* and *not* on the first round.  Once a **player** has *knocked*, each other **player** proceeds to play their **turn** as normal, during which they ***MUST*** *swap* 1 or all 3 of their **cards**.  Once every **player** has had a final turn the **players** turn over their hands and the **player** or **players** with the lowest scoring **hand** loses a **life**.

The hands resemble traditional poker hands, with a couple of minor differences and caveats.  If you know how poker hands are scored you will understand how Bastard Brag hands are scored.  The lowest possible hand is a pair of 2s and the highest possible hand is triple 3s.  When 2 players have the same type of hand, the hand with the higher card values ranks higher.  I.e. a pair of 9s beats a pair of 6s, triple aces beats triple kings, queen high flush beats jack high flush, 6,7,8 beats 5,6,7 and so on.

types of hand (weakest to strongest):

  - PAIR (2 cards with the same **value**)
  - FLUSH (3 cards of the same **suit**)
  - STRAIGHT (3 cards with **values** in a sequenital row i.e. 4,5,6 but not of the same **suit**)
  - STRAIGHT FLUSH (a STRAIGHT where the cards all have the same **suit**)
  - 3 OF A KIND (3 cards with the same **value**)
  - TRIPLE 3s (3 cards with the **value** 3) [a devastating hand!]

That's it in a nutshell but there are a few interesting caveats to bear in mind:

  - jokers
    - as stated above, jokers can represent any card value in a hand
   
  - 3 of a kind
    - if a player has 3 cards of the same value 'aka trips' EVERY other player loses a life
    
  - triple 3s
    - if a player has triple 3s in their hand every player loses TWO lives.
 
  - knock and lose
    - if the player who knocks ends up with the weakest hand that player loses TWO lives
    - if a player has trips (3 of a kind) the player who knocked loses TWO lives
    - if a player has triple 3s in their hand, the player who knocked loses THREE lives

  - aces
    - aces can be counted as HIGH or LOW


## the app (v0.0.1)

The plan is to write the MVP in vanilla javascript and deploy somewhere for free, share the link amongst friends, and add features/debug based on their feedback.  If the interest is there, we'll incorporate a host of front end libraries and tools and structure the project more appropriately before starting to look at creating a back end for the application.  I have heaps of ideas for new features but want to get a working demo online as quickly as possible.  

## demo

*A link to an online demo will be added here as soon as the MVP is deployed*.  Play the demo a few times and you'll soon learn why it's called *bastard* brag.

My main interest in the project is in programming the AI of the computer players.  It is, after all, an opportunity to prove beyond any doubt that I am the best Bastard Brag player amongst my friends :)
