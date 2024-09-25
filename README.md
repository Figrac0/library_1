# Customizator

A JavaScript-based UI component that allows users to customize the scale of text and the background color of a webpage, with settings saved in local storage. This project also includes a reset button to restore default settings.

## Features

- **Text Scaling**: Users can increase or decrease the font size of text elements on the page by selecting from the scale options (1x, 1.5x).
- **Background Color Change**: Users can pick a background color using a color picker input.
- **Local Storage**: Customization settings (text scale and background color) are saved to `localStorage` and are persisted across page reloads.
- **Reset Functionality**: A reset button clears all customizations and restores the default background color and text scale.

## How to Use

1. **Scale Control**: There are two buttons labeled `1x` and `1.5x` that allow users to change the text scaling across the page. Clicking one of these buttons will increase or decrease the font size of all text content on the page.
   
2. **Color Picker**: Users can change the background color by selecting a color from the input color picker. The selected color is applied to the background of the webpage and saved to `localStorage`.

3. **Reset**: A "reset" button (styled as `×`) allows users to reset the background color and text scale to their default values (white background and 1x scale).

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Figrac0/library_1.git
    ```

2. Navigate to the project folder:

    ```bash
    cd library_1
    ```

3. Open the project in a local web server or simply open `index.html` in your browser.

## Code Explanation

- **`onScaleChange(e)`**: This method adjusts the font size of all text nodes based on the selected scaling value (e.g., 1x, 1.5x).
  
- **`onColorChange(e)`**: Updates the background color of the page based on the user's selection and saves the value in `localStorage`.

- **`setBgColor()`**: Applies the saved background color from `localStorage` when the page loads.

- **`reset()`**: Clears the saved scale and color values from `localStorage` and restores default settings.

- **`injectStyle()`**: Injects the CSS styles required for the control panel (scale buttons, color picker, reset button) into the document's head.




