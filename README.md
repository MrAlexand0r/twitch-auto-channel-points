# Twitch - Auto Claim Channel Points
Bookmarklet that will automatically claim Channel Points

This is a very simple bookmarklet that will periodically detect the "+50 Channel Points" button, if it exists, trigger a click.

1. "Add Page" to your bookmark bar

2. Paste this into the URL field

```
javascript:(function(){setInterval(()=>{var a=document.querySelector(".tw-interactive.tw-button");a?a.click():null},12500)})();
```

3. Open up your favorite streamer then press the bookmark to begin collecting points automatically.
