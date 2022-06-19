# dungeon-generator
My attempt to generate 2D dungeons, like in this video: https://youtu.be/rBY2Dzej03A

### pathing.html
First, I generalized my A* algorithm to be more useful to this project.

### triangulation.html
I learned how to create a Delaunay triangulation, which took longer than it should have.

### stuffedDungeon.html
The first dungeon generator, which pathfinds every connection between rooms recorded on the Delaunay triangulation.

## TODO
Reduce the number of connections, via creating a MST of the connections, but keep a few extra for variety. If the Delaunay triangulation works so well by itself, maybe I don't need this. I could reduce complexity by only creating an MST, but it might be hard to add the extra connections.
