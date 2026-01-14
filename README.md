# Mathematics - Unity Project

A Unity game project demonstrating world-to-screen coordinate conversion and mathematical transformations.

## Overview

This project explores coordinate system conversions in Unity, specifically transforming 3D world positions to 2D screen coordinates. Useful for UI overlays, HUD elements, and understanding Unity's coordinate systems.

## Features

- **World-to-Screen Conversion**: Real-time conversion of 3D world positions to screen space coordinates
- **Debug Visualization**: Live logging of screen positions for educational purposes

## Project Structure

```
Assets/
├── Scenes/
│   └── SampleScene.unity    # Main demo scene
└── WorldToScreen.cs          # Core coordinate conversion script
```

## Requirements

- **Unity Version**: 2021.3 or later (LTS recommended)
- **Platform**: Windows, macOS, Linux

## Getting Started

### Installation

1. Clone the repository:
```bash
git clone <your-repository-url>
cd mathematics
```

2. Open the project in Unity Hub
3. Open `Assets/Scenes/SampleScene.unity`
4. Press Play to see coordinate conversions in the console

### Usage

Attach the `WorldToScreen` component to any GameObject in your scene. The script will continuously log the object's screen-space position to the Unity console.

```csharp
// The WorldToScreen script converts world position to screen coordinates
Vector3 screenPos = Camera.main.WorldToScreenPoint(transform.position);
```

## Development

### Scripts

- **WorldToScreen.cs**: Demonstrates Camera.WorldToScreenPoint() functionality
  - Updates every frame in Update()
  - Logs screen coordinates (x, y, z) where z is the distance from camera

### Building

1. Open Build Settings (`File > Build Settings`)
2. Select your target platform
3. Click `Build` or `Build and Run`

## Technical Details

- **Screen Coordinates**: Origin (0,0) is bottom-left corner
- **Z-value**: Represents distance from camera in world units
- **Camera**: Uses main camera for conversions

## Contributing

Feel free to fork this project and submit pull requests for improvements or additional mathematical demonstrations.

## License

This project is open source and available under the MIT License.

## Author

DefaultCompany

---

*Built with Unity for learning coordinate systems and mathematical transformations in game development.*
