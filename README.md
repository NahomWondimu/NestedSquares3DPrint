# Nested Square Model

## Project Overview

The nested square model is a 3D printing project that creates a cube-like structure with square holes in each layer. Each layer has a square hole that is 1/2 the area of the square hole in the layer above it. The length of each square's sides is calculated using the formula:

$$\ L_x = \sqrt{2} \left( \frac{L_{x-1}}{2} \right) \$$

where:
- \(L_x\) is the length of the side of the square hole in layer \(x\),
- \(L_{x-1}\) is the length of the side of the square hole in the layer above layer \(x\).

## Design Process

1. **Formulas Creation**: The first step was to create the formulas that represent the relationship between all the square shapes. The formula \(L_x = \sqrt{2} \left( \frac{L_{x-1}}{2} \right)\) was used to calculate the side length of each square based on the previous layer's square side length.

2. **Area Summation**: Next, a summation was created to represent the total area of all the square holes in the cube. The summation formula is:

\[ \sum_{n=0}^{\infty} 1 \left( 0.5 \right)^n \]

Each term of the summation represents the area of each layer of the square hole, showing how the area decreases with each layer until it approaches 0 or reaches the bottom layer of the cube.

3. **Implementation in Blender**: The formulas were applied in Blender to calculate and create each layer of the cube with the appropriate square hole size.

4. **Transfer to Tinkercad**: The project was then transferred to Tinkercad to add the summation that represents the total area added to the side of the cube by all the square holes.

## Conclusion

The nested square model is a visually intriguing 3D printing project that demonstrates the concept of geometric progression in a tangible and visually appealing way.
