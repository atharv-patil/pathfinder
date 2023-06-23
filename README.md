# PathFinder
<img src="https://github.com/atharv-patil/pathfinder/assets/83455141/563df622-0de2-4242-b47b-ec433bdafcdb"  width="300" height="300">

## Collaborators
Atharv Patil - [github.com/atharv-patil](https://github.com/atharv-patil)<br>
Utkarsh Shukla - [github.com/utkarshukla7](https://github.com/utkarshukla7)
## Description

PathFinder is a Python application designed to provide efficient route planning for bus transportation. By leveraging the A* algorithm and bus stop coordinates from Pune Mahanagar Parivahan Mahamandal Ltd open transit data, PathFinder calculates the optimal path between two points. The application extracts bus stop coordinates, generates a distance matrix using the haversine formula, and applies the A* algorithm to explore the graph-like structure created from the distance matrix. Through an iterative process, PathFinder intelligently narrows down the search space and identifies the most efficient route, considering both the distance to the goal and the cost incurred so far. The resulting route is presented as a list of bus stop identifiers, allowing transportation planners and commuters to optimize bus travel, reduce time, and enhance the overall efficiency of bus transportation.

In addition to route planning, PathFinder offers a visual representation of the recommended route. Using the folium library, the application generates a map where the bus stops along the path are marked as red circles. This visual representation provides an intuitive and clear understanding of the suggested route. PathFinder can be a valuable tool for transportation planners, commuters, and individuals involved in optimizing bus routes, contributing to improved travel experiences, reduced commute times, and enhanced overall efficiency in the realm of bus transportation.
## Usage
To use PathFinder, follow the steps below:

1. Download the bus stop data from Pune Mahanagar Parivahan Mahamandal Ltd open transit data.
2. Make sure you have the following dependencies installed:
   - pandas
   - numpy
   - haversine
   - folium
   - geopy
3. Save the bus stop data in a file named "stops.txt" in the project directory.
4. Run the provided code to generate the optimal path between two bus stops.
5. Review the output to obtain the route details.

## Code Explanation
1. The code reads the bus stop data from the "stops.txt" file and stores it in a pandas DataFrame.
2. The bus stops' coordinates are extracted from the DataFrame and stored in a list.
3. A distance matrix is created using the haversine formula to calculate the distance between each pair of bus stops.
4. The distance matrix is saved to a file named "DistanceMatrix.txt".
5. The A* algorithm is used to find the optimal path between the specified start and end bus stops.
6. The route data is processed to determine the stops and connections made along the route.
7. The output is visualized on a map using the folium library, with the bus stops marked as red circles.

## Example Output
An example output of PathFinder is a list of bus stops representing the optimal route between two points.

```
Route: [33884, 33589, 32994, 32868]
```

## Screenshots
![image](https://github.com/atharv-patil/pathfinder/assets/83455141/22f88985-fa25-4403-b574-4ae1b7a4280f)
![image](https://github.com/atharv-patil/pathfinder/assets/83455141/839decdc-a5c5-476e-8fb2-7f4c14cd4951)
![image](https://github.com/atharv-patil/pathfinder/assets/83455141/5e249236-2d4e-4f38-9a69-411d05684bde)



## Acknowledgments
- Pune Mahanagar Parivahan Mahamandal Ltd for providing the open transit data.
- The haversine library for calculating distances between coordinates.
