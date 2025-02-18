# HTML Links

## Learning Goals

1. Recognize how `a` tags are structured and implemented
2. Create different types of links with the `a` tag

## Introduction

Links, also known as _hyperlinks_, put the _web_ in _World Wide Web_: many
millions of HTML pages, connected together through _links_. In this lab, we will
be discussing links in HTML and applying what we've learned.

## Recognize How `a` Tags Are Structured And Implemented

### The Anchor Link Tag

To create a link, we use the _anchor link_ tag, written as `<a>`.
The `<a>` tag requires two things:

* An `href` attribute to tell the browser where we want the link to go to.
* Some sort of text or content that the `<a>` tag can wrap around, becoming the
link text. This includes images!

```html
<a href="https://www.google.com">Google</a>
```

The example above, when displayed in the browser, by default, would show
[Google](google.com) in blue and underlined. If this were on a website, clicking
it would _redirect_ the user, changing the current browser window URL to
_google.com_.

The `href` attribute in this example, is a full link, also known as an
**absolute** path. Alternatively, we can also use a _relative_ path, which is
used when we want to link to a separate file on the same website:

```html
<a href="about.html">About Page</a>
```

Say this link was on `index.html`, the home page of a website you had built.
When a site visitor clicks the above link, the browser knows to look for a file
called `about.html` that is located in the same folder as `index.html`.

### The Target Attribute

The `target` attribute can be added along side `href` and has a specific use:
setting this attribute to be `target='_blank'` will cause the browser to open a
new tab when the link is clicked, instead of changing the current page you are
on:

```html
<a href="https://www.google.com" target="_blank">Google</a>
```

## Create Different Types of Links With the `a` Tag

Let's practice creating links. Take a look at `index.html` for some additional
guidance. To complete this lab you must:

* Write one absolute path link and one relative path link
* Wrap the provided image in a link tag

For the relative path link, there is a second HTML file, `about.html`, that can
be used as the value in the `href` attribute.

Run `learn test` and follow along with the test errors. Open `index.html` in the
browser to see the results of your code as you work.

## Conclusion

To recap what we've learned, links can:

* Connect a user to a separate website
* Connect a user to another page on the same website
* Open up a new browser tab, using `target`

Links connect individual web pages together, and collectively create what we
know as the _web_.
