# Web Development

This is an opinionated list about web development

# Chrome devtools

Use Chrome. The [devtools](https://developers.google.com/web/tools/chrome-devtools) are great.

In the network-tab of the devtools enable "Slow 3G" from time to time to see how your page behaves on slow networks.

ctrl-shift-i Inspect element. Three dots: Store in global variable: temp1. Then in console: temp1.classList.add('foo')

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
<script src="https://unpkg.com/htmx.org@1.1.0" integrity="sha384-JVb/MVb+DiMDoxpTmoXWmMYSpQD2Z/1yiruL8+vC6Ri9lk6ORGiQqKSqfmCBbpbX" crossorigin="anonymous"></script>
```

[SRI Hash Generator](https://www.srihash.org/)


# JS Libraries

## tom-select


https://tom-select.js.org/

> Tom Select is a versatile and dynamic <select> UI control. With autocomplete and native-feeling keyboard navigation, it's useful for tagging, contact lists, country selectors, and so on. Tom Select was forked from selectize.js with four main objectives: modernizing the code base, decoupling from jQuery, expanding functionality, and addressing issue backlogs.

# Related

* [Güttli's opinionated Django Tips](https://github.com/guettli/django-tips)

# WOL

More of [Güttli Working Out Loud](https://github.com/guettli/wol)
