---
layout: post
tags: project emacs
title: "Using EWW on Emacs"
---

Since `eww` stands for [Emacs Web Wowser][eww] (No, I'm not kidding!)
putting Emacs in the title of this piece is redundant. I figured `EWW`
might just not be a term whose definition would easily come to mind. I
couldn't resist `wowser` in any case.

Browsing via `eww` is not particularly useful when I am searching for
a page online. I have `Linux` running in a container on my Chromebook.
The TLDR of this is that I have one terminal to work with. I can use
`Chrome` to search the web on the Chromebook side.

Complicating things for me is that the Chromebook screen reader only
works at a terminal prompt but not in, for example, editors. That's
why I am using `Emacs`. I am using `speechd.el` for speech in the app.

## Using EWW to Read Web Pages Focused on Documentation ##

I have wanted to refer to specific information  contained on a number
of web pages, especially code. Copying this can be tricky. Reviewing
the steps to accomplish tasks is even trickier.

EWW helps here.

1. Activate EWW.

	M-X eww RET

2. At the prompt you can either type keywords for a search or the web
   site address. I can copy the address in `Chrome` and then yank it
   into the prompt with `C-y`.
   
3. The page appears in a buffer. There are a number of actions you can
   take here, but what I do is type `C-x C-w` and then a filename with a `.txt` extension. .

Voila. I have saved the information on the web page. I can now review
it at my leissure and days or weeks later should I need to go back to
it. I can copy commands as needed.

For my own convenience I have created a directory called
`documentation-on-various-topics` where I save these pages.

## Local html browsing ##

In [Setting Up Ablog]({% link _posts/2021-08-15-setting-up-ablog.md %}) I did not show
you how to view your `index.html` files. If your installation is like
mine or you want something quick, `eww` can help. It's a different
command, but the outcome is the same.

	eww-open-file

Enter the filename you want to open as a web page. For example:

		~/posts/_website/index.html

Voila. Here's your web page. It's not as pretty as your regular
	browser would do, but I can spot big errors and then work to fix them.



[eww]: https://www.gnu.org/software/emacs/manual/html_mono/eww.html
.
