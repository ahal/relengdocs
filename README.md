[![Docs](https://readthedocs.org/projects/moz-releng-docs/badge/?version=latest)](https://moz-releng-docs.readthedocs.io/en/latest/?badge=latest)

# Mozilla Release Engineering Documentation

This repository contains some of the more technical internal documentation for Mozilla Release
Engineering.

Rendered versions of the documentation may be viewed at:
  http://moz-releng-docs.readthedocs.io/en/latest/

## Contributing

1. Create a Python [virtualenv](https://docs.python.org/3/tutorial/venv.html)
2. Run:

    pip install -r requirements/base.txt

3. To build the docs locally, run:

    make html

Verify changes by viewing `_build/html/index.html` in your browser.

Note: Any new docs should be directly or indirectly linked to from `index.rst`. (For example, if
`index.rst` contains `balrog/index.rst` in its
[toctree](https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-toctree),
and the new doc is in the `balrog/index.rst` toctree, then the new doc is successfully indirectly
linked.)

## Reference

These docs use [reStructuredText](https://en.wikipedia.org/wiki/ReStructuredText) and
[Sphinx](https://www.sphinx-doc.org/en/master/index.html). Here are some reference materials:

* [reStructuredText primer](https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html)
* [Sphinx roles](https://www.sphinx-doc.org/en/master/usage/restructuredtext/roles.html)
* [Sphinx domains](https://www.sphinx-doc.org/en/master/usage/restructuredtext/domains.html)