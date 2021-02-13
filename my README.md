CS 425 Assignment 0.

The purpose of this Assignment was to 
- Create a number of triangles on a canvass
- Change the colors of the triangels using RGBA sliders
- Randomly change the color of the triables using a checkbox
- Read JSON files and convert the data into a series of triangles and colors.

My first function "makeTrianges(number)" updates the number of trinagles and the
n_slider value, then it creates the buffer and binds it to the vao to make the 
drawings.

The next function, loadShader(type, source) creates a shader and returns it

The next function, createProgram() creates the program and links the shaders
we need in the program

The next function, changeColorOnInput(), changes the color of the triangle to 
the rgb values either assigned in the JSON file, or the default triangle at launch. It will also dynamically change the colors.

randomizeColor() will create random rgb values and call the changeColorOnInput() method to update the color change.

createVAO() creates the VAO.

draw() is the method that binds the vao and draws on the canvas the triangles based on the data provided.

main() starts the application off.