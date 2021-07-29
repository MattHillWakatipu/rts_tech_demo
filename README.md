# COMP313 - Matthew Hill - Assignment 1 - rts_tech_demo
Link to video showing the prototype/game ( approx. 4-9 mins )

## Behaviour Trees
Behaviour trees originated from the video game industry, as a tool to model the behaviour of NPCs but have since been used in other areas such as robotics. They are represented by a directed acyclic graph comprised of control flow nodes and execution nodes. The execution nodes are leaf nodes which simply define a task to complete, whereas the control flow nodes control which of its children should execute. Although this model is simple, it can create very complex behaviour.

## Support in Unreal
Unreal has extremely good support for behaviour trees as it supports them natively through the Behaviour Tree and Blackboard blueprints. These blueprints are both easy to modify and change, and easy to add to different actors in the world through the AI controller blueprint.

## Implementation challenges
The hardest part of implementing this technology was not the behaviour trees themselves, although I did have some difficulty with smoothly integrating animations for tasks, but the sheer amount of required code before being able to implement them. Due to the lack of RTS templates I chose to work from an empty project, which meant that before I could start implementing behaviour trees, I needed to create camera controls, unit selection tools, buildings, user interfaces, units, resources and many other objects.

## Use in existing games
Behaviour trees are a common way of implementing game AI and are often used to control NPC's. Their discrete nature, essentially mimicking finite state machines but modelled over tasks instead of states, means that they are aptly suited to performing complex behaviours. For example, Just Cause 3 utilised behaviour trees for their NPC AI, which led to some incredibly complex behaviour trees, as they needed to account for many different situations. Due to the chaotic and unpredictable nature of the open world game Just Cause 3, it necessitates having AI which is both intelligent enough to promote suspension of disbelief and flexible enough that it can handle many different situations.

Source: https://youtu.be/SurYVTMINhg

## How could this be used in future games?
While behaviour trees are used prolifically and will always be very useful for creating simple AI which always behaves in a specific manner, the evolution of the artificial intelligence field may see complex behaviour trees being replaced by other, more cutting-edge technologies. Perhaps one of the ways in which we may see AIs evolve to be more dynamic, complex and human-like would instead be to model them as optimizers or satisficers with a utility function. However, even if game AI does tend towards a different path, behaviour trees would likely still have a place due to their simplicity and predictability, for example the AI for a patrolling quest giver in an RPG would be well suited for a behaviour tree as it may be more important that the NPC is predictable rather than realistic.
