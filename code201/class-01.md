# Class 1

## Read01: Introductory HTML and JavaScript

### Duckett HTML Introduction (pp.2-11)

This section includes an explanation of how the internet works, using **DNS servers** across the world get you to the web page you want to see.

### Duckett HTML Chapter 1: “Structure” (pp.12-39)

- html tags are called **elements**
- opening tags can carry attributes, which tell us more about the content of that element
- closing tag format `</p>`

### Duckett HTML Chapter 8: “Extra Markup” (p.176-199)

See notes on html tags and escape characters from [code102](/code102/class04-html.md).

### Duckett HTML Chapter 17: “HTML5 Layout” (pp.428-451)

- HTML 5 added many semantic tags to differentiate elements, instead of using a bunch of div tags.
  - header, footer, nav, article, aside, section, hgroup (heading groups), figure, figcaption
- using `<a>` tag around other blocks to link.
- older browsers may not recognize new semantic tags, use this css to treat them as inline elements: `header, section, footer, aside, nav, article, figure {display: block;}`

### Duckett HTML Chapter 18: “Process & Design” (pp.452-475)

See notes about considerations when designing a web page from [code102](/code102/class04-html.md).

### Duckett JS Introduction (pp.2-10)

- JavaScript Examples in Webpages: Slideshows, Validating Forms, Reloading part of a page, Using filters to show the data the user wants.
- Steps to writing scripts: Define goal, design script, code each step
- Using a flow chart to sketch out the tasks/steps needed to solve the problem.

### Duckett JS Chapter 1: “The ABC of Programming” (pp.11-52)

- Introduction Objects, Events and Methods; and how they are used together.
- Window object and document object
- How web browswers see a web page:
  - receive a page as html
  - create a model of the page and store it in memory
  - use a rendering engine to show the page on screen

---

## Lecture Notes

- Move directory up one level with `mv my_directory ../`
- `live-server` command in terminal to start server in your working directory.
- use `!` in vscode first line of html to insert html boilerplate.

[<== Back](/README.md)
