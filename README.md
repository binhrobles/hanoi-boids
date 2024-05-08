# Hanoi
A packed street Boid simulation.

Done for a 24 hour creative code-a-thon at Recurse NGW 2024. Theme: A method to the madness

Boid flocking behavior forked from  [jqlee85/boids](https://github.com/jqlee85/boids)

This project focused on channeling them through dynamic streets / unique boid behaviors.
- Red boids are **Buses**, and they kinda rule the road
- Green boids are **Cars**, whose owners are generally more cautious than other drivers
- White boids are **Motos**, who are highly variable in risk and tend to flocking behavior more than the other types

## Considerations
- for streets behavior
    - need quick lookup way of understanding street width and direction (?)
    - boids do not want to go off the street
    - concept of "streets" drawn through the canvas
        - boids are instantiated on a street, with valid directions being in a certain direction
        - street intersections become chaotic
    - flock only against boids in MY street
- variability
    - motos vs cars vs trucks (vs peds)
        - prioritization
        - speed / turn radius
        - motos have a tendency to create "streams" for each other

## Future
- OSM import -> playable street grid
- get dropped in as a controllable player
    - different modes: moto / car / truck / ped
- renegades (motos who are going against the grain / disrespect "street directionality" rules)
- more interesting
