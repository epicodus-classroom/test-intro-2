## Terminology
<hr />

* **Minified**: A file where unnecessary characters have been removed, making the file smaller and more efficient. Because whitespace is removed and words are reduced to single letters, this code is hard for humans to read. Minified files generally include a `.min` in their name.

* **CDN**:  Short for "content delivery network", a network of servers that deliver content to users. We can load Bootstrap into a project by linking to its CDN location. This simply links to an online version of Bootstrap's stylesheet(s) instead of a version we download and place into our project's directory.

* **End of Life**: When a software version is no longer supported by a company. This usually means that it is not receiving security fixes or new features. 

* **Breaking Changes**: When there are differences between two versions of the same software that can cause your project to stop working.

## Tips
<hr />

* The downside to installing Bootstrap with a CDN link is that you'll be unable to see Bootstrap styles in your project without an internet connection, because the project needs to load the online stylesheet to use Bootstrap's CSS.

* For now, we'll use either the `bootstrap.css` file, or the `bootstrap.min.css` files in our projects. 

* To optionally load Bootstrap's JavaScript, use the `bootstrap.bundle.js` file.
