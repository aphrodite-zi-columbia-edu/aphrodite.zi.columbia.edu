# aphrodite.zi.columbia.edu

Static Website at Aphrodite Server for Lomvardas Lab in Zuckerman Institute @ Columbia University.

## Development

To run site locally:

```bash
git clone https://github.com/aphrodite-zi-columbia-edu/aphrodite.zi.columbia.edu.git
bundle install  # if not already installed
bundle exec jekyll serve
```

And the program will produce a url for previewing the site in the terminal output. For more information on getting [Jekyll](https://jekyllrb.com/) installed or first time usage, reach out or [read their docs](https://jekyllrb.com/docs/quickstart/).

To publish, copy these files into the folder found in nginx configuration on the server. The location of these files is described [here](http://nginx.org/en/docs/beginners_guide.html), for ssh access reach out. (TODO: make git hooks to publish on push to branch)

To view a static copy of the site on a computer without a Ruby interpreter but with a Python one, use:

```bash
cd /path/to/_site/
python -m SimpleHTTPServer 8000
```

and navigate to `http://localhost:8000/` in your browser. as described in the last line of [this document](https://docs.python.org/2/library/simplehttpserver.html).
