# Make Your Github Pages Site

1. Log into https://github.com
2. Click the + sign in the upper right hand corner and then click "new repository"
3. Name your repository [yourusername].github.io as in mjlavin80.github.io
4. Click the box to initialize the site with a README
5. Click the green "create repository" button

# Create index.html with basic page elements

1. Navigate to your repository and click "create new file"
2. In the "name your file" box, type "index.html"
3. In the "edit new file" field below the title, paste the following base markup with your "about me" paragraph

```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>[Your Name]'s Github Pages Site</title>
    </head>
    <body>
      <h1>[Your Name]'s Github Pages Site</h1>
      <nav>My Menu</nav>
      <main>
        <h2>About Me</h2>
        <p>[About me text here]</p>
      </main>
      <footer>
        My Footer
      </footer>
    </body>
  </html>
```
4. Click the green commit button to save changes

# Add a style.css file

1. Navigate to your repository and click "create new file"
2. In the "name your file" box, type "style.css"
3. Add a test rule to your css file, perhaps something like ``` h1 { color: lightgray; } ```
4. Navigate back to your repository and click the "index.html" file 
5. Locate and click the pencil icon, which will bring to an editor view
6. Paste the following line of code just before the ```</head> ``` tag

```html
<link rel="stylesheet" type="text/css" href="style.css">
```
7. Click the green commit button to save changes

# Create your main menu

1. Edit your ```index.html``` file (instructions above)
2. Replace the text "my menu" with this block of code inside the ```<nav>``` tag 

```html
<ul class="main-menu">
  <li>Link 1</li>
  <li>Link 2</li>
  <li>Link 3</li>
  <li>Link 4</li>
  <li>Link 5</li>
</ul>
```
3. Edit your ```style.css``` file the same way you would edit ```index.html``` (instructions above)
4. Add a rule for ```<ul>``` blocks with the class ```main-menu ```

```css

ul.main-menu {
    list-style-type: none;
    margin: 0;
    padding: 0;
}
ul.main-menu>li {
    display: inline;
}
```
5. Click the green commit button to save changes

# Add Directories

Note: These steps create a link and a location for your final portfolio

1. Navigate to your repository and click "create new file"
2. In the "name your file" box, type "portfolio/index.html"
3. In the "edit new file" field below the title, paste the markup from your index.html file, editing things like the page title where appropriate
4. Click the green commit button to save changes

This process has now created a folder called "portfolio" and an index.html file in that folder. Repeat these steps to add other directories.

# Links to the Menu/Site

1. Edit your ```index.html``` file (instructions above)
2. Inside of your first ```<li>``` tag, change "link 1" to the following:

```html
<a href="/portfolio/">Final Portfolio</a>
```
3. Click the green commit button to save changes
