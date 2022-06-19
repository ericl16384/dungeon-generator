# dungeon-generator
My attempt to generate 2D dungeons, like in this video: https://youtu.be/rBY2Dzej03A

### pathing.html
First, I generalized my A* algorithm to be more useful to this project.

### triangulation.html
I learned how to create a Delaunay triangulation, which took longer than it should have.

### stuffedDungeon.html
The first dungeon generator, which pathfinds every connection between rooms recorded on the Delaunay triangulation.

### dungeonExplorer.html
Configurable generator, to which I plan to add settings in the html for users. Not finished.

## TODO
[2D algo description](https://youtu.be/rBY2Dzej03A)
 - [x] Place rooms
 - [x] Delaunay triangulation of room centers
   - Bowyer-Watson algorithm
 - [ ] Minimum spanning tree
   - Prim's algorithm
 - [ ] Randomly choose edges
   - 12.5% chance?
 - [x] Pathfind hallways
   - Cheaper to use existing hallways (20% cost?)
   - Existing rooms have increased cost (200%?)
   - Connect to doors, or to the nearest point on the edge?

Reduce the number of connections, via creating a MST of the connections, but keep a few extra for variety. If the Delaunay triangulation works so well by itself, maybe I don't need this. I could reduce complexity by only creating an MST, but it might be hard to add the extra connections.
