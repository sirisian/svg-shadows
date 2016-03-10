# svg-shadows
An algorithm to generate minimal SVG shadow paths from SVG paths.

**Note that quadratic Paths aka C and c are not supported. They could be supported though and the code is partially there. Wasn't part of my requirements.**

Also while it could be supported I treat paths that duplicate points as invalid. If you pass in a path that duplicates points you'll see the shadow clip through subpaths. This can be fixed by removing such paths after the parsing step or fixing the SVG path to not do that which is more ideal.

**svgshadow.js** - Contains the core algorithms. Specifically PathToSVGShadowPath(svgPath, width, height) takes in an SVG path as a string and outputs an SVG shadow path.

**index.html** - Contains tests that use Material Design Icons  
**icons.txt** - The test icons  
