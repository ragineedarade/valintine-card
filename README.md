# Valentine's Day Card Animation

This project is a web-based animated Valentine's Day card featuring a floating envelope, an animated card reveal, and a background music loop.

## Features

- Animated envelope and card with hover interaction.
- Falling hearts animation.
- Background music that plays on loop.
- Responsive design that centers the animation on the screen.

## Requirements

- A modern web browser with JavaScript enabled.
- Basic knowledge of HTML, CSS, and JavaScript for any modifications.

## Usage

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/raginee_darade/valentines-day-card.git
    cd valentines-day-card
    ```

2. **Open the main HTML file**:
    Open `index.html` in your preferred web browser to view the animation.

3. **Add your custom message**:
    Replace the placeholder `____` in the `.text` div with your desired message.

## File Structure

- `index.html`: The main HTML file containing the structure of the animation.
- `style.css`: Contains the CSS styles for the animation.
- `veer.mp3`: Background music file.
- `README.md`: Project overview and instructions.

## HTML Code Overview

1. **HTML Structure**:
    ```html
    <div class="container">
      <div class="valentine">
        <div class="envlop"></div>
        <div class="front"></div>
        <div class="card">
          <div class="text">Happy<br />Valentine's<br />Day ____</div>
          <div class="heart"></div>
        </div>
        <div class="hearts">
          <div class="one"></div>
          <div class="two"></div>
          <div class="three"></div>
          <div class="four"></div>
          <div class="five"></div>
        </div>
      </div>
    </div>
    <div class="shadow"></div>
    <audio autoplay loop>
      <source src="veer.mp3" type="audio/ogg" />
    </audio>
    ```

2. **CSS Styles**:
    The CSS in the `<style>` section of the `index.html` file styles the envelope, card, hearts, and shadow, and defines animations.

3. **JavaScript for Hover Interaction**:
    ```javascript
    $(document).ready(function () {
      $(".container")
        .mouseenter(function () {
          $(".card").stop().animate({ top: "-100px" }, "slow");
        })
        .mouseleave(function () {
          $(".card").stop().animate({ top: "0px" }, "slow");
        });
    });
    ```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request on GitHub.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, you can contact the developer through the following links:

- [GitHub](https://github.com/ragineedarade)
- [Email](mailto:ragineedarade@gmail.com)

---

 
