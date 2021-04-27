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

# Related

* [Güttli's opinionated Django Tips](https://github.com/guettli/django-tips)

# WOL

More of [Güttli Working Out Loud](https://github.com/guettli/wol)
