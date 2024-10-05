
# Solar System Simulation

A simple interactive solar system simulation created using Three.js. This project visualizes the sun and the eight planets orbiting around it, showcasing their colors, distances, and labels.

![image](https://github.com/user-attachments/assets/04559e34-c733-4bbe-886c-2005fa4d5f3d)



## Features

- **Interactive Camera Controls**: Navigate through the scene using orbit controls.
- **Realistic Planet Colors**: Each planet is represented with its corresponding color.
- **Orbit Paths**: Visual representation of the orbits for each planet around the sun.
- **Dynamic Animation**: Planets rotate on their axes and orbit the sun in real-time.

## Technologies Used

- [Three.js](https://threejs.org/) - A JavaScript library for creating 3D graphics in the browser.
- JavaScript (ES6+)
- HTML
- CSS

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/solar-system.git
   ```
   
2. **Navigate to the Project Directory**:
   ```bash
   cd solar-system
   ```

3. **Open `index.html` in Your Browser**: You can use any web server or simply open the file directly in your browser.

## Usage

- **Orbit the Camera**: Click and drag with the mouse to rotate the camera around the scene.
- **Resize the Window**: The simulation automatically adjusts to window size changes.

## Code Structure

- `index.html`: Main HTML file that sets up the canvas and includes scripts.
- `main.js`: Main JavaScript file where the Three.js scene, camera, renderer, planets, and animations are created.

## Example Code Snippet

Here is a small part of the code that creates the sun and planets:

```javascript
// Create the Sun
const sunGeometry = new THREE.SphereGeometry(1, 32, 32);
const sunMaterial = new THREE.MeshBasicMaterial({ color: 0xffff00 });
const sun = new THREE.Mesh(sunGeometry, sunMaterial);
scene.add(sun);

// Create a planet
function createPlanet(size, color, distance) {
    const geometry = new THREE.SphereGeometry(size, 32, 32);
    const material = new THREE.MeshBasicMaterial({ color: color });
    const planet = new THREE.Mesh(geometry, material);
    planet.distance = distance; // Store distance
    return planet;
}
```



## Acknowledgments

- Thanks to the Three.js community for the extensive documentation and resources.
- Inspiration from various solar system simulations online.

## Contributing

Feel free to submit issues or pull requests if you have suggestions for improvements or additional features!


