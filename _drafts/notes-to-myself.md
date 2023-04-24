# Notes to Myself #

1. For referencing other blog posts in the `ablog`html build:
<pre>[this blog post](this-blog-post/)</pre>
2. To serve my pages locally:
   A. Open terminal from the Launcher on my chromebook: alt+shift+l
   B. Change directory to where the html is, e.g. `~/post/_website/`
   C. Type the command:
      <pre>python3 -m http.server</pre>
The website is served at localhost:8000`. ctrl+c kills the server.
3. With speech, move to the beginning of the line is C-a and move to
   the end of the line is C-e C-e. To move bysentence is M-a
   (backwards) and M-e (forwards.
4. `pandoc` can process multiple files as input to create one file:
   `pandoc -o single.md *.md`
