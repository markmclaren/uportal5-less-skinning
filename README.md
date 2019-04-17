uPortal 5 uses a Bootstrap 3 based skin (called Respondr).  It also uses Less for producing custom skins.

See: http://jasig.github.io/uPortal/implement/frontend/SKINNING_UPORTAL.html

I am developing a new skin.  I wanted a quick way to see the effect of editing the Less variables in the browser without having to rebuild and redeploy the uPortal after every change.  So I copied the front page of the uPortal-demo and edited it slightly.

I used [Less.js in the browser](http://lesscss.org/usage/#using-less-in-the-browser).
This repository also includes Bootstrap source code (I think 3.4.1) which also uses Less.  

To see this working, either you need to view index.html in Firefox or access it in Chrome via a simple web server (maybe use Python's http.server or Node's http-server) - so that it is available at:

http://localhost:8080/index.html

You should then be able to edit "*respondr/newskin/less/variables.less*" and Ctrl-F5 reload the page to see the effect of your change almost immediately (Less.js then converts the less file to CSS in the browser).

A good place to start is changing the value of **@color1**.