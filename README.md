# Bootstrap Starter Project Template

This project is a starter template for Bootstrap 5 using the NPM package.

## Setup Instructions

1. Create an HTML file with boilerplate content.

2. Open the terminal and navigate to your project directory. Type `npm init -y` to initialize a new Node.js project with default settings.

3. Install Bootstrap by running the following command in the terminal: `npm install bootstrap@5.2.3`

Note: Replace `5.2.3` with the desired Bootstrap version number to ensure compatibility.

1. Create a `src` folder and move your `index.html` file into it.

2. Inside the `src` folder, create a new file called `main.scss`.

3. To compile SASS into CSS, you need to install a SASS compiler extension in your code editor (e.g., Visual Studio Code).

- Install the "Live Sass Compiler" extension in Visual Studio Code.
- At the bottom of the VS Code window, click on the "Compile SASS" tooltip.
- A `main.css` file will be generated in the `src` folder alongside your `index.html` and `main.sass` files.

1. Link the generated `main.css` file in your HTML file using the appropriate `<link>` tag.

2. Add the following `<script>` tag underneath the `<title>` tag in your HTML file to include the Bootstrap JavaScript file:

`<script src="../node_modules/bootstrap/dist/js/bootstrap.bundle.min.js"></script>`

1. Test your setup by adding some Bootstrap components to your HTML file.

2. When deploying your site, you shouldn't rely on the node_modules folder. Instead, copy the bootstrap.bundle.min.js file from ../node_modules/bootstrap/dist/js/ and paste it into a new JavaScript file within the src folder. Name this file appropriately (e.g., bootstrap.bundle.js).
   Ensure that the contents of this file match the original bootstrap.bundle.min.js file.
   Update the `<script> tag in your HTML file to point to the new file location.`

3. Finally, test your project to ensure that the Bootstrap components are working as expected.

---

## Overriding Bootstrap Styles

To customize the appearance of Bootstrap components, you can override the default styles by following these steps:

1. Open your main.scss file in the src folder.
2. Below the import statement, you can start overriding Bootstrap styles by targeting specific classes or components. For example, to change the primary button color:

   .btn-primary {
   background-color: #ff0000;
   border-color: #ff0000;
   }

3. Save the main.scss file, and the SASS compiler will automatically generate the updated main.css file.
4. In your HTML file, make sure the main.css file is linked after the Bootstrap CSS file to ensure your custom styles take precedence.
5. Test your changes by refreshing your web page. The customized styles should now be applied to the corresponding Bootstrap components.

N.B Remember to use the appropriate selectors and SCSS syntax when overriding styles. You can refer to the Bootstrap documentation for more information on customizing components and styles.
