# Web Development

This is an opinionated list about web development

# Chrome devtools

Use Chrome. The [devtools](https://developer.chrome.com/docs/devtools) are great.

In the network-tab of the devtools enable "Slow 3G" from time to time to see how your page behaves on slow networks.

ctrl-shift-i Inspect element. Three dots: Store in global variable: temp1. Then in console: temp1.classList.add('foo')

`$(...)` is the shortcut for `document.querySelector(...)`.

You want to debug something which is only visible if you hover it? Catching this might not be possible with the normal element selection. But you can use (in Element Tab) "Break on" "subtree modifications"

# Fast feedback cycle

To get CSS right, I often change the CSS via Chrome devtools and not via IDE. After I found the matching CSS I copy it to my IDE. This
gives me a faster edit-check feedback cycle.

# Avoid "Modal Dialog"

Use inline-edit or a new page.

# Create simple APIs for testing

You want to share an idea or problem with other people. For example in a Github issue or a
StackOverflow question. But you sample code needs a server to make it reproduceable?

[mocky](https://designer.mocky.io/) is a simple service to generate static responses.

# html fragments over the wire

There are alternatives to modern frontend libraries like React/Vue: [htmx](//htmx.org). Just
send HTML fragments over the wire. It is simple and fast.

# SRI Hash Calculator

If you use a third party library via a CDN, then use a hash, so that you are safe if the CDN got hacked.

Example:

```
<script src="https://unpkg.com/htmx.org@1.4.1/dist/htmx.min.js" 
        integrity="sha384-1P2DfVFAJH2XsYTakfc6eNhTVtyio74YNA1tc6waJ0bO+IfaexSWXc2x62TgBcXe" 
        crossorigin="anonymous"></script>
```

[SRI Hash Generator](https://www.srihash.org/)

# Download via http-GET, not http-POST

There is a very old bug in Chromium which makes troubles if you want to download a PDF
which the browser receive via http-POST: https://bugs.chromium.org/p/chromium/issues/detail?id=158957

This means you should sent PDF (and other formats the user might want to "save as") via http-GET, not http-POST.

# `<br>`

Use `<br>`, not `<br />` or other outdated ways to create a line-break.

HTML is not a subset of XML.

Same for `<li>`: No need to close it.

> An li element's end tag can be omitted if the li element is immediately followed by another li element or if there is no more content in the parent element.

Source: https://html.spec.whatwg.org/multipage/grouping-content.html#the-li-element

# Tunnel for localhost

I want to provide a customer/product-owner/team-mate the current state of your work? Some companies have solved this, and you can easily create feature systems. Many companies have not solved this yet.

You can help yourself with a tunnel. There are many options. See [awesome tunneling](https://github.com/anderspitman/awesome-tunneling)

And don't forget to speak up and engage, so that your employer provides a solid solution. Tunneling to localhost is just a dirty work-around. If you switch off your laptop because you commute by train, then you customer/product-owner/team-mate  won't be able to access the system.


# JS Libraries

## tom-select


https://tom-select.js.org/

> Tom Select is a versatile and dynamic `<select>` UI control. With autocomplete and native-feeling keyboard navigation, it's useful for tagging, contact lists, country selectors, and so on. Tom Select was forked from selectize.js with four main objectives: modernizing the code base, decoupling from jQuery, expanding functionality, and addressing issue backlogs.


# Related

* [Güttli's opinionated Django Tips](https://github.com/guettli/django-tips)

# WOL

More of [Güttli Working Out Loud](https://github.com/guettli/wol)
