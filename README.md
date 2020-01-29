# My_Syntax_Highlighter
Syntax Highlighter Bloger

## Add syntax highlighting to my Blog

March 01, 2017

Many websites like this one feature a bunch of code snippets, which can be a pain when changing the theme, as you might have manually styled the code chunks. To avoid this, you can add the highlightjs library that does it for you - that way, when you change theme, you only need to tweak one gadget (instead of all of your posts and their snippets.)

To add the needed JS and CSS, you can click the button below! The content of the gadget is shown below.


Alternatively, you can head to the Layout tab for your blog, and add an HTML/Javascript gadget, with the following in the Content area.

```HTML
<link rel="stylesheet"href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.9.0/styles/androidstudio.min.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.9.0/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>
```

In this example, we're using the androidstudio style, but there's a big bunch of different themes which you can replace the first line CSS link with.

Note that this highlighting library requires your post's HTML to wrap the relevant code snippets in a code tag, with the code tag having the class of the relevant language. For example, these snippets use

```HTML
<pre><code class='html'> [My HTML goes here] </code></pre>
```
Also note that you'll need to escape the HTML content, which is done by default when you paste into the Compose mode of the editor. So generally, it's easier to add your snippets first, then wrap them in the required pre and code tags by switch to HTML mode of the editor, just as a final touch before publishing your post.

Happy snippeting!
