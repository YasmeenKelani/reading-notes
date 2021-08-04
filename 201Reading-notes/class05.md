# Images
**ChoosIng Images for Your sIte**
* A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one. Images can be used to set the tone for a site in less time than it takes to read a description. If you do not have photographs to use on your website, there are companies who sell stock images; these are images you.
**Strong images on your site**
* If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses. As a website grows, keeping images in a separate folder helps you understand how the site is organized. Here you can see an example of the files for a website; all of the images are stored in a folder called images.

* Adding Images: < img>To add an image into the page you need to use an < img>element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:srcThis tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images — relative URLs were covered on pages 83-84). altThis provides a text description of the image which describes the image if you cannot see it.titleYou can also use the titleattribute with the < img> element to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

* heIght & WIdth of Images: You will also often see an < img>element use two other attributes that specify its size:  height: This specifies the height of the image in pixels.width: This specifies the width of the image in pixels.Images often take longer to load than the HTML code that makes up the rest of the page. It is, therefore, a good idea to specify the size of the image so that the browser can render the rest of the text on the page while leaving the right amount of space for the image that is still loading.

**Where to plaCe Images In Your Code**
![image address](https://slidetodoc.com/presentation_image_h2/61d5bf52be95a1b120eda3b5ca2378d5/image-23.jpg)

### Color
* Color can really bring your pages to life. 
**forefround color**
* The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
1. rgb values: These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90).
2.  hex Codes: These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80.
3. Color names: There are 147 predefined color names that are recognized by browsers. For example: DarkCyan.
**Background Color**
* CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box. You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names (covered on the next page). If you do not specify a background color, then the background is transparent. 

![background-color](https://www.stechies.com/userfiles/images/backgroundcolorhtml1200x700webp1577801469.webp)

**Understandimg Color**
* Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.understanding ColorComputer monitors are made up of thousands of tiny squares called pixels (if you look very closely at your monitor you should be able to see them).When the screen is not turned on, it's black because it's not emitting any light. When it's on, each pixel can be a different color, creating a picture.The color of every pixel on the screen is expressed in terms of a mix of red, green, and blue — just like on a television screen. Color picking tools are available in image editing programs like Photoshop and GIMP. You can see the RGB values specified next to the radio buttons that say R, G, B.The hex value is provided next to the pound or hash # symbol. There is also a good color picking tool at: [paletton.com](https://paletton.com/#uid=1000u0kllllaFw0g0qFqFg0w0aF)

![color wheel](https://cdn11.bigcommerce.com/s-all2n9o8xo/images/stencil/1280x1280/products/54353/43245/cwc-3389__24915.1557243287.jpg?c=2)

* CSS3: HSL Colors: CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values. 
1. HueHue: is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360.
2. satuRatioN: Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.
3. liGHtNess: Lightness is the amount of white  (lightness) or black (darkness) in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as luminosity.
![HSl](https://slidetodoc.com/presentation_image_h2/561b6fbf8636d2cc6ecce3560fb12044/image-15.jpg)

### Text
**TechniqueS ThaT offer a Wider choice of TypefaceS**
* There are several ways to use fonts other than those listed on the previous page. However, typefaces are subject to copyright, so the techniques you can choose from are limited by their respective licenses. 
**Specifying TypefaceSfont-family**
```
<!DOCTYPE html><html>  <head>      <title>Font Family</title>      <style type="text/css">   body {font-family: Georgia, Times, serif;}h1, h2 {font-family: Arial, Verdana, sans-serif;}.credits {font-family: "Courier New", Courier, monospace;}      </style>  </head>  <body>      <h1>Briards</h1>      <p class="credits">by Ivy Duckett</p>      <p class="intro">The <a class="breed"  href="http://en.wikipedia.org/wiki/ Briard">briard</a>, or berger de brie, is  a large breed of dog traditionally used as  a herder and guardian of sheep...</p>  </body></html>
```
**Size of Type font-size**
* The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:
1. pixelS: Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px.
2. percenTage: The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.
3. EMS: An em is equivalent to the width of a letter m.We will look at these measurements in greater detail on the next page.

## JPEG vs PNG vs GIF 
* TL;DR: Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.
* Compression: Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.
* Transparency: In a simple form, transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours. Hence it is desirable, that the background of these logos and icons is made transparent so that a single image can be used over multiple background variations.
* Colours: There is a significant difference in the number of colours that can be supported by these 3 formats. JPEG images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes. PNG images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.
* Animation: Animation, in this case, refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video, but essentially a part or the entire image changes with time. Of these 3 formats, only GIF supports animation. This capability makes GIF format suitable for delivering engaging ads and banners. Of late, with the advent of companies Tumblr, 9Gag, Giphy etc. the use of GIF format for memes has picked up.
* Visit [JPEG VS PNG VS GIF](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d).