# highlightjs-metasploit

**Note: This doesn't work yet because apparently I've done something to
offend Canoncial and I have to rebuild my Ubuntu environment from the
ground up to un-fsck node.js**

This is the first pass at a 3rd party module for a Metasploit language grammar
for Highlight.js. It does the minimal job of making Metasploit Framework
console output /not/ parse as plain text or bash shell text, which it is often
confused with.

About Metasploit: https://metasploit.com

About Highlight.js: https://highlightjs.org/

## Usage

You should be familiar with [Highlight.js
usage](https://highlightjs.org/usage/) first. That said, here's a simple,
underexplained, and probably mystifying example usage, which assumes you're
locally hosting Highlight.js and you have copied the grammar definition from
this repo's `/dist` to your own `highlight-metasploit/dist` dir (just the one
built, minified javascript file is really all you need).

```html
<html>
<head>
<title> hello world </title>
<link rel="stylesheet" href="styles/default.css">
<script src="highlight.pack.js"></script>
<script src="highlight-metasploit/metasploit.min.js"></script>
<script>hljs.initHighlightingOnLoad()</script>
</head>

<body>
<pre><code language="metasploit">

... Metasploit console copypasta goes here ..

</code></pre>

```

