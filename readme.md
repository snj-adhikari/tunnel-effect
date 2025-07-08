# Immersive Scrollable 3D Tunnel

This project is a single-page web experience that combines a scrollable content overlay with an immersive 3D tunnel animation created using Three.js. As the user scrolls through different sections of content, the camera moves through a dynamically colored, glowing tube, creating a seamless and engaging journey.

## Features

-   **Scroll-Driven Animation**: The 3D camera's position inside the tunnel is directly tied to the user's scroll position.
-   **Immersive 3D Tunnel**: A dynamically generated tube with glowing rings that the user travels through.
-   **Dynamic Color Change**: The color of the tunnel's rings changes as the user scrolls into new content sections.
-   **Smooth Section Snapping**: Custom scroll logic smoothly animates the view from one section to the next, preventing jarring jumps.
-   **Responsive Content**: Content sections are styled with Tailwind CSS for a clean and responsive layout.
-   **"End of Tunnel" Effect**: The final section features a fade-out effect using fog, giving the impression that the tunnel is ending.

## How to Use

Since this project is a self-contained HTML file with CDN-linked dependencies, running it is simple:

1.  Download the `index.html` file.
2.  Open the file directly in a modern web browser (like Chrome, Firefox, or Edge).

## Customization

You can easily customize several aspects of the animation and content directly in the `index.html` file:

-   **Content**: Modify the HTML within the `<div id="scroll-content-wrapper">` to change the text, images, or number of sections.
-   **Tunnel Colors**: Change the hexadecimal color values in the `colors` array inside the `updateSceneAndContent()` function to alter the ring colors for each section.
-   **Tunnel Shape**: Adjust the `tubeLength`, `numPoints`, and the math within the `for` loop in the `initThree()` function to change the path of the tunnel.
-   **Animation Speed**: Modify the `duration` variable inside the `scrollToSection()` function to make the scroll transition faster or slower.
-   **Fog Effect**: Tweak the `THREE.Fog` parameters in `initThree()` and the logic in `updateSceneAndContent()` to change the start, end, and color of the fog.

## Technologies Used

-   **HTML5**
-   **CSS3** & **Tailwind CSS**
-   **JavaScript (ES6)**
-   **Three.js**