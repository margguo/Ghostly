# Ghostly

A theme for [Ghost](http://github.com/tryghost/ghost/) based on the default theme, [Casper](https://github.com/TryGhost/Casper).

## What does it provide

As it's based on Casper, the general look and feel is the same you would get with it, but we added some features that will enhance your experience using it:

* **Code syntax highlight**: when writing fenced code blocks (those surrounded by accent marks (`` ``` ``) ), you can add the language after the opening quotes, and the HTML output will be highlighted according to the language.
    * If no language is specified, the engine will try to guess it
    * Provided by [Highlight.js](https://highlightjs.org/)
* **Disqus** as a comment system: if you use Disqus as a comment system, you will only need to define your Disqus shortname and it will be all set.
    * The comments will be lazy-loaded only when the user clicks the "Load comments" button, so no unnecessary requests are made
* **Revamped side menu**: the standard side menu felt old and incompleted. W
* **Social profiles**: On the lower part of the new side menu, you will be able to show links to your social profiles. Currently, the ones supported are:
    * Twitter
    * Facebook
    * Github
    * Linkedin

## Why

We liked the Ghost default theme, but we thought it lacked some things, such as Syntax Highlighting or easy integration with a comment system.

## How

Installation instructions

## Customization

For customizing the different options that this theme provides, you will need to go to your Ghost admin panel, open the **Code Injection** section, and on the **Blog Header** add this:

```html
<script type="text/javascript">
  // You variables go here
</script>
```

Any further modification should be made by direct editing of the source code. Feel free to do it!

### Disqus

If you want to use the Disqus comment system, you will need to tell the theme which one is your Disqus shortname.

For doing so, between the script tags you put on the **Blog Header** section, you will need to add the following code:

```javascript
var disqus_shortname = 'YOUR_SHORTNAME';
```

### Social profiles

Those are the variables you will need to define in order to show your social profile links on the side menu:

```javascript
// Github
var github_user = 'dexafree';

```

> ### Note
> Twitter and Facebook profiles will be taken from the blog defaults,defined under the *General* section

## Example

```html
<script type="text/javascript">
    var ga_ua = 'UA-123456-1';
	var disqus_shortname = 'MYSHORTNAME';
    var github_user = 'MYGITHUBUSER';
</script>
```

## Copyright & License

Copyright (c) 2013-2016 Ghost Foundation - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
