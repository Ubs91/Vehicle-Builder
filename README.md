# TypeScript Vehicle Builder

A command-line application that allows users to create and interact with different types of vehicles including cars, trucks, and motorbikes.

## Description

The Vehicle Builder is a TypeScript-based CLI application that showcases object-oriented programming principles. Users can create various vehicle types, each with their own unique properties and actions. This application demonstrates inheritance, polymorphism, and interfaces in a practical way.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Class Structure](#class-structure)
- [Video Walkthrough](#video-walkthrough)
- [Technology Used](#technology-used)
- [License](#license)

## Installation

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Install dependencies:
   ```bash
   npm install
   ```

## Usage

To run the application:

```bash
npm start
```

The application will prompt you to:
1. Create a new vehicle or select an existing one
2. If creating a vehicle, choose between car, truck, or motorbike
3. Enter vehicle details
4. Perform actions with the selected vehicle

## Features

- **Vehicle Creation**: Create cars, trucks, or motorbikes with custom specifications
- **Vehicle Actions**: All vehicles can:
  - Start/stop
  - Accelerate/decelerate
  - Turn left/right
  - Reverse
- **Special Actions**:
  - Trucks can tow other vehicles (weight permitting)
  - Motorbikes can perform wheelies
- **Interactive CLI**: User-friendly command-line interface with easy navigation

## Class Structure

The application uses the following class hierarchy:

- **Vehicle** (base class)
  - Implements the Driveable interface
  - Contains basic vehicle functionality (starting, accelerating, etc.)
  
- **Car** (extends Vehicle)
  - Contains car-specific properties and methods
  
- **Truck** (extends Vehicle, implements AbleToTow)
  - Contains truck-specific properties
  - Can tow other vehicles
  
- **Motorbike** (extends Vehicle)
  - Contains motorbike-specific properties
  - Can perform wheelies
  
- **Wheel**
  - Standalone class for wheel properties
  
- **Cli**
  - Handles user interaction and command processing

## Video Walkthrough

[Link to walkthrough video](https://app.screencastify.com/v3/watch/MnplvoMJ1MD8tCwafbGq)

## Technology Used

- TypeScript
- Node.js
- Inquirer.js (for command-line prompts)
- Object-Oriented Programming principles

