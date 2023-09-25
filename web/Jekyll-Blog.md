---
layout: default
title: Jekyll Blog 
---
# Jekyll Blog

## Starting and stopping the server (running it locally)
Start the server: `jekyll serve`<br>
It will automatically rebuild the website, putting the files into \_site, whenever you save a change to your files.<br>
This command works, when you don't have a Gemfile.

Better yet, start the server AND make the browser refresh every time you make an edit to a file: `jekyll serve --livereload`

Stop the server: `Ctrl - C`

Start over (delete cache and the \_site folder, which contains the generated website files):<br>
`jekyll clean`<br>
Useful when you modify \_config.yml.

To see your website locally, go to:
`http://localhost:4000/index.html`

## About Jekyll
Jekyll helps make static websites.

**Static websites** appear the same to every user.  Static websites can still use JavaScript, have clickable buttons, play CSS animations and video, allow downloads, and use forms.  But the server will always serve up the same page to everyone.

Jekyll accepts HTML or Markdown files.<br>
It converts the Markdown into HTML, uses CSS, and processes Liquid code (eg to insert the Page or Post content into a Layout template file).

It outputs HTML files to the \_site folder.  These files can be 
hosted on a website.  Or all the unprocessed files can be pushed to a GitHub Pages repo, where GitHub will automatically run Jekyll, generate the static web pages, and publish the GitHub Pages.

[Jekyll Docs](https://jekyllrb.com/docs/)

## Layouts (aka Templates)
Jekyll lets you use layout templates.
Store them in \_layouts directory


Layout templates have:

`{ { c o n t e n t } }`  which will be replaced by the content of each post.

## Posts and Pages
Posts and pages will have front matter at the very top of the file.
<h4>Front Matter</h4>
- Begins and ends with `---` (3 hyphens)
- A list of properties in key: value format
- Property name can be anything.
- These properties are used in layout files.
- When Jekyll tries to generate the HTML output, it will use these properties and perform substitutions in the layout files.

Default post naming pattern:<br>
YYYY-MM-DD-post-title.html

## \_config.yml
_ config.yml defines global properties<br>
`permalink: /:title`<br>
This shortens the URL of the post, so it includes only the title and not the date.

## Liquid
- [Docs](https://shopify.github.io/liquid/)
- Jekyll uses this template language.
- Add conditionals and loops to control what HTML is generated.
- Add variables, like site.posts, post.title or post.url.
- `{  % %  }` surrounds the Liquid code.

<img class="large_picture" src="/images/Jekyll.png" />
