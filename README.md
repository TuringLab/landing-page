#Landing Page

Create your own landing page. Whenever you open your internet browser you can chose what to show.

## Making a Website

Websites are made of `HTML`, `CSS` and `JavaScript`. You are going to learn about all 3 today.

### HTML Introduction

Start by working through [this turotial](https://www.codecademy.com/en/skills/make-a-website/topics/html-elements/html-css-intro) which will give you an introduction to web design.

When you have completed the introduction return to this page and continue the tutorial.

### Editing HTML

To create your own website you need to edit the code.

- Download [Sublime Text](http://www.sublimetext.com/3) to get started.
- Install Sublime Text
- Open Sublime Text to get started

### HTML Basics

Lets create your first website using the code bellow

- Paste this code into Sublime Text
- Save your file on your Desktop and call it `index.html`
- Double click `index.html` to open the file in your browser


```html
<html>
    <head>
        <title>My's Landing Page</title>
    </head>
    <body>
        Hello World!
    </body>
</html>
```

### Adding a Greeting

Change your `<body></body>` tag to look like the following code

```html
<body>
    <div class="greeting">
        <h1>Hello</h1>
    </div>
</body>
```

The `class="greeting"` is used in the next section.

Save your work and **reload your page**, how does your website look?

### Adding a Style

Have a look at [this turotial](https://www.codecademy.com/en/skills/make-a-website/topics/css-properties-text/css-intro) to get started with how `CSS` works.

Change your `<head></head>` tag to look like the following code 

```html
<head>
    <title>My's Landing Page</title>
    <style type="text/css">
        body {
            background-color: red;
        }
    </style>
</head>
```

**Reload your page** and have a look how it has changed, this changes the color of the page.

To make your greeting more elegant change your `<style></style>` tag to look the following code

```html
<style type="text/css">
    body {
        background-color: red;
    }
    .greeting {
        margin: auto;
        padding: 100px;
        text-align: center;
    }
</style>
```

### Background Image

<!-- TODO - HENRY MISKIN -->
https://unsplash.it/1280/800/?random

### Weather Widget

<!-- TODO - HENRY Lake -->
http://www.wunderground.com/stickers/

### Quote of the Day

We are going to include a quote of the day on your website

Add the following lines to the `<head></head>` tag.

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
<script>
    $.get( "http://api.theysaidso.com/qod.json", function( data ) {
        var quotes = data.contents.quotes;
        $('#quote').html(quotes[0].quote)
        $('#author').html(quotes[0].author)
    });
</script>
```

Add the following lines to the `<head></head>` tag.

```html
<div class="quote">
    <h2 id="quote"></h2>
    <h3 id="author"></h3>
</div>
```

## Resources

http://webdesign.tutsplus.com/series/web-design-for-kids--cms-823
https://www.codecademy.com/skills/make-a-website
