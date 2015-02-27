# mathjax-slim
A trimmed down version of the MathJax library for general use

Includes the STIX font (Regular variant only) and works well with the following configuration (other configurations may need other files):

<pre>MathJax.Hub.Config({
  tex2jax: {inlineMath: [['$','$'],['\\(','\\)']]},
  jax: ['input/TeX','output/HTML-CSS', 'output/CommonHTML'],
  extensions: ['tex2jax.js','MathMenu.js','MathZoom.js', 'CHTML-preview.js'],
  TeX: {
    extensions: ['AMSmath.js','AMSsymbols.js','noErrors.js','noUndefined.js']
  },
  MatchWebFonts: {
    matchFor: {
      'HTML-CSS': true
    }
  }
});</pre>
