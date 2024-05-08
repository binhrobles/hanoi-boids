# Hanoi
A packed street Boid simulation.

Boid flocking behavior forked from  [jqlee85/boids](https://github.com/jqlee85/boids) -- this project focused on channeling them through dynamic streets / unique boid behaviors.

## Considerations
- for streets behavior
    - need quick lookup way of understanding street width and direction (?)
    - boids do not want to go off the street
    - concept of "streets" drawn through the canvas
        - boids are instantiated on a street, with valid directions being in a certain direction
        - street intersections become chaotic
    - flock only against boids in MY street
- variability
    - renegades (motos who are going against the grain / disrespect "street" rules)
    - motos vs cars vs trucks (vs peds)
        - prioritization
        - speed / turn radius
        - motos have a tendency to create "streams" for each other
- player
    - different modes: moto / car / truck / ped

## Future
- OSM import -> playable street grid
