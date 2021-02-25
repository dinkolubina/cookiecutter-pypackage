Cookiecutter PyPackage
======================


[![Tests][tests-badge]][tests-url]

[Cookiecutter](cookiecutter-url) template for a Python package, forked from [briggySmalls/cookiecutter-pypackage](briggySmalls-pypackage-url) which in turn was based on [audreyr/cookiecutter-pypackage](audreyr-pypackage-url).

* GitHub repo: https://github.com/briggySmalls/cookiecutter-pypackage/
* Documentation: https://briggysmalls.github.io/cookiecutter-pypackage/
* Free software: BSD license


Features
--------

This template has all of the features of the original `audreyr/cookiecutter-pypackage`_, plus the following:

* Dependency tracking using poetry_
* Linting provided by both [pylint](pylint-url) and [flake8](flake8-url) [executed by Tox]
* Formatting provided by yapf_ and [isort](isort-url) [checked by Tox]
* Autodoc your code from Google docstring style (optional)
* All development tasks (lint, format, test, etc) wrapped up in a python CLI by [Invoke](invoke-url)

Quickstart
----------

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)::

    pip install -U cookiecutter

Generate a Python package project::

    cookiecutter https://github.com/briggySmalls/cookiecutter-pypackage.git

Then:

* Create a repo and put it there.
* Add the repo to your Travis-CI_ account.
* Install the dev requirements into a virtualenv. (``poetry install``)
* Run the Travis CLI command `travis encrypt --add deploy.password` to encrypt your PyPI password in Travis config
  and activate automated deployment on PyPI when you push a new tag to master branch.
* Add the repo to your [Read the Docs](read-the-docs-url) account + turn on the Read the Docs service hook.
* Release your package by pushing a new tag to master.
* Get your code on! 😎 Add your package dependencies as you go, locking them into your virtual environment with ``poetry add``.
* Activate your project on [pyup.io](pyup-url).

For more details, see the [cookiecutter-pypackage tutorial](original-pypackage-tutorial-url) 


<!-- Markdown link & img dfn's -->
[tests-badge]: https://github.com/dinkolubina/cookiecutter-pypackage/actions/workflows/tests.yml/badge.svg
[tests-url]: https://github.com/dinkolubina/cookiecutter-pypackage/actions/workflows/tests.yml
[invoke-url]: http://www.pyinvoke.org/
[isort-url]: https://pypi.org/project/isort/
[yapf-url]: https://github.com/google/yapf
[flake8-url]: https://pypi.org/project/flake8/
[pylint-url]: https://www.pylint.org/
[poetry-url]: https://python-poetry.org/
[tox-url]: http://testrun.org/tox/
[sphinx-url]: http://sphinx-doc.org/
[pyup-url]: https://pyup.io/
[bump2version-url]: https://github.com/c4urself/bump2version
[PyPi]: https://pypi.python.org/pypi
[read-the-docs-url]: https://readthedocs.io/
[briggySmalls-pypackage-url]: https://github.com/briggySmalls/cookiecutter-pypackage/
[briggySmalls-pypackage-tutorial-url]: https://briggysmalls.github.io/cookiecutter-pypackage/tutorial.html
[cookiecutter-pypackage-url]: https://github.com/audreyr/cookiecutter-pypackage
[cookiecutter-url]: https://github.com/audreyr/cookiecutter/