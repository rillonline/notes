---
blogpost: true
category: Tech
location: Earth
date: August 29, 2021
---

# Displaying Date and Time in Emacs #

{sub-ref}`wordcount-minutes` min read  
{sub-ref}`wordcount-words` words 

I so enjoy working in Emacs on my Chromebook.  This prompts me to
investigate how to get more information so I don't have to switch over
to the Chrome side for web searches. As I have explained in [Using EWw
on Emacs](using-eww-on-emacs/) I try to read so much more of these web
pages on the Linux side, especially those pages which I will refer
back to over and over again.

After switching from `emacspeak` to `speechd.el` I have missed some
functionality. One of the things I have missed is checking the time.
Of course I have my watch, my phone and the status display on the
launcher on the Chrome side, but I was convinced it should be possible
to get this information without leaving Emacs.

And I can!

The key combination `C-c RET` reads the mode line in Emacs with
`speechd.el`. I added these two lines to `init.el` to have the date
and time placed there:

    '(display-time-day-and-date t)
    '(display-time-mode t)

Voila! I can use `C-e RET` to hear the day of the week, the date and
the time. No flipping about.

```{note}
Other information in the mode line will be read also.
```
