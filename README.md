# Selected Animation Method: Perlin Noise-driven Motion



To animate this scene, I used Perlin Noise as the primary technique to create smooth, natural movement for all elements. By assigning unique Perlin Noise offsets to each component and newly added free particles, following the original color scheme, a natural, fluid swaying effect was achieved. This allowed each element to show slight drifts and shifts over time, each moving individually yet in coordinated harmony.

## Perlin Noise Usage Explanation:   
### Individual Dynamic Settings Using Perlin Noise:

Perlin Noise is applied to each base element individually, creating unique, dynamic movement across the entire composition.
### Creating Free Particles:    

A set of free-floating particles is created, and Perlin Noise is used to make them wander within the canvas bounds.
### Layered Dynamic Effect:

To enhance the visual layering, a secondary dynamic effect is applied over all elements on the canvas, adding an extra layer of visual depth.
## Special Design Treatments
### Plates:    

These foundational elements appear first, with subtle horizontal and vertical swaying achieved via Perlin Noise. Each plate has its own noise offset, creating a soft, random movement that brings a natural feeling to the base structure of the scene. Only a few plates are displayed at a time, gradually building a sense of depth.
### Vertical Lines:      

Introduced after the plates, these vertical lines serve as structural supports in the scene. Under the influence of Perlin Noise, each line sways slightly along the y-axis, adding vertical layers and enhancing the scene’s dimensionality.

### Random Boxes:    

These elements move around the vertical lines, with limited movement within the defined vertical space. Perlin Noise drives their movement across different axes, making each box appear as though it is floating around the structure, adding complexity and depth to the scene.

### Free Shapes:    

These are the final elements to appear, freely floating in the 3D space, filling the entire screen area with Perlin Noise-driven motion. Each shape moves independently, like colorful petals carried by the wind.

This animation effect creates a visually smooth and dynamic experience. By using Perlin Noise, each element moves fluidly. Grouping the elements and setting varied movement ranges and amplitudes enriches the scene with visual layers. Perlin Noise introduces unpredictable yet coherent motion, bringing the scene to life with an immersive sense of depth.


## References and Inspiration   
Inspired by petals floating in the streets of Sydney, I used Perlin Noise to create dynamic, free-moving blocks to simulate the movement of petals, presenting a dreamy effect.

![8fa6bede8c2cb6125860352958320802](https://github.com/user-attachments/assets/b5d18d72-966f-448f-8b80-4d9449d345c9)

![b81a50d8ef343e258d3a3203c7b181d1](https://github.com/user-attachments/assets/97c66561-9c33-4ae4-a41b-81629e051b14)


## Technical Explanation   
In this code, I used p5.js to implement dynamic effects based on Perlin Noise. Here are the key techniques utilized:

### Perlin Noise Dynamic Effect

Perlin Noise was used to generate dynamic variations in elements (such as boxes and particles), ensuring smooth, free-flowing motion in space. By mapping noise to each element's position and rotation, a natural dynamic effect is achieved.
Specifically, noise(x, y, z) controls the positional variation of elements, creating a smooth transition based on the noise function at each iteration.

### Nested Structure

Multiple nested loops were used in the code (mainly for individual element oscillation and overall element movement) to apply Perlin Noise across multiple dimensions. Each nested level controls different visual elements, enriching the animation effect and enabling smooth transitions across layers.


### 3D Rendering and Canvas Setup

The WEBGL mode in p5.js was used to create a 3D canvas, which allows for 3D graphical functions like rotation, translation, and scaling to enhance the visual experience.
By setting up the canvas with createCanvas() in WEBGL mode, 3D shapes (e.g., boxes and particles) can be dynamically controlled and rendered on the canvas.

## External Tools and Techniques

WEBGL: 3D effects were achieved by setting the canvas to WEBGL mode. Reference: [WEBGL in p5.js ](https://p5js.org/reference/#/p5/WEBGL)


map(): Used to precisely control the dynamic variation of element properties, ensuring smooth and natural animation. Reference: [map() in p5.js](https://p5js.org/reference/#/p5/map)


This code combines layered Perlin Noise, separate settings for different elements, and variations in shape and color to achieve a free-flowing, dreamy, and multi-layered animation effect in a 3D scene.


