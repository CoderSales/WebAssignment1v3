# WebAssignment1v3

## Description

WebAssignment1v3

## Content with references

### commands

```bash
$ git rm index.html --cached
```

filename can then be added to the .gitignore file

Google Search: [stop tracking a file in git that was previously tracked](https://www.google.com/search?q=stop+tracking+a+file+in+git+that+was+previously+tracked&oq=stop+tracking+a+file+in+git+that+was+previously+tracked&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIHCAEQIRigAdIBCDk1NjZqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8)

[To stop tracking a file that is currently tracked | git-scm.com](https://git-scm.com/docs/gitignore#:~:text=To%20stop%20tracking%20a%20file,being%20reintroduced%20in%20later%20commits.)

____

```bash
git update-index --skip-worktree <file>
```

To cancel

```bash
git update-index --no-skip-worktree <file>
```

Update, a better option [How do I make Git forget about a file that was tracked, but is now in .gitignore? | StackOverflow](https://stackoverflow.com/questions/1274057/how-do-i-make-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitignore)

____

code quote:

```json
 "workbench.colorCustomizations": {

  "editorGutter.addedBackground": "#333",
  "editorGutter.deletedBackground": "#333",
  "editorGutter.modifiedBackground": "#333",
  "editor.background": "#333",
 }
```

modified color to match current vscode settings:

```json
 "workbench.colorCustomizations": {

    "editorGutter.addedBackground": "#202020",
    "editorGutter.deletedBackground": "#202020",
    "editorGutter.modifiedBackground": "#202020",
    "editor.background": "#202020",
 }
```

Summary:

change background color from:
#333 (light grey / black)
to
#202020 (darker black)

Procedure:

Settings > Search: workbench.colorCustomizations > click: edit in settings.json > paste code quote > edit colors to #202020

[VSCode setting to disable git status colors in editor gutter [duplicate] | StackOVerflow](https://stackoverflow.com/questions/45880172/vscode-setting-to-disable-git-status-colors-in-editor-gutter)

____

```css
.card {
        margin: 0 auto; /* Added */
        float: none; /* Added */
        margin-bottom: 10px; /* Added */
}
```

[How to center cards in bootstrap 4? | StackOverflow](https://stackoverflow.com/questions/39031224/how-to-center-cards-in-bootstrap-4)
____

Select all child elements.

```css
parentSelector > * {
  // CSS Styles
}
```

[How to select all child elements recursively using CSS? | geeks4geeks.org](https://www.geeksforgeeks.org/how-to-select-all-child-elements-recursively-using-css/)

____

```css
@media only screen and (max-width: 460px) {
  body {
    background-color: white;
  }
}
```

[What is a Media Query? | W3Schools.com](https://www.w3schools.com/css/css_rwd_mediaqueries.asp)
____

On Windows OS, the forward-slash (/) wasn't working, so I switched to back-slash (\) and that fixed it. For example, try using the following:

```html
"..\..\index.html"
```

[How do I put a hyperlink to "two levels above in the directory tree"? | StackOverflow](https://stackoverflow.com/questions/7051735/how-do-i-put-a-hyperlink-to-two-levels-above-in-the-directory-tree#:~:text=to%20go%20two%20level%20up,to%20go%20more%20levels%20up.&text=You%20can%20use%20..%2Findex.)

____

### Images

[HTML Images | W3Schools](https://www.w3schools.com/html/html_images.asp)

____

### Center Oversized Image in div

#### Failed Attempt

[How to avoid overflow of a bootstrap card image in card-body?](https://stackoverflow.com/questions/72150450/how-to-avoid-overflow-of-a-bootstrap-card-image-in-card-body)

____

#### Successful Attempt

```css
.parent {
    position: relative;
    overflow: hidden;
    //optionally set height and width, it will depend on the rest of the styling used
}

.child {
    position: absolute;
    top: -9999px;
    bottom: -9999px;
    left: -9999px;
    right: -9999px;
    margin: auto;

}
```

[Center Oversized Image in Div | StackOverflow](https://stackoverflow.com/questions/14562457/center-oversized-image-in-div)

____

### Scale Image Responsively

An image can be made responsive by using CSS and setting the width of the image to be a percentage of its parent container, rather than a fixed pixel value. This way, when the size of the parent container changes (e.g. due to different screen sizes), the size of the image will also change proportionally.

```css
img {

max-width: 100%;

height: auto;

}

```

[How to make images responsive | Browser Stack](https://www.browserstack.com/guide/how-to-make-images-responsive#:~:text=An%20image%20can%20be%20made,image%20will%20also%20change%20proportionally.)

____

```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <!-- Container wrapper -->
  <div class="container-fluid">
    <!-- Toggle button -->
    <button
      class="navbar-toggler"
      type="button"
      data-mdb-toggle="collapse"
      data-mdb-target="#navbarCenteredExample"
      aria-controls="navbarCenteredExample"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <i class="fas fa-bars"></i>
    </button>

    <!-- Collapsible wrapper -->
    <div
      class="collapse navbar-collapse justify-content-center"
      id="navbarCenteredExample"
    >
      <!-- Left links -->
      <ul class="navbar-nav mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <!-- Navbar dropdown -->
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            href="#"
            id="navbarDropdown"
            role="button"
            data-mdb-toggle="dropdown"
            aria-expanded="false"
          >
            Dropdown
          </a>
          <!-- Dropdown menu -->
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider" /></li>
            <li>
              <a class="dropdown-item" href="#">Something else here</a>
            </li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true"
            >Disabled</a
          >
        </li>
      </ul>
      <!-- Left links -->
    </div>
    <!-- Collapsible wrapper -->
  </div>
  <!-- Container wrapper -->
</nav>
```

[How to center Bootstrap Navbar](https://mdbootstrap.com/how-to/bootstrap/navbar-center/)

____

```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
```

[Bootstrap Documentation > Navbar > Supported content](https://getbootstrap.com/docs/5.0/components/navbar/#supported-content)

____

### Attempt to make Bootstrap Navbar Responsive

____

[Bootstrap Navbar Active Disabled | freecodecamp.org](https://forum.freecodecamp.org/t/bootstrap-navbar-active-disabled/33111/2)

____

```html
<div id="topheader">
  <nav class="navbar navbar-default">
		<div class="container-fluid">
			 <div class="navbar-header">
				  <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
						<span class="sr-only">Toggle navigation</span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
				  </button>
				  <a class="navbar-brand" href="#">Brand</a>
			 </div>
			 <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
				  <ul class="nav navbar-nav">
						<li class="active"><a href="#home">home<span class="sr-only">(current)</span></a></li>
						<li><a href="#page1">page 1</a></li>
						<li><a href="#page2">page 2</a></li>
						<li><a href="#page3">page 3</a></li>
				  </ul>
				  <ul class="nav navbar-nav navbar-right">
						<li><a href="#">Link</a></li>
				  </ul>
			 </div>
		</div>
  </nav>
</div>
```

```css
#topheader .navbar-nav li > a {
	text-transform: capitalize;
	color: #333;
	transition: background-color .2s, color .2s;
	
	&:hover,
	&:focus {
		background-color: #333;
		color: #fff;
	}
}

#topheader .navbar-nav li.active > a {
	background-color: #333;
	color: #fff;
}
```

```javascript
$( '#topheader .navbar-nav a' ).on( 'click', function () {
	$( '#topheader .navbar-nav' ).find( 'li.active' ).removeClass( 'active' );
	$( this ).parent( 'li' ).addClass( 'active' );
});
```

[Bootstrap Navbar Change Active Class Link [codepen.io]](https://codepen.io/gearmobile/pen/bByZdG)
____

[How to make a .nav-link inactive?](https://stackoverflow.com/questions/15648329/how-to-make-a-nav-link-inactive)
____

## References

center bootstrap div [mdbootstrap](https://mdbootstrap.com/docs/b4/jquery/utilities/horizontal-align/)

stop tracking file [How to stop tracking a file in Git?](https://medium.com/@timmouskhelichvili/how-to-stop-tracking-a-file-in-git-88a75e3f421#:~:text=You%20need%20to%20use%20the,it%20in%20the%20working%20directory.)

Quantitative Research Methods - Sweeney, J.

Web Development - Ryan, C.

Intermediate Programming - Alrimawi, F.

Human Computer Interaction - Motti Ader, L.

Requirements - Richardson, I.
