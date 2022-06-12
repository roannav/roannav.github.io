---
layout: default
title: GitHub Profile or GitHub Project README vs. GitHub Pages
---

# GitHub Profile and Project README.md vs GitHub Pages

## GitHub Profile README.md and Project README.md

Your GitHub Profile is at<br>
https://github.com/{GitHub username}/{GitHub username}/README.md

Your repo project README.md is at<br>
https://github.com/{GitHub username}/{GitHub repo name}/README.md

README.md are written in GitHub flavored markdown, so there are some limitations.

Can add images, GIFs, SVGs, and emojis.

Can use some HTML (but not input, textarea, or button).  

No CSS.  However, there are 2 hacks to get around this:<br>
- You can make images float to the right, by setting<br>
&lt;img align=&quot;right&quot;&gt;.  
- You can add a &lt;style&gt; tag and CSS code by encapsulating it in SVG and foreignObject.

No JavaScript.


## GitHub Pages

Your main GitHub Page is at<br>
https://{GitHub username}.github.io/index.html (or index.htm or index.md)

For a repo project, the main GitHub Page is at<br>
https://{GitHub username}.github.io/{GitHub repo name}/index.html (or index.htm or index.md)

Can use HTML, CSS, and JavaScript, like a regular web page.


<img class="large_picture" src="/images/GitHub-Octocat.png" />
