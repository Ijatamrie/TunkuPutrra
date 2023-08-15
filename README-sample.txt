# Project Name 

An empty template for Kuching Property.

# Setup

Make sure to install the dependencies: yarn install

How? : Open a new terminal, an choose a command prompt. Then type yarn install and enter. Dependencies will be installed

## Table of contents 

1. 

   Rename the white coloured text to desired Main title. This white coloured text will be displayed on the page.

   proceed to do steps instructions on line 12 of `condo.vue` file 

   To proceed, check the file `components>Design.vue` and go to line 67.

2. Image folder renaming in `components>Design.vue`

   Rename the image folder path `~/assets/img/floorlayout/*.jpg` to the desired path. For example, if you have a folder named "shoplots" in `assets>img`, change the above line to `~/assets/img/shoplots/*.jpg`.

   If your images are of the `.png` format, update `*.jpg` to `*.png`.

   Proceed to the file `pages>index.vue` and continue following the steps from line 24.

3. **Variable Renaming for Layouts**

   You can rename the variable `LayoutOneBedroom` to your desired name. For instance, change "LayoutOneBedroom" on line 27 to "MallLGFloor". Also, remember to rename "LayoutOneBedroom" on line 72 to "MallLGFloor" accordingly.

   Repeat the renaming process for other variables like "LayoutTwoBedroom" on line 33 and line 79.

4. **Title and URL Replacement for Images**

   Replace the orange-colored text in the title and URL sections. The title will be displayed on the page, and the URL should match the name of the images you placed in the `assets>img>create your-own-folder` directory.

   For example, if you have a folder named "shoplots" and an image named "watson.jpg" within it, set the title to `title: 'Watson'` and URL to `url: 'watson'`.

## Development server

Before continuing on to the development server, Save the changes that has been made on every file by ctrl+s. On the same terminal from the setup part, enter yarn dev to start the development server on `http://localhost:3000`. ctrl+click on the localhost to see the changes that has been made. If the desired pages does not appear, add /condo after the url. So, it will be `localhost:3000/condo`.