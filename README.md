# Video Game Project

By: Manuel Oliveira & Bob Kammauff
UVA Mechatronics Sp26

## Goal

Make a dungeon side-scrolling beat-em up starring prof. Momot & prof. Garner exploring a newly formed cave in the basement of the MEB in hopes of rescuing prof. Natasha Smith from the evil prof. Griffiths

## Initial Concept
### Story
As described above. SPOILERS!!: Natasha Smith is actually the villain

### Mechanics
Prof. Momot will be the usual brawler with a sort of dark superman/magneto complex (being able to hover for short periods of time using his Papist Magic). The hope is that Prof. Garner will play as an Olimar/Pikmin-style character by throwing TA's at enemies to fight.

## Deliverables
![ProjectDeliverables.png](MarkdownMedia/ProjectDeliverables.png)

### Plan for completion + Deadlines

1. We need to build the "engine"

I think this should be the goal for friday Mar. 28th and the rough draft: Make a lil tech demo that we can run around in. I've made a mockup of what it could look like:
![GameMockup.png](MarkdownMedia/GameMockup.png)

We need to import the pre-existing sprites that already exist, and then make some placeholder ones (or just go ahead and make them) for the ones we don't have yet. Biggest priorities for the features: 
1. Moving & Jumping in the 2.5D space

    - Use the drop shadows to determine position in the xz plane

2. Animations and actions, Character properties

    - Determine a moveset for Momot.
    - Which buttons for light, heavy attacks
    - Do we have a health bar?

This shpuld help us get started and then we can keep going from there.


I'm basing a lot of my ideas about how the game looks and plays based off of Double Dragon. [Here's](https://youtu.be/NkuB2PWJssY?si=GuOCqAQArytiKDvg) a youtube link for reference.

## Log
3/23/26 - Bob started up the repo and started planning the design of the game. Hopefully can start looking at some code tomorrow.

3/24/26 - Starting on some of the spritework:

![MechBasement](MarkdownMedia/MechBasementReference.jpg)

![MechFloor1](MarkdownMedia/MechFloor1Reference.jpg)

I'm just thinking about the tile sets that I'd need for this.

The floor tiles are going to have the reflection coming off of the fluorescents. One for the first floor, one for the basement

![Floor1](MarkdownMedia/CustomSprites/Floor1%20(1).png)
![Floor1](MarkdownMedia/CustomSprites/Floor1%20(2).png)
![FloorB](MarkdownMedia/CustomSprites/FloorB%20(1).png)
![FloorB](MarkdownMedia/CustomSprites/FloorB%20(2).png)

These can be rotated to get the bottom half of the parallelogram

I ended up going back on the design, so now this is the floor tile:

![Floor.png](MarkdownMedia/CustomSprites/floor.png)

...which can be rotated in order to have it tile effectively!

3/25/26 - Garner Sprites

[Reference for pikmin](https://www.deviantart.com/pikmin789/art/Pikmin-Sprite-Sheet-2-101570656)

I started out by making all of these pikmin sprites!

![pikmin.png](MarkdownMedia/CustomSprites/pikmin.png)

These should cover them walking, attacking, and equipping the fabled monocle

3/27/26 - Another day another dollar, I think. I'll import the log from the other day, but the big thing is that I'm going to try and work smarter this time in order to get the second controller working. Testing frequently and getting it working bit by bit. 

Manuel added a hitbox to the attacking, an hp bar, and now the bullet bill drops a gem that can heal hp. 

I think the first thing I should do is get a second player character loaded up, so I have someone to even control. Time to load in Garner sprites. And then just copy enough code so that his motion is controlled by the first controller. And then work on the second controller integration, working from the controller tester. In fact, maybe I'll just go run that first to make sure both controllers work...

Ok yes they do!! Good.

