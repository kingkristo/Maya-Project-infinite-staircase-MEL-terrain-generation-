-TERRAIN GENERATOR-

This tool uses the principles of the Diamond Square algorithm, a classic approach to terrain generation in which a flat plane is continually subdivided, moving the vertices up or down by a random amount each time, with the level of randomness reduced on each pass. 

Usage: Simply load the Terrain_Generator.mel script into Maya and the tool will be usable via a simple user interface.

Parameters: The tool has several parameters which will help you create terrain of the desired type. Their respective purposes are listed here for reference.
	-TERRAIN PARAMETERS-
	- Iterations: The number of iterations (subdivisions) the algorithm will perform, the more iterations, the more high poly the end mesh. To prevent crashes the maximum number of iterations is 5. [NOTE: iterations of 4 or 5 will be slow but should work without issue.] 
	- Maximum Displacement: The maximum amount the terrain vertices will be moved up or down. 
	- Scale Factor: The amount the max displacement will be divided by upon each iteration (a value of 1 will result in a very volatile terrain, a value of 10 will be much smoother).
	- X Size: The size of the terrain in X dimension.
	- Z Size: The size of the terrain in Z dimension.
	- Add Sea: A Boolean deciding on whether a sea plane is added to the terrain.
	- Sea Height: The height at which the sea plane will be added.
	-TEXTURE PARAMETERS-
	- Add Arnold Textures: A Boolean that decides whether Arnold textures will be added to the terrain mesh [NOTE: in order to view Arnold textures ensure you are using the Arnold renderer and have one or more Arnold lights in the scene]
	- Mountain/Canyon Threshold: The threshold between ground colour and Mountain / canyon colour (e.g. 0.5 will start changing colour halfway between mountain tops and ground level).
	- Sea Opacity: Alpha value of sea texture.
	- Wave Amplitude: Wave bump texture amplitude.
	- Wave Frequency: Wave bump texture Frequency.
	- Sea Colour: Choose the sea colour via a colour picker, default is blue.
	- Mountain/Canyon Colour: Choose the Mountain/Canyon colour via a colour picker, default is grey.
	- Base Ground Colour: Choose the base ground colour via a colour picker, default is green.


