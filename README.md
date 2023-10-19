# Unity Pathfinding Visualizer

This is a 3D visualizer for pathfinding algorithms, made with Unity and written in C#. It allows you to compare how different algorithms find paths between two points in a dynamic environment that is mapped over using a grid system.

<kbd><img src="https://raw.githubusercontent.com/Oprescu/Unity-Pathfinding-Visualizer/main/Images/Animation.gif" width="750"></kbd>
<kbd><img src="https://raw.githubusercontent.com/Oprescu/Unity-Pathfinding-Visualizer/main/Images/1.png" width="750"></kbd>


## Features

- Three algorithms implemented: Depth-First Search (DFS), Breadth-First Search (BFS), and A* Search (A*).
- Two buttons to randomize the seeker (start) and the target (end) positions.
- A slider to adjust the speed of the visualization.
- A text UI to display the distance of the path found and the time taken to find it.
- The level is composed of rigid bodies can be dragged with your mouse and the pathfinding will work around them.

## Implementation
- A* uses Chebyshev distance as the heuristic function:
$$D_{\text{Chebyshev}}(P,Q) = \max_{i} |p_i - q_i|$$
- Each pathfinding algorithm has it's own implementation class withing the `Assets` folder
- Unity gizmos are used to draw the pathfinding, so make sure they are enabled in the editor or the game view.

## How to use

- Clone this repository
- Open the project folder with Unity using Unity Hub (preferably version 2022.3.11f1).
- Enable Gizmos in game view
- Open the `Test1` or `Test2` scene in the `Assets` folder.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
