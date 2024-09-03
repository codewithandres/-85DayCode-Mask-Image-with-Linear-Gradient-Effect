![alt text](<assets/bandicam 2024-09-02 21-07-19-379.jpg>)

# Project Image Hover Effect

This project implements a dynamic image reveal effect for project links on a web page. When users hover over project links, corresponding images are revealed with a smooth animation effect.

## File Structure

-   `js/app.js`: The main JavaScript file containing the hover effect logic.
-   `assets/`: Directory containing project images.

## How It Works

The `app.js` file handles the following key functionalities:

1. **Mouse Tracking**: The script tracks mouse movements to update the position of revealed images.

2. **Image Management**: Each project link is associated with an `ImageItem` instance, which manages the corresponding image and its reveal effect.

3. **Hover Effect**: When a user hovers over a project link, the associated image is revealed with a sliding animation effect.

4. **Smooth Animations**: The script uses linear interpolation (lerp) to create smooth transitions for both mouse tracking and image reveal animations.

## Key Components

-   `ImageItem` class: Manages individual project images and their hover effects.
-   `animate` function: The main animation loop that updates mouse position and animates all `ImageItem` instances.
-   Event listeners: Handle mouse movements, window resizing, and hover events on project links.

## Usage

To use this effect in your project:

1. Include the `app.js` file in your HTML.
2. Ensure your project links have a `data-image` attribute with the corresponding image filename.
3. Place your project images in the `assets/` directory.

The script will automatically set up the hover effects for all elements with the class `project`.
