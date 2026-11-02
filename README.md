

# Traffic Simulator

A JavaFX-based traffic simulation that models a four-way intersection with traffic lights and moving vehicles. Vehicles follow predefined routes, respond to traffic-light states, and slow down to maintain distance from vehicles ahead.

## Features

- Four-way intersection with six lanes on each road: three lanes in each direction
- Traffic lights with green, yellow, and red states
- A repeating signal sequence with yellow and all-red transition phases
- Vehicles that travel straight or turn left or right
- Vehicle types including cars, buses, bikes, and ambulances
- Vehicle movement along waypoint-based routes
- Traffic-light stopping and speed reduction
- Basic vehicle-following logic to reduce overlap
- Vehicles reset to their starting positions after completing their routes

## Built With

- Java
- JavaFX
- Maven

## Requirements

- JDK 26
- Maven
- JavaFX-compatible desktop environment

## Run the Project

1. Clone or download this repository.
2. Open the project in IntelliJ IDEA, or another IDE that supports Maven.
3. Make sure JDK 26 is configured for the project.
4. Open the Maven tool window and run the `javafx:run` goal.

You can also run the project from a terminal in the project directory:

```bash
mvn javafx:run
```

## Project Structure

```text
src/
└── main/
    └── java/
        ├── Main.java
        └── Model/
            ├── Lane.java
            ├── Road.java
            ├── TrafficLight.java
            └── vehicle.java
pom.xml
```

## How It Works

`Main.java` creates the road, traffic lights, and vehicles, then starts an animation loop. The traffic lights cycle through signal phases, while each vehicle updates its position according to its route, the traffic-light state, and nearby traffic.

The `Model` classes handle road drawing, lane information, traffic-light visuals, and vehicle movement.

## Notes

This is a simulation project for learning and experimentation. It does not model every real-world traffic rule or driving condition.

