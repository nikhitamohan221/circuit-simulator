
# Circuit Simulator

A browser-based interactive circuit simulator built with vanilla JavaScript and HTML5 Canvas. Supports real-time simulation using Modified Nodal Analysis (MNA) with Backward Euler integration.

## Features

- **Components**: Resistor, Capacitor, Inductor, DC Voltage Source, Ground
- **Wire Routing**: Draw wires to connect components
- **Real-Time Simulation**: Live voltage and current calculation
- **Oscilloscope Graph**: View V/I waveforms with zoom and pan
- **Undo / Redo**: Full history with Ctrl+Z / Ctrl+Y
- **Component Properties**: Edit values and labels via the properties panel
- **Rotation**: Right-click any component to rotate
- **Delete**: Remove selected components or wires

## How to Use

1. Select a component from the toolbar
2. Click on the canvas to place it
3. Select **Wire** and draw connections between component pins
4. Add a **Ground** component to at least one node
5. Click **Start Simulation** to begin
6. Click any component to view its voltage/current graph

## Simulation Details

- Solver: Modified Nodal Analysis (MNA)
- Integration: Backward Euler
- Time Step: 1ms (DT = 0.001s)
- Max History: 10,000 data points

## Components

| Component       | Symbol | Unit |
|----------------|--------|------|
| Resistor        | R      | Ω    |
| Capacitor       | C      | F    |
| Inductor        | L      | H    |
| DC Voltage Source | V    | V    |
| Ground          | GND    | —    |

## Keyboard Shortcuts

| Action     | Shortcut        |
|------------|-----------------|
| Undo       | Ctrl + Z        |
| Redo       | Ctrl + Y        |
| Delete     | Delete / Backspace |

## Tech Stack

- HTML5 Canvas
- Vanilla JavaScript
- No external libraries or frameworks

## Live Demo

[Click here to open the simulator](https://github.com/nikhitamohan221/circuit-simulator/)

## License

MIT License
