# Images, Color, and Text

## Images

Images can be displayed in HTML with the `<img>` tag. This tag has 2 necessary attributes: `src` and `alt`. `src` is used to define the path to the image (either relative, if the file is stored locally with your page, for instance `images/image.jpg`, or as an URL, for instance `https://www.example.com/image.jpg`). Although images may be rescaled easily in CSS, it is best practice to alter the image beforehand to the desired dimensions.

## Color

Color, when used effectively, will make your webpage clean and functional, and can be used to highlight or soften the impact of certain elements. It is a very important factor in the overall aesthetic of your site. Color can be desclared in several ways in CSS:

* RGB value: in the format `rgb(0,0,255)` (this will make a pure blue color.)
* RGBA value: the same as RGB but the final value will specify opacity.
* Hex codes: Similar to RGB but using the hexidecimal system, for instance `#FF0000` (this will make a bright red color).
* Color names: some color names have predefined values and can be used to more easily reference colors, for instance `aquamarine` (this will make an aquamarine color. Who would have guessed?)

Online color pickers can be a useful tool to find the RGB value of colors you want, and to tweak them slightly using color wheels or graphs to find the exact color you need. Many text editors, such as VSCode, have built-in color pickers.

## Text

In CSS you can control several properties of text, including font (`font-family`), font size (`font-size`), weight (`font-weight`), and style, such as itallics or oblique (`font-style`). While millions of fonts exist, there are a standard relatively few that you can assume will be installed on every machine. With the `font-family` attribute you can choose more than one font and the site will fall back on the next in the list if the computer is unable to render the first. If the font is not likely to be installed, you can use the `@font-face` tag and define its name with the `font-family` attribute and then specify a URL to download it with the `src` attribute. You can seperately style links that have been visited or not, or are hovered over, with the `a:link`, `a:visited`, and `a:hover` tags respectively. These are called pseudoclasses, and the `:hover` pseudoclass in specific also works on many other elements. For instance, you could make an image light up or pop out when it's hovered by using `img:hovered`.
