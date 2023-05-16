---
title: Web Console Chat - Profanity in the browser
date: 2023-05-16T15:00+07:00
author: Trần H. Trung

---

As the owner of a tiny public XMPP service, I use Profanity daily.

After lots of effort to set up the webchat service the way I want, I
eventually gave up with all the web-dev frameworks as they are all way too
complex with countless dependencies that even the main developers of those
projects can't seem to keep track of. So I looked for alternative: Can I use
« Profanity » the same piece of software that I use for my webchat services? 

I search around the net and turns out it is extremely easy to offer a terminal
to the browser with [ttyd.](https://tsl0922.github.io/ttyd/)

But Profanity is a really powerful client which not only offers very
customized configurations but also allow user to read, write, execute any
other scripts and|or programs at will. So the question became: How can I serve
Profanity that is running on my server to the public so that my whole
infrastructure wouldn't just vanish when people `/system exec rm -rf /`

In the process of answering that, I realized that Profanity is not the one and
only console client out there; and those software would probably need some
similar treatments.

Thus, the birth of [Web Console Chat:](https://soft.trung.fun/webcc/webcc.html)
an installation guide and a collection of patches to make sure existing XMPP
console clients would be safe enough before serving them to the web.
I use Profanity (obviously) so there is currently only one patch for the latest
stable release. But contributions are always welcome!

