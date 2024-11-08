# Selected Animation Method: Perlin Noise-driven Motion



To animate this scene, I used Perlin Noise as the primary technique to create smooth, natural movement for all elements. By assigning unique Perlin Noise offsets to each component and newly added free particles, following the original color scheme, a natural, fluid swaying effect was achieved. This allowed each element to show slight drifts and shifts over time, each moving individually yet in coordinated harmony.

## Animation Properties and Uniqueness   

Plates: These foundational elements appear first, with subtle horizontal and vertical swaying achieved through Perlin Noise. Each plate has its own noise offset, which introduces gentle, random motion, adding a natural feel to the foundational structure of the scene. Only a few plates are shown at a time, gradually building up the scene’s layers.

Vertical Lines: Introduced after the plates, these vertical lines serve as supports within the scene's structure. Each line undergoes slight oscillation along the y-axis under the influence of Perlin Noise, enhancing vertical depth and the scene’s three-dimensional feel.

Random Boxes: These elements move around the vertical lines, constrained to the space around them with subtle Perlin Noise-driven movement along all axes. Each box appears to hover around the structures, adding layers and complexity to the scene.

Free Shapes: These are the final elements to appear, floating freely in the 3D space, driven by Perlin Noise throughout the entire screen space. Each element drifts as if blown by the wind, resembling colorful petals.

This animation effect creates a smooth, dynamic visual experience by using Perlin Noise to enable seamless motion for each element. By grouping elements and setting different ranges and amplitudes of movement, the composition becomes layered and rich. Perlin Noise introduces unpredictable yet coherent movement, making the scene more lively and immersive.

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

WEBGL: 3D effects were achieved by setting the canvas to WEBGL mode. Reference: https://p5js.org/reference/p5/WEBGL/

map(): Used to precisely control the dynamic variation of element properties, ensuring smooth and natural animation. Reference: https://p5js.org/reference/p5/map/

This code combines layered Perlin Noise, separate settings for different elements, and variations in shape and color to achieve a free-flowing, dreamy, and multi-layered animation effect in a 3D scene.


