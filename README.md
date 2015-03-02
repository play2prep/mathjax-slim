# mathjax-slim
A trimmed down version of the MathJax library for general use

Includes the STIX font (Regular variant only) and works well with the following configuration (other configurations may need other files):

<pre>MathJax.Hub.Config({
  tex2jax: {inlineMath: [['$','$'],['\\(','\\)']]},
  jax: ['input/TeX', 'output/HTML-CSS'],
  extensions: ['tex2jax.js']
});</pre>

Because the js files reside in dist/ use the following in bower.json exportOverride if necessary:

<pre>"mathjax-slim": {
    "/": "dist"
}</pre>
