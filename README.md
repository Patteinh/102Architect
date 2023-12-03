# 102Architect 🏡

Welcome to **102architect**.

This project focuses on implementing geometric transformations for home planning software in the context of architecture.

## Language and Tools 🛠️

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

- **Language:** Python
- **Binary Name:** 102architect

## Project Overview 🔎

Your task is to develop a program that computes the coordinates of a point after several geometric transformations, using homogeneous coordinates. The transformations include:

- Translation
- Scaling
- Rotation centered at the origin (O)
- Reflection over any axis through O
- Any combination of the above transformations

### Usage

`./102architect x y [transformation arguments]`

#### DESCRIPTION

- `x`, `y`: Coordinates of the point before transformation
- Transformation arguments vary based on the type of transformation:

  - `-t dx dy` for translation
  - `-z sx sy` for scaling
  - `-r angle` for rotation
  - `-s angle` for reflection

### Examples

#### Example 1

`Input: ./102architect 5 0 -t -1 1`<br>

`Output:`<br>
`Translation along vector (-1, 1)`<br>
`Matrix and coordinates transformation`<br>
`(5.00, 0.00) => (4.00, 1.00)`<br>

#### Example 2

`Input: ./102architect 1 2 -t 2 3 -z 1 -2 -r 45 -s 30`<br>

`Output:`<br>
`Combined transformations`<br>
`Matrix and coordinates transformation`<br>
`(1.00, 2.00) => (0.31, 10.44)`<br>

*Note: Pay attention to the precision of float numbers.*

## Installation and Usage 💾

1. Clone the repository.
2. Compile the program using the provided Makefile.
3. Run the program: `./102architect x y [transformation arguments]`.
4. For detailed guidelines, refer to `102architect.pdf`.

## License ⚖️

This project is released under the MIT License. See `LICENSE` for more details.
