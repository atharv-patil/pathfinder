# PathFinder

## Description
PathFinder is a Python application that utilizes the A* algorithm to find the optimal path between two points using bus stop coordinates provided by Pune Mahanagar Parivahan Mahamandal Ltd open transit data. It calculates the Euclidean distance between bus stops as the heuristic to guide the search for the shortest path.

## Usage
To use PathFinder, follow the steps below:

1. Download the bus stop data from Pune Mahanagar Parivahan Mahamandal Ltd open transit data.
2. Make sure you have the following dependencies installed:
   - pandas
   - numpy
   - haversine
   - googletrans
   - requests
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
![Bus Route Map](screenshot.png)

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- Pune Mahanagar Parivahan Mahamandal Ltd for providing the open transit data.
- The haversine library for calculating distances between coordinates.

Please note that this is a simplified README file, and you may need to provide more details, such as installation instructions, usage examples, and additional features, depending on the complexity and requirements of your project.
