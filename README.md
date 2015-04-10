# mathjax-slim
A trimmed down version of the MathJax library for general use

Includes the STIX font (Regular variant only) and works well with the following configuration (other requirements may need other configurations):

<pre><script type="text/x-mathjax-config">
  if(_.isObject(window.MathJax)) {
    window.MathJax.Hub.Config({
      tex2jax: {
        inlineMath: [
          ['$', '$'],
          ['\\(', '\\)']
        ]
      },
      jax: ['input/TeX', 'input/MathML', 'output/HTML-CSS'],
      extensions: ['tex2jax.js', 'mml2jax.js'],
      messageStyle: 'none'
    });
  }
</script></pre>

Because the js files reside in dist/ use the following in bower.json exportOverride if necessary:

<pre>"mathjax-slim": {
    "js": "dist"
}</pre>
