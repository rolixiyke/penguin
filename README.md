# Penguin Project

## Project Description
This project is a playful CSS-based representation of a penguin character, designed to demonstrate various CSS techniques and animations. It includes:
- A custom-styled penguin using CSS variables for consistent theming.
- Interactive features like waving arms and resizing on interaction.
- A scalable and responsive design suitable for teaching and learning CSS fundamentals.

## Features
1. Custom CSS Variables:
   - `--penguin-face`: Defines the penguin's face color.
   - `--penguin-picorna`: Defines the shared color for the beak and feet.
   - `--penguin-skin`: Defines the penguin's body color.

2. Animations:
   - `wave`: A keyframe animation used to make the penguin's arm wave.
   - Resizing effect when the penguin is clicked or activated.

3. Interactivity:
   - Clicking or activating the penguin scales it by 50%.

## File Structure
```
project/
|-- index.html   # The HTML structure of the penguin project
|-- styles.css   # The CSS for styling and animations
|-- README.md    # Project documentation
```

## How to Use
1. Clone or download the repository.
2. Open `index.html` in a web browser to view the penguin.
3. Interact with the penguin by clicking on it or observing its waving arm animation.

## CSS Techniques Used
1. CSS Variables:
   - Centralized styling with variables for easy updates.
2. Keyframe Animations:
   - Smooth, repeating animations for dynamic behavior.
3. Pseudo-classes:
   - `:active` pseudo-class to handle user interactions.
4. Transformations:
   - `scale` and `rotate` for resizing and waving effects.
5. Transitions:
   - Added smooth transitions for resizing effects.

## Example Code Snippets
### CSS Variables
```css
:root {
  --penguin-face: white;
  --penguin-picorna: orange;
  --penguin-skin: gray;
}
```

### Waving Animation
```css
@keyframes wave {
  10% {
    transform: rotate(-10deg);
  }
  20% {
    transform: rotate(10deg);
  }
  30% {
    transform: rotate(-15deg);
  }
  40% {
    transform: rotate(15deg);
  }
  100% {
    transform: rotate(0deg);
  }
}

.left-arm {
  animation: wave 3s infinite linear;
  transform-origin: top center;
}
```

### Resizing on Interaction
```css
.penguin:active {
  transform: scale(1.5);
}
```

## Contribution Guidelines
Feel free to fork the repository, make changes, and submit pull requests. Suggestions and feedback are welcome!

## License
This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).

