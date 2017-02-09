# repo2site

Uses AJAX to build an HTML site from a git repo's MarkDown files

## Usage

Usage is seen in the `index.html` file. Replace the `<body>` tag's `onload`
attribute so that it calls `repo2site` using your username and repo name.
You may also specify the branch name (default: `master`) and the name of the
initial file to load (default: `README.md`).

**Update:** You can now also provide the URL stem for the files to be loaded
via AJAX. You may use the `{repo}` and `{branch}` tokens in your URL stem, and
they will be automatically replaced with the appropriate variables. The current
default is GitHub, but it could be easily adapated for other hosting services.

## Example

The [x84-extras](https://x84-extras.github.io) site uses repo2site to generate
its pages.

## Credits

I'm using [markdown-js](https://github.com/evilstreak/markdown-js) and a
simple, cross-browser, vanilla JS AJAX implementation I found on
[Krasimir Tsonev's blog](http://krasimirtsonev.com/blog/article/Cross-browser-handling-of-Ajax-requests-in-absurdjs)
(which is used in AbsurdJS).
