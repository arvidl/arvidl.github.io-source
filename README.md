# Source for http://arvidl.github.io
This repository contains the source for my Computational Medicine blog http://arvidl.github.io/. <br>
Based on: $ git clone https://github.com/jakevdp/jakevdp.github.io-source.git

## Building the Blog

Clone the repository & make sure submodules are included

```
$ git clone https://github.com/arvidl/arvidl.github.io-source.git
$ git submodule update --init --recursive
```

Install the required packages:

```
$ # conda create -n pelican-blog python=3.5 jupyter notebook
$ conda create -n pelican-blog python=3.7 jupyter notebook
$ conda activate pelican-blog
$ pip install pelican Markdown ghp-import
```

Edit content (e.g. using ~~Remarkable~~  `atom` with Markdown Preview)

```
$ cd content/articles
$ atom yyyy-mm-dd-<blogpost>.md
```

Build the html and serve locally:

```
$ make html
$ make serve
$ open http://localhost:8000
```

Add, commit and push changes (to arvidl.github.io-source)

```
$ git add .
$ git commit -m "<info on changes>"
$ git push origin master
```

Deploy to github pages (on arvidl.github.io)

```
$ make publish-to-github
# or
$ make publish-to-github-force
```

Comments (Disqus)

https://arvidl-github-io.disqus.com/admin/settings/general/
