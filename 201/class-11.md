## Readings: Audio, Video, Images


[Video and Audio Content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

### Explain how the ability to use video and audio on the web has evolved since the early 2000s.
* The first influx of online videos and audio were made possible by proprietary plugin-based technologies like Flash and Silverlight. Both of these had security and accessibility issues, and are now obsolete, in favor of native HTML solutions <video> and <audio> elements and the availability of JavaScript APIs for controlling them.

### Describe the use of the src and controls attributes in the <video> element.
#### src
* In the same way as for the <img> element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.

#### controls
* Users must be able to control video and audio playback (it's especially critical for people who have epilepsy.) You must either use the controls attribute to include the browser's own control interface, or build your interface using the appropriate JavaScript API. At a minimum, the interface must include a way to start and stop the media, and to adjust the volume


### Why is it important to have fallback content inside the <video> element?
* this will be displayed if the browser accessing the page doesn't support the <video> element, allowing us to provide a fallback for older browsers. This can be anything you like; in this case, we've provided a direct link to the video file, so the user can at least access it some way regardless of what browser they are using.

### Write a very short story where <audio> and <video> are characters.

Video said to audio: "I can hear you but I can't see you." 
Audio said to video: "What?"
The End.

## [A Complete Guide To Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

### How does Grid layout differ from Flex?
Flex is one dimensional
Grid is more like a table, but better!

### Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.
 * Grid Container: The element on which display: grid is applied. It’s the direct parent of all the grid items.

 * Grid Item: The children (i.e. direct descendants) of the grid container.

 * Grid Line: The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column.

 * Grid Cell:  The space between two adjacent row and two adjacent column grid lines. It’s a single “unit” of the grid. 

 * Grid Track: The space between two adjacent grid lines. You can think of them as the columns or rows of the grid. 

 * Grid Area: The total space surrounded by four grid lines. A grid area may be composed of any number of grid cells.

### [Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

### Besides making a site visually appealing across different screen sizes, why should developers make images responsive?
* This helps to improve performance across different devices.
* wasted bandwidth; in particular, mobile users don't want to waste bandwidth by downloading a large image intended for desktop users, when a small image would do for their device.

### Define the following img attributes srcset and sizes. Write an example of how they are used.
* img: The standard <img> element traditionally only lets you point the browser to a single source file.

* srcset: defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma. 

* sizes:defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true.

### How is srcset more helpful for responsive images than CSS or JavaScript?
Use srcset and the x descriptor in the img element to give hints to the browser about the best image to use when choosing from different densities.
The srcset attribute enhances the behavior of the img element, making it easy to provide multiple image files for different device characteristics.


## Bookmark and Review

[Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)

Discusses how to add an image to a web page

This article is review from Class 05.

[Other Embedding Technologies](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Other_embedding_technologies)

Looks at  some elements that allow you to embed a wide variety of content types into your webpages: the iframe, embed and object elements. iframe's are for embedding other web pages, and the other two allow you to embed external resources such as PDF files.

