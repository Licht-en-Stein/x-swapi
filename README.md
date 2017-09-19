# x-swapi

A Star Wars API exercise.

This exercise does not need a `package.json` but you will need a server in order to use AJAX.

If you don't have it already installed, I recommend to use `live-server` (which can be installed with `npm i -g live-server` and then run from the terminal with the `live-server` command in the directory of your project).

## Steps

### HTML

Create an `index.html` file with:
- A `header` tag which contains:
  - A `h1` tag with the following content: "Star Wars Browser"
- A `main` tag to which you add the attribute `role` with value `main`
- A `footer` tag with the following content:
  ````html
  Developed with 💙 in Berlin, using the <a href="https://swapi.co/">Star Wars open API</a>.
  ````


### JavaScript

- Create a `index.js` file and add the `script` tag in your `index.html`.
- Add the following content to your `index.js` file:
  ````js
  var mainElement = document.querySelector('main');
  //
  function loadPeople(done) {
    /*
      fill here
      ---------
      - make a request to: 'https://swapi.co/api/people/'
      - call the function "done" and pass it the result of the request
    */
  }
  //
  function renderPeople(people) {
    /*
      fill here
      ---------
      For each given people (use a loop or Array.forEach())
      - create a section element (with the document.createElement())
      - fill the innerHTML (maybe have a look at template literals) of the section with:
        - A header tag which has
          - A h1 tag containing the name of the person
        - A div tag which has a list of the following information:
          - Birth Year
          - Eye Color
          - Skin Color
          - Hair Color
          - Height
          - Mass
        - Add the section element to the main element of the index.html
    */
  }
  // call the loadPeople with the renderPeople function as parameter
  loadPeople(renderPeople);
  ````


### CSS

- Download the `background.gif` file and save it at the root of your project.
- Add the following code in a `style.css` (don't forget to add the `link` tag):
  ````css
  *,
  *:before,
  *:after {
    box-sizing:/* fill here */;
  }

  html {
    height:/* fill here */;
  }

  body {
    font-family:/* fill here */;
    line-height:/* fill here */;
    color:/* fill here */;
    background-color:/* fill here */;
    display:/* fill here */;
    flex-direction:/* fill here */;
    margin:/* fill here */;
    height:/* fill here */;
    background-image:/* fill here */;
    background-attachment:/* fill here */;
  }

  a,
  a:link,
  a:hover,
  a:visited {
    color:/* fill here */;
    text-decoration:/* fill here */;
  }

  h1,
  h2,
  h3 {
    margin:/* fill here */;
    font-weight:/* fill here */;
  }

  header,
  footer {
    color:/* fill here */;
    background-color:/* fill here */;
  }

  body>header,
  body>footer {
    padding-left:/* fill here */;
    padding-right:/* fill here */;
  }

  body>header,
  body>footer {
    padding-top:/* fill here */;
    padding-bottom:/* fill here */;
  }

  body>header {
    border-bottom:/* fill here */;
  }

  main {
    flex-grow:/* fill here */;
    overflow:/* fill here */;
    display:/* fill here */;
    flex-wrap:/* fill here */;
  }

  body>footer {
    border-top:/* fill here */;
  }

  .person {
    width:/* fill here */;
    margin:/* fill here */;
    background-color:/* fill here */;
    border:/* fill here */;
    border-radius:/* fill here */;
  }

  .person>header,
  .person>div {
    padding:/* fill here */;
  }

  .person>header {
    border-bottom:/* fill here */;
  }

  .person ul {
    padding:/* fill here */;
  }

  .person li {
    display:/* fill here */;
    padding:/* fill here */;
  }

  .person .label {
    flex-grow:/* fill here */;
    width:/* fill here */;
  }

  .person .gender {
    color:/* fill here */;
  }

  .person .value {
    color:/* fill here */;
  }

  ````


## Credits

- Star Wars API: https://swapi.co
- background.gif: http://www.textures4photoshop.com/tex/bokeh-and-light/animated-golden-glitter-gif-texture-overlay.aspx