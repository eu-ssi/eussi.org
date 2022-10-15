# EuSSI website

The sources behind <https://eussi.org>.

Templates and Sass sources adapted from https://github.com/bennetthardwick/simple-dev-blog-zola-starter
(MIT license).


### How this works

The website sources are hosted on GitHub (here) and the website is deployed via
GitHub pages.

The source code resides on the `main` branch and upon every change (merged
pull request), it auto-generates the `gh-pages` branch which containes the
generated HTML code.

The HTML code is generated using [Zola](https://www.getzola.org/) static site
generator.

To edit content, you most of the time only need to edit Markdown files.
[Zola](https://www.getzola.org/) auto-generates HTML from these.


### How to contribute changes

To add/edit content, modify files inside the [content](content) folder. You can modify
these via the web or by opening pull requests.

If you want to add new pages to the navigation bar or modify the navigation
bar, modify `navigation` in [config.toml](config.toml).

You can change the looks inside the [sass](sass) folder if you know your way
around CSS/Sass.

You can modify the page layouts by editing files inside the [templates](templates) folder.

To add data to the consortium team and organizations page, please edit
<content/consortium/people.yaml>
and
<content/consortium/organizations.yaml>.

Don't hesitate to ask [Radovan Bast](mailto:firstname.lastname@uit.no) for help with
how to implement some changes that you have in mind.


### How to preview changes locally

Install [Zola](https://www.getzola.org/), then run:
```
$ zola serve
```


### Why Zola and not X?

Radovan: sorry, personal choice but I have been working with a number of static
site generators and this one stands out in terms of design, good defaults,
folder layout, functionality, and minimal dependencies.

But like any other static site generator, we will mostly only need to edit
Markdown files.  I can help with everything else.

And also no problem to migrate to something else if that simplifies
maintenance.  This was just to get something up on the web.
