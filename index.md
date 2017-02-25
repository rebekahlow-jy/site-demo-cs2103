<link rel="stylesheet" href="css/main.css">

<navbar placement="top" type="default">
    <a slot="brand" href="index.html" title="Home" class="navbar-brand">CS2103/T</a>
    <li><a href="index.html">Schedule</a></li>
    <li><a href="textbook.html">Textbook</a></li>
    <li><a href="handbook.html">Handbook</a></li>
</navbar>

<div class="website-content">
<include src="contents/overview/index.html" />
<include src="contents/week1/index.html" />
<include src="contents/week2/index.html" />
</div>

<div id="disqus_thread"></div>

<script>
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = '//cs2103.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>

<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
