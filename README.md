# EuSSI website

The sources behind <https://eussi.org>.


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

You can modify the page layouts by editing files inside the [templates](templates) folder.

To add data to the team and organizations page, please edit
[content/network/people.yaml](content/network/people.yaml)
and
[content/network/organizations.yaml](content/network/organizations.yaml).

Don't hesitate to ask [Radovan Bast](mailto:firstname.lastname@uit.no) for help with
how to implement some changes that you have in mind.


### How to preview changes locally

Install [Zola](https://www.getzola.org/). Or you can download the binary from
[here](https://github.com/getzola/zola/releases).

Then run:
```console
$ zola serve
```


### Why Zola and not X?

Radovan: Sorry, personal choice but I have been working with a number of static
site generators and this one stands out in terms of design, good defaults,
folder layout, functionality, and minimal dependencies.  And also no problem to
migrate to something else if that simplifies maintenance.  This was just to get
something up on the web.

But like any other static site generator, we will mostly only need to edit
Markdown files.  I can help with everything else.
