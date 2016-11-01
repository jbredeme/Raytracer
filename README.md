# Raytracer
TODO
 
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

## Resources
TODO