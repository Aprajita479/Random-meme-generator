# Random Meme Generator

This is a simple web application that generates random memes using the Meme API. It displays a meme image on the page and updates it every 5 seconds with a new random meme.

## Getting Started

To run this application, simply open the `index.html` file in a web browser.

## Prerequisites

No prerequisites or additional dependencies are required to run this application.

## Usage

Once the application is running, you will see a heading "Random Meme Generator" and a meme container with an initially empty image. The application will automatically fetch a random meme from the Meme API and display it in the image container.

The image will be updated every 5 seconds with a new random meme. If you hover over the image, the automatic updating will pause. When you move the mouse away from the image, the updating will resume.

## Code Overview

The code consists of two main files: `index.html` and `style.css`.

### `index.html`

This file contains the HTML structure of the web application. It includes a heading, a meme container, and a script section with JavaScript code.

### `style.css`

This file contains the CSS styles for the web application. It sets some basic styling for the page layout and the meme image.

### JavaScript Code

The JavaScript code in the `<script>` section performs the following actions:

1. It selects the meme image element using the class name.
2. It defines an `async` function called `randomMemeGenerator` that fetches a random meme from the Meme API.
3. The function fetches the meme using the URL "https://meme-api.com/gimme" and waits for the response.
4. It logs the response to the console for debugging purposes.
5. It parses the response JSON and extracts the meme URL.
6. It sets the `src` attribute of the meme image to the extracted URL, thus displaying the meme on the page.
7. The `randomMemeGenerator` function is called once to display an initial meme.
8. It sets up a timer that calls the `randomMemeGenerator` function every 5 seconds to update the meme.
9. It adds event listeners to the meme image for the `mouseover` and `mouseleave` events.
10. When the mouse is over the image, it clears the timer, pausing the automatic updating.
11. When the mouse leaves the image, it resets the timer, resuming the automatic updating.

Feel free to modify the code or add new features as needed.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
