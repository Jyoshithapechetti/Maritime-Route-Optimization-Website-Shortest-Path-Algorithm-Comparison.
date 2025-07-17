# Maritime Route Optimization Web Application

This project presents a web-based application designed to optimize maritime transport routes in the Indian subcontinent. It compares the performance of three shortest path algorithms: **Dijkstra’s Algorithm**, **A\*** Algorithm, and **Bellman-Ford Algorithm**. The application uses real-world geospatial and oceanographic data to compute and visualize optimal routes between ports.

---

## Features

* Displays interactive maritime maps with port-to-port routing
* Implements and compares three shortest path algorithms:

  * Dijkstra’s Algorithm
  * A\* Algorithm (heuristic-based)
  * Bellman-Ford Algorithm (supports negative weights)
* Computes and compares time and memory usage for each algorithm
* Provides visualizations through dynamic graphs and route maps
* Integrates real-world oceanographic data from CMEMS (Copernicus Marine Environment Monitoring Service)

---

## Technology Stack

**Backend**:

* Python (Flask)

**Libraries Used**:

* NetworkX: Graph representation and pathfinding algorithms
* GeoPandas, Shapely: Processing GeoJSON and spatial data
* Plotly: Data visualization
* psutil: Memory tracking
* xarray, ftplib: Oceanographic data handling

**Frontend**:

* HTML templates rendered by Flask
* Folium for interactive maps

---

## Installation and Setup

1. Clone the repository:

   ```
   git clone https://github.com/your-username/maritime-route-optimizer.git
   cd maritime-route-optimizer
   ```

2. Install the dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Run the application:

   ```
   python app.py
   ```

4. Open your browser and go to `http://localhost:5000`.

---

## Application Workflow

1. The user selects source and destination ports through the interface.
2. GeoJSON and oceanographic data are processed to build a weighted graph.
3. The selected algorithms compute optimal paths based on distance, time, and memory.
4. The application displays the route on a map and provides comparison charts for performance evaluation.

---

## Evaluation Summary

* **A\*** algorithm performed fastest in terms of execution time.
* **Dijkstra’s algorithm** was the most efficient in terms of memory usage.
* **Bellman-Ford algorithm** was the most flexible for handling graphs with negative weights but was less efficient.

---

## Use Cases

* Maritime route planning and decision-making
* Evaluation of algorithm efficiency for transportation systems
* Support for logistics and shipping industries
* Academic demonstration of graph-based optimization

---

## Contributors

* Jyoshitha Pechetti (BL.EN.U4CSE22227)
* Tarunya G (BL.EN.U4CSE22259)
* Sneha Yadav (BL.EN.U4CSE22266)

Submitted as part of the Bachelor of Technology degree in Computer Science and Engineering at Amrita School of Computing, Bangalore.
