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

## References

center bootstrap div [mdbootstrap](https://mdbootstrap.com/docs/b4/jquery/utilities/horizontal-align/)

stop tracking file [How to stop tracking a file in Git?](https://medium.com/@timmouskhelichvili/how-to-stop-tracking-a-file-in-git-88a75e3f421#:~:text=You%20need%20to%20use%20the,it%20in%20the%20working%20directory.)

Quantitative Research Methods - Sweeney, J.

Web Development - Ryan, C.

Intermediate Programming - Alrimawi, F.

Human Computer Interaction - Motti Ader, L.

Requirements - Richardson, I.
