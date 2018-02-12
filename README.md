# responsive_layout_v2.0 (Techdegree Project 2)
Project Overview

--------------------

-   Create your file structure:

-   Create an index.html and styles.css file.

-   Create a folder called css and put your styles.css file inside of it. The name of the folder should not be capitalized.

-   Link the styles.css file to index.html

-   Build the layout using a mobile first design:

-   Make sure the HTML file includes the viewport meta tag in the head of the document. See [Configuring the Viewport](https://developers.google.com/speed/docs/insights/ConfigureViewport#overview) to understand why and how to add this tag.

````
<head>
  <meta charset="utf-8">
  <title>Jane Foster</title>
  <meta name=viewport content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="css/styles.css">
</head>
````

-   Look at the provided mockup for the mobile device and add the same header, titles, content and footer information into your index.html file.

-   Use the provided images for the portfolio gallery images shown in the mockups.

````
<div class="list-item odd">
  <img src="images/portfolio-1.png" alt="Marketing Page." class="gallery">
  <div class="description">
    <h3 class="titles">Marketing Page</h3>
    <p>
    This project shows the front page of a marketing website ment for a specific
    business I'm interested in.
    </p>
  </div> <!-- Marketing Description Div -->
</div> <!-- Marketing Div -->
````

-   Use a font from [Google Fonts](https://fonts.google.com/) for the text.

-   Use CSS to style your layout to match the provided mobile mockup. Make sure your mobile design matches the mockup at 320px screen size.

-   Once you have everything in place for the mobile layout, use media queries to add breakpoints to adjust the layout for wider tablet and desktop screens.

-   Match the design as it should look on a tablet device that is 768px wide and a desktop screen size that is 1024px wide.

-   Use a mobile-first approach by writing your media queries using the min-width property in your CSS.

-   Once all your breakpoints are in place, double check your layout matches the three mockups.

````
@media (min-width: 768px) {

  nav, footer {
    flex-direction: column;
  }

  .top-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 0.9em;
    width: 100%;
    margin-top: 2em;
  }

  h1 {
    display: inline-block;
    margin: 0;
    padding: 0;
  }

  .top-nav-list {
    background-color: #E4B04A;
  }

  .top-nav-list:hover {
    background-color: #E4B04A;
  }

  .top-name {
    margin-right: auto;
  }

  .top-nav li {
    padding: 5px 10px 10px 10px;
  }

  header {
    flex-direction: row-reverse;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 3em;
  }

  header p {
    font-size: 1.2em;
    text-align: left;
    margin-left: 1em;
    margin-right: 1em;
    margin-top: -1.5em;
  }

  .portfolio-image {
    margin-top: 2em;
    max-width: 40%;
    margin-right: 1em;
  }

  main {
    margin-top: 0;
  }

  .skills-list {
    flex-direction: row;
  }

  .portfolio {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-around;
  }

  .closing-statement {
    max-width: 65%;
  }

  .list-item {
    max-width: 50%;
  }

  .odd {
    padding-left: 1em;
  }

  .even {
    padding-right: 1em;
  }

  .gallery {
    max-width: 97%;
    align-self: center;
  }

  .end-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 0.9em;
    width: 100%;
  }

  .end-nav-toggle {
    display: block;
  }

  .end-nav li {
    padding: 5px 10px 10px 10px;
  }

  .small-redirect {
    display: none;
  }
}

  @media (min-width: 1024px) {

    nav, header p,
    .portfolio-image, .portfolio,
    .contact, .end {
      margin-left: 2em;
      margin-right: 2em;
    }

    .top-nav {
      flex-direction: row;
      justify-content: space-between;
      width: 100%;
    }

    .top-name {
      text-align: left;
      display: inline-block;
      align-self: flex-start;
    }

    .top-nav li {
      align-self: flex-end;
      display: flex;
    }

    header p {
      width: 50%;
    }

    .list-item {
      max-width: 33%;
    }

    .odd {
      padding-left: 0;
    }

    .even {
      padding-right: 0;
    }

    .closing-statement {
      max-width: 47%;
    }
  }
`````

-   The design does not need to be exact, but the general spacing and arrangement of the elements should match the design of the mockups for mobile, tablet and desktop.

-   Feel free to replace the profile image and customize the text, but the layouts should match the mockups.

-   Link your navigation menu to the correct sections of the page using IDs to link to anchor tags. See this video on  [Linking to Sections of a Web Page](https://teamtreehouse.com/library/linking-to-sections-of-a-web-page).
