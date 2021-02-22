# Class 12

## Chart.js and Canvas

[Chart.js Docs](https://www.chartjs.org/docs/latest/)

### [Chart.js Article](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

Charts are a great way to display data in a web page. Chart.js is a well documented and highly used JS plugin. This is how you can use it:

- Download chart.js with npm install chart.js --save
- Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in.
- Place `<script src='Chart.min.js'></script>` in html head
- Add a canvas element to your page `<canvas id="buyers" width="600" height="400"></canvas>`
- Will also need a script to retrieve context of the canvas added to the bottom of body and vars containing data and options. See how this is done on the article.
- You can use similar methods to create line, pie, bar graphs and more that are detailed in the docs.

### `<canvas>`

- The canvas element can also be used without employing an external library. Use these docs from mdn to learn how to do _ with canvas:
  - [Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
  - [Drawing shapes](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
  - [Appling style and color](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
  - [Text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

[<== Back](../README.md)
