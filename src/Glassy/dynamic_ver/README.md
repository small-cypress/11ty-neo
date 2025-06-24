# Glassy Layout

Thanks for using this work. 
- Developed by Pale.
- Demo images and assets belongs to their respective authors
- The default design features artwork from "Bleach" manga by Tite Kubo.
- Default background image by Tomoko Uji from unsplash.
## Features

- Static site.
- Dynamic template.
- Support for multiple pages.
- Responsive layout.
- Styling for headers, logs, blog entries and gallery.
- Avoids frames and iframes.
- Dynamic gallery widget.
- Profile section included.

## How it works

This layout features having multiple "pages" in one single file. This pages are elements with the class `section` and are wrapped by the element with the id ` layout_content `. All sections are in the page but only the active (the one with the class active) is the one that shows up. The script in main.js ensures that whenever a user click a link, the corresponding section will show up. Each time an user clicks a link the id of the section `#blog` by example will be appended to the url. Also if you share this url, the script verifies if the url has a section appended so it will render the section the url indicates.

## How to add a new section
Inside the nav tag with the class `nav_links`, add a new link to the menu with the class `nav_link`, with an unique id pointing to the new section you want to add.

Example: To add a "contact" section, add the following inside `nav_link`

`<a class="nav_link" href="#contact">Contact me</a>`

Inside the div with the id `layout_content`, add a new div with the class `section`, and make sure the id of the div corresponds to the href source of the link you added before.

Example: `<div id="contact" class="section"> </div>`

Inside this div add any code you want.

## How enable homepage

The section that will show by default is the one with the class `active`. To change the default homepage just add the class active to the section you want. Be sure to only have one div with the class `active`.

## How to change colors, background and cover image.

Inside **style.css** in the `:root` selector, you can change the default colors and background of the layout.

    --bg-color: The background color of the container. Only change this if you don't want the transparent effect on the layout.
    --text-color: color of the text
    --accent-color: Color of links and titles.
    --accent-color-2: Color of some extra decorations.
    --light-color: Color of borders of the page and titles (h1) and subtitles (h2).
    --bg-image: path to the background image.

To change the cover image of the left side, go to **index.html** and change the src of the image with the class `img-nav`.

## How gallery works

The gallery uses javascript to insert the images dynamically in the desired section. To add images to the gallery, in **main.js** find the variable `gallery_images`, and inside the of the array add the name of your images between duble commas.

You also have to specify the path where you're storing your images in the variable gallery_folder.
## Terms of use

- Feel free to rewrite HTML, CSS, and Javascript as you want and modify the general appearance of the layout as you want.
- I would appreciate if you don't remove the credits, but you can move them freely to another part of the website.
- Don't redistribute the original source code and claim as yours.
---
- Terms are subject to change without notice.
- Code is subject to change without notice.
- Demo images and assets belongs to their respective authors and are credited on each work.

If you have questions please send them to themesbypale@gmail.com

Support me on [Ko-fi](https://ko-fi.com/palemomos) ❤️