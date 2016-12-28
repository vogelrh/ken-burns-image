[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/vogelrh/ken-burns-image)
# \<ken-burns-image\>

A Polymer Web Component that pans and zooms an image in a manner often referred to as the _[Ken Burns Effect](https://en.wikipedia.org/wiki/Ken_Burns_effect)_

The component provides a fixed size viewport in which the contained image is animated with scale and translate transforms.
Most all aspects of the animation are controlled by custom CSS styling or web component properties.

_[API Docs](https://vogelrh.github.io/ken-burns-image/components/ken-burns-image/)_
_[Demo](https://vogelrh.github.io/ken-burns-image/components/ken-burns-image/demo)_

Install the component with bower:

```bower install ken-burns-effect --save ```

### Usage

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="ken-burns-image.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<ken-burns-image
   source="demo/kb_example.jpg"
   viewport-width="450px"
   viewport-height="250px"
   scale-start="0.96"
   scale-end="1.8"
   translate-x-end="-290px"
   translate-y-end="-180"  
></ken-burns-image>
```
 This example will create a viewport 450px by 250px to display the image. It starts the animation with the image not visible and scaled by 0.96. The image fades in then over the length of the animation, will end
 with a scale factor of 1.8 and shift the image to the left and down by -290px and -180px respectively before fading out at the end of the cycle. _See the Syling section
 for a description of the default values for the other properties that were not explicitly specified in the example._
 
### Styling
The following custom CSS properties are provided for stying and animation control:

Custom property  | Description | Default
-----------------|-------------|--------
`--kb-animation-duration` | Duration of the animation | 15s
`--kb-animation-count`  | Animation iteration count | `infinite`
`--kb-viewport-width` | Sets the width of the image viewport | `auto`
`--kb-viewport-height` | Sets the height of the image viewport | `auto`
`--kb-background-color` | Sets the background color of the viewport | `auto`
`--kb-scale-start` | Sets the image scale at start of animation | `1`
`--kb-scale-end` | Sets the image scale at end of animation | `1`
`--kb-translate-x-start` | Sets the x axis translation at start of animation | `0px`
`--kb-translate-x-end` | Sets the x axis translation at end of animation   | `0px`
`--kb-translate-y-start` | Sets the y axis translation at start of animation | `0px`
`--kb-translate-y-end` | Sets the y axis translation at end of animation   | `0px`
`--kb-opacity-start` | Sets image opacity at the start of animation | `0`
`--kb-opacity-end` | Sets image opacity at the end of animation | `0`

### License

#### The MIT License (MIT)
Copyright (c) 2016 Robert Vogel

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.