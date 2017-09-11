Check it out here: https://ugotsta.github.io/code-glorify/

# Code Glorify

Simple web app to glorify code ala Instacode (http://instacod.es/) but using GitHub Gists and CSS effects.

Code Glorify is just a simple way to beautify code using CSS effects. It relies entirely on GitHub Gists (https://gist.github.com/) for code reference as well as CSS customization and highlight.js (https://highlightjs.org/) for syntax coloring.

# Usage

The project is just an html page that can be downloaded and used locally or accessed directly online.

Access online here:
https://ugotsta.github.io/code-glorify/

Source code here: https://github.com/Ugotsta/code-glorify/tree/gh-pages

Simply enter a Gist ID and click Glorify. A page will open displaying the Gist's code decorated with default syntax coloring and some basic CSS. Click and drag to move the code section around on the rendered page.

Optionally, select a style for the code coloring as well as a Gist ID to use custom CSS.

More details about the parameters below.

## Gist

Add a Gist ID parameter to view that Gist's code:
https://ugotsta.github.io/code-glorify/?gist=d9d2cd4cdabd1f89c6d6

The Gist ID is simply the ID provided in the url of a Gist repository. The above ID, for example, is seen in the url of the original repository here: https://gist.github.com/uilian/d9d2cd4cdabd1f89c6d6

Just copy the ID portion to use it with Code Glorify.

## Style

Code Glorify uses highlight.js for syntax coloring. As a result, numerous color themes are available, accessible here using the style parameter.

Add a style parameter like so:
https://ugotsta.github.io/code-glorify/?gist=9787981&style=monokai

For more info on the highlight styles, see: https://highlightjs.org/

## CSS

For themeing and further customization purposes, Code Glorify can accept external CSS through a Gist file. Simply provide a Gist ID for the CSS code you wish to use and the app will inject it after loading up.

Completely change the style using custom CSS like so:
https://ugotsta.github.io/code-glorify/?gist=5611986&style=none&css=09e81aebdfc3e6f429a04f22b2308ec5

### Security concerns with user provided CSS

Security is obviously a huge concern when accepting user provided CSS. So besides restricting use of external CSS to GitHub Gists, Code Glorify will also attempt to sanitize the user provided Gist code.

Sanitization method and credits:
https://quaxio.com/html_white_listed_sanitizer/

I'm all ears as to suggestions about this and will easily replace this feature if it becomes an issue.

# Screenshots

No built-in method is currently implemented for screenshots. It's actually difficult because of the heavy use of CSS transforms. Feel free to let me know of any viable library for HTML screenshots that considers CSS transforms. Fortunately, screenshots are easily done with countless free tools.

Some great screenshot apps here: http://alternativeto.net/software/awesome-screenshot-minus/

## Example Gists
- [Vim logo](?gist=5611986) - Vim logo in ASCII art.
- [Cubes](?gist=9787981) - Simple cub in ASCII.
- [Vim Cheats](?gist=c002acb756d5cf09b1ad98494a81baa3) - Simple, intuitive cheatsheet for Vim

## Example CSS Themes
- [Skewed](?css=1fca8332dd34ccfc0eba084deb023962) - Perspective skewed transform
- [Code Glorify](?css=3df562d921295d88564e24b828c0b8b6) - Code Glorify logo theme

## `$gd_info`
Style your code with CSS.  
`$gd_help_ribbon`
`$gd_gist`
`$gd_css`

`$gd_hide`
