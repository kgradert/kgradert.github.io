---
layout: post
title: 'Global Notes: Password-Protected Jekyll Collections'
category: DH
tags: notes
published: false
---

I'm soon moving to Germany for a postdoc, where I'm hoping to finish my current book project. But like any book project, mine is built atop a mountain of other books, and I tend to fill them with detailed notes about each author's argument. That is, I need my books to write my own. How to tote them all overseas? My stinginess spurns shipping costs.

So I've begun to transcribe all these notes and quotes into markdown files (my go-to for nearly all of my writing). But this raised the question of access and formatting. I could just leave a folder full of .md in my Dropbox, but I preferred to have all of my notes localized on my personal website, with matched styling.

Jekyll's collections feature works well for a project like this. Jfx has a good [tutorial](http://jxf.me/entries/custom-collections-jekyll/) on how to set these up.

But the prospect of displaying personal research notes for all the Internet to see is about as attractive as nude public speaking. Jekyll stores each collection in its own folder, which you can then password-protect by dropping in two wee htaccess and htpasswd files. I like AddedByte's [tutorial](https://www.addedbytes.com/blog/code/password-protect-a-directory-with-htaccess/). (A tip: the path you enter in the htaccess file to point it to the htpassword file is not intuitive. You can find the correct path by dropping a phpinfo file into the folder you wish to protect. See Media Temple's [tutorial](https://mediatemple.net/community/products/dv/204643880/how-can-i-create-a-phpinfo.php-page).) If you're hosting a Jekyll site on Github, this won't work. But it's the simplest method I've found for moderate privacy on a regularly hosted website.

After setting up a password-protected Jekyll collection, I can simply write my notes as markdown, use a single Jekyll command to turn them into handsome htmls, then upload them to my domain. Quick, centralized, and easy on the eyes.
