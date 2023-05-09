---
permalink: /index.html
---

# SECO-ASSIST sources

[![Deployment](https://github.com/secoassist/secoassist.github.io/workflows/deploy.yaml/badge.svg?branch=sources)](https://github.com/secoassist/secoassist.github.io/actions/workflows/deploy.yaml)

This website is built with [Genja](https://github.com/AlexandreDecan/Genja).
It is built on top of [Jinja2](https://jinja.pocoo.org/docs/latest/), a powerful template engine written in Python. The layout of the website relies on [Bootstrap 3](https://getbootstrap.com/docs/3.3/).

Any modification or pull request should be done on the "sources" branch. Every commit done in the sources branch triggers an automatic build by Genja, and an automatic deployment to GitHub pages (ie. the content of the output folder will be deployed). Notice that any "invalid" modification (ie. any modifications that lead to something that cannot be processed by Genja) will not be deployed. The status badge in this README file informs you of the status of the latest build.

If you want to locally test your modifications before pushing them, go to the Genja repository and download both ``genja.py`` and ``requirements.txt``. The script requires Python >= 3.5, and some dependencies that can be easily installed using ``pip install -r requirements.txt``. Then simply type ``python genja.py`` at the root of this repository to build the pages.
