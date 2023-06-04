# CSS_Task2
README for Adding New Images for List Style Type in `<ul>` with CSS
--------------------------------------------------------------------

This README provides a step-by-step guide on how to add new images for the list-style-type in an unordered list (`<ul>`) using CSS. By following these instructions, you can customize the appearance of list items by replacing the default bullet points with your own images. Here's how to get started:

1. Prepare your custom images: Collect or create the images you want to use as list markers. Ensure that the images are in an appropriate format such as PNG, JPEG, or SVG.

2. Add the images to your project: Place the image files in a directory accessible to your HTML file. Note the file path to the images for future use.

3. Define a class for your custom list style: Open your CSS file and create a new class to define the custom list style. Let's name this class `.custom-list`:

```css
.custom-list {
  list-style-type: none; /* Remove default list style */
  padding-left: 10px; /* Adjust padding as needed */
}
```

4. Set the background image for list items: Within the `.custom-list` class, set the `background-image` property to the path of your image file(s) using the `url()` function:

```css
.custom-list li {
  background-image: url('path/to/your/image.jpg');
  background-repeat: no-repeat; /* Prevent image repetition */
  background-position: left center; /* Adjust image position */
  padding-left: 30px; /* Adjust padding to make room for the image */
}
```

Replace `'path/to/your/image.jpg'` with the actual path to your image file. If you have different images for various list items, you can use distinct class names or specify different images for individual list items using their respective selectors.

5. Apply the class to your unordered list: In your HTML file, add the `.custom-list` class to the `<ul>` element you wish to style:

```html
<ul class="custom-list">
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ul>
```

Upon viewing your HTML page, the list items should display your custom images as list markers.

Note: Ensure that the image files are accessible from the HTML file by providing the correct file path. Additionally, adjust the CSS properties (such as padding, background-position) to suit your desired layout and styling preferences.

Congratulations! You have successfully added new images for the list-style-type in an unordered list using CSS. Feel free to experiment with different images, styles, and positioning to create unique and visually appealing list styles.
