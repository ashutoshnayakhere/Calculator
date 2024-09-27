# Calculator

### Documentation 

#### HTML Structure:
1. **`<!DOCTYPE html>`**: Specifies the document type and version of HTML (HTML5).
2. **`<html lang="en">`**: The root element that defines the document as an HTML file with English as the language.
3. **`<head>` Section**:
   - **`<meta charset="UTF-8">`**: Sets the character encoding of the document to UTF-8.
   - **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Ensures proper scaling and responsiveness on different devices, especially mobile.
   - **`<title>Fixed Size Calculator</title>`**: Sets the title of the webpage as "Fixed Size Calculator" (this appears in the browser tab).
   - **`<style>`**: Contains CSS for styling the calculator layout and buttons.

4. **`<body>` Section**: The body contains the calculator layout and includes:
   - A `div` element with the class **`calculator`** which serves as the container for the entire calculator, giving it a fixed size, background color, and positioning.
   - **Display Section**:
     - **`<input type="text" id="display" disabled />`**: This serves as the display screen of the calculator. It is read-only, so users can only see the result but not type directly into it.
     - **`<button id="backspace">`**: The backspace button is located inside the display container and helps in removing the last entered character.
   - **Buttons Section**:
     - **`<div class="buttons">`**: This section contains all the calculator buttons (numbers, operations, clear, etc.) in a grid layout.

#### CSS Styling:
1. **Body Styling**: The calculator is centered in the viewport using `flexbox`, and a black background covers the entire page.
2. **Calculator Container**: 
   - The calculator has fixed dimensions (`360px` wide and `600px` high) and is styled with a dark background, padding, rounded corners, and a shadow effect to give a sleek look.
3. **Display Area**: 
   - The display box is styled with a black background, white text, and a padding on the right to make space for the backspace button. It includes a white underline for emphasis.
4. **Button Styling**: 
   - Buttons are circular with dark backgrounds and white text. They expand slightly on hover and shrink slightly when pressed for a visual effect.
   - Special buttons like the clear (`C`), divide (`÷`), multiply (`×`), and equal (`=`) buttons are highlighted with a green color to distinguish them from number buttons.

#### JavaScript Functionality:
The following functions manage the core functionality of the calculator:

1. **`appendToDisplay(value)`**: 
   - Appends the selected value (numbers or parentheses) to the calculator's display.

2. **`clearDisplay()`**: 
   - Clears the calculator display when the "C" button is pressed.

3. **`operate(operator)`**: 
   - Adds the corresponding operator (`+`, `-`, `*`, `/`) to the display.

4. **`toggleSign()`**: 
   - Toggles the sign of the displayed number. If the number is positive, it becomes negative and vice versa.

5. **`calculate()`**: 
   - Evaluates the mathematical expression on the display and shows the result. If the input is invalid, it displays "Error".

6. **`deleteChar()`**: 
   - Deletes the last entered character from the display.

7. **Keyboard Input Functionality**:
   - The calculator listens for keyboard events to allow input via the keyboard. It processes numeric keys, operators, the "Enter" key (to calculate), "Escape" (to clear), and "Backspace" (to delete the last character).

#### Key Features:
1. **Fixed Size**: The calculator has a fixed width and height for consistency.
2. **Responsive to Keyboards**: The calculator also supports input from the keyboard for more efficient usage.
3. **Error Handling**: Displays "Error" if the input expression is invalid.
4. **Interactive Button Styles**: Buttons change appearance when hovered or clicked, enhancing user interaction.

