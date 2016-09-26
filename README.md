# synergie-blog

## Installation

### Requirements
* Python3

### Get the code
```
git clone git@github.com:synergie-asso/website
```

### Virtualenvs
In order to isolate our working environment from other python projects,
we will use virtualenvs. pew is a neat tool to do so.

Install pew:
```
pip install pew
```

Create a new project for the blog
```
pew new -r requirements.txt synergie-blog
```

To quit the virtualenv use Ctrl+D or enter `exit`.

To work on the synergie-blog environment:
```
pew workon synergie-blog
```
You can find in-depth documentation about pew ![here](https://github.com/berdario/pew)

## Pelican

Pelican is static site generator. We use it to build our website.
The articles and pages in the `content` directory are converted to
html to serve as content for the website.

Give the server execution permission:
```
chmod +x develop_server.sh
```

To launch the development server (default port is 8000):
```
./develop_server.sh start
```

The website is now accessible at http://localhost:8000

To stop it:
```
./develop_server.sh stop
```

When the server is running, the html will be automagically updated
at each modification in the `contents`.

## Adding new articles

Refer to ![this section](http://docs.getpelican.com/en/3.6.3/content.html) of
the Pelican documentation.
