# Raytracer
This application implements a recursive raytracer that creates a PPM (Portable PixMap) image of mathematical primitives drawn from a JSON (JavaScript Object Notation) file. The data is loaded into pixel buffer where reflection and refraction components are added to the scene of objects to produce lighting and coloring effects.
 
## Screenshots
TODO

## Usage
```c
raytrace width height input.json output.ppm
```

## Example json scene data
```javascript
[
    {
        "type": "camera",
        "width": 2.0,
        "height": 2.0
    },
    {
        "type": "sphere",
        "radius": 2.0,
        "reflectivity": 0.2,
        "refractivity": 0.3,
        "ior": 1.33,
        "diffuse_color": [1, 0, 0],
        "specular_color": [1, 1, 1],
        "position": [0, 1, 5]
    },
    {
        "type": "sphere",
        "radius": 0.35,
        "reflectivity": 0.2,
        "refractivity": 0.3,
        "ior": 1.33,
        "diffuse_color": [.13, .25, .53],
        "specular_color": [1, 1, 1],
        "position": [0, .45, 2.5]
    },	
    {
        "type": "plane",
        "normal": [0, 1, 0],
        "diffuse_color": [0, 1, 0],
        "specular_color": [1, 1, 1],
        "position": [0, -1, 0]
    },
    {
        "type": "light",
        "color": [2, 2, 2],
        "theta": 0,
        "radial-a2": 0.125,
        "radial-a1": 0.125,
        "radial-a0": 0.125,
        "position": [1, 3, 1]
    }
]
```

## Built With
* [Cygwin](https://cygwin.com/index.html) - 64-bit version for Windows
* GNU Compiler Collection (GCC) release 5.4.0
* GNU Make release 4.2.1
* Windows 10 Professional

## Author
* **Jarid Bredemeier**
