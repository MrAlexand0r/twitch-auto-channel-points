# twitch-auto-community-points
Bookmarklet that will automatically collect Community Points

This is a very simple bookmarklet that will periodically detect the "+50 Community Points" button, if it exists, trigger a click.

1. "Add Page" to your bookmark bar

2. Paste this into the URL field

```
javascript:void function(e){var t=function(e){console.log("Loaded"),setInterval(function(){var t=e(".tw-interactive.tw-button");t.length%3F(t.trigger("click"),console.log("Got points")):console.log("Attempted")},12500)},o=e%26%26e.fn%26%26parseFloat(e.fn.jquery)>=1.7;if(o)t(e);else{var n=document.createElement("script");n.src="//ajax.googleapis.com/ajax/libs/jquery/1/jquery.js",n.onload=n.onreadystatechange=function(){var e=this.readyState;e%26%26"loaded"!==e%26%26"complete"!==e||t(jQuery.noConflict())}}document.getElementsByTagName("head")[0].appendChild(n)}(window.jQuery);
```

3. Open up your favorite streamer then press the bookmark to begin collecting points automatically.
