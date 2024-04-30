# No-Distraction-Dark-Mode-HTML-Webpage

Sometimes you just need a blank homepage so you can think and chill out in between projects. The HTML page, Title and Favicon are all in dark mode.
There are two parts to this:

✅ HTML Homepage

✅ Favicon


The HTML Webpage uses simple code to create a "dark mode" page. It points to a black colored Favicon, so the tab will be in dark mode as well. The HTML title, which appears on the browser tab, is also blank, with the following code:

```HTML
<title>&#65279;</title>
```

How to setup:

1️⃣ Decide where you will store the two files (HTML and Favicon). I recommend My Documents.
   
2️⃣ Change the below code in the HTML file to reflect the directory where you will store the Favicon:
```HTML
<link rel="shortcut icon" type="image/x-icon" href="/Users/name/Documents/favicon.ico">
```
3️⃣ Put the HTML file in the same directory as the Favicon.

4️⃣ Rename the HTML file as you wish.

5️⃣ In your browser, set the Homepage to the HTML file that you renamed.

6️⃣ Make sure your browser is set to display the homepage icon.

7️⃣ Click the homepage icon and enjoy a few moments of quiet thinking..

Here is the HTML if you want to copy and paste it:

```HTML
<html>
<link rel="shortcut icon" type="image/x-icon" href="/Users/name/Documents/favicon.ico">
<head><title>&#65279;</title></head>
<body bgcolor="black">
</body>
</html>
```

Ideas for forks:

💡 Redirect to HTML pages based on the time. Someone may want two sets of links - one for day (work related) and one for night.
In the below, you create two additional webpages - index-day.html and index-night.html. The code is currently 
set to redirect index-day.html between 6am and 7pm (the 6 and 19 variables). No special code needed for the day and night index pages. Change the links 
as you wish (perhaps to even non-HTML links).

```HTML
<html lang="en">
<head>
<meta charset="UTF-8" />

<title>Links</title>

</head>
<body>
<script type="text/javascript">
// var SpecialRedirectURL = ['night.html','morning.html','day.html','eve.html'];
var SpecialRedirectURL = [
   'index-night.html',
   'index-day.html'
];

function specRedirect() {
  var currentTime = new Date();
  var currentHour = currentTime.getHours();
  var Hour = 0;
  if ( (currentHour >= 6) && (currentHour < 19) ) { Hour = 1; }
//  alert(Hour+' goes to: '+SpecialRedirectURL[Hour]);
  window.location.href = SpecialRedirectURL[Hour];
}  

window.onload = function() {
  specRedirect(); 
}

</script>
</body>
</html>
```

💡 Change the colors.

💡 Add minimalist content like the weather.

💡 Whatever else you can think of..


Enjoy!

