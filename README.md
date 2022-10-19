# Free1040
The best in-browser, privacy respecting 2022 1040EZ application using minimal html, css, svg, and javascript. Inspired by a [Hacker News comment](https://news.ycombinator.com/item?id=33269215) where someone said:

```
Oh, I don't know, if the data-structure was easy to understand (and contribute to) it might be fun to have a comprehensive representation of the tax code to play with. It's also a problem that lends itself to "local first" attempts - I can see an individual might try to encode rules about their local sales tax and property taxes.

Another approach would be to have a programming competition to see who can write the best in-browser, privacy respecting 2022 1040EZ application using nothing but html, css, svg, and javascript[0]. The end product should be capable of saving its state as a single json object, and producing a usable PDF. One might host such an application as a public utility. A good test suite would model the 1040 historically to make sure the app can reach all states characteristic of the problem, and produce the correct result. On macos you might want to bundle it all in an app, include Chrome, the resources, the data and any generated PDFs.

This would be relatively low-effort and could have real impact on, e.g., TurboTax. Heck, I'd use it. I bet a lot of people here would. Here (https://github.com/b-k/1040.js) is one person who took a serious stab at a part of this, the calculations themselves!

0 - Someone is also taking a stab at this: https://github.com/Free1040/Free1040 
```

## Prior work

[1040.js](https://b-k.github.io/1040.js/) ([github](https://github.com/b-k/1040.js)) is a programmatic representation of the tax code using a technique which uses python with extensive use of the m4 macro language. 
However it is also written in an interesting "reactive" style using "Cells" that seems like a very good idea.

Browsers can generate PDFs from html (and svg) reliably and fast using the "Print to PDF" function.

The ideal tax form archive would have 3 files in it: the form html, a data json, and optionally a browser, or a virtual machine image.
