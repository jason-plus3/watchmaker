# Contributing

Contributions are welcome, and they are greatly appreciated! Every little bit
helps, and credit will always be given.

## Bug reports

When [reporting a bug](https://github.com/plus3it/watchmaker/issues)
please include:

*   Your operating system name and version.

*   Any details about your local setup that might be helpful in
    troubleshooting.

*   Detailed steps to reproduce the bug.

## Documentation improvements

Watchmaker could always use more documentation, whether as part of the official
Watchmaker docs, in docstrings, or even on the web in blog posts, articles, and
such.

## Feature requests and feedback

The best way to send feedback is to file an issue at
<https://github.com/plus3it/watchmaker/issues>.

If you are proposing a feature:

*   Explain in detail how it would work.

*   Keep the scope as narrow as possible, to make it easier to implement.

*   Remember that this is a volunteer-driven project, and that code
    contributions are welcome :)

## Development

To set up `watchmaker` for local development:

1.  Fork [watchmaker](https://github.com/plus3it/watchmaker) (look for the
    "Fork" button).

2.  Clone your fork locally::

```shell
git clone https://github.com/your_name_here/watchmaker.git
```

3.  Create a branch for local development:

```shell
git checkout -b name-of-your-bugfix-or-feature
```

   Now you can make your changes locally.

4.  When you're done making changes, run all the checks, doc builder and spell
checker with [tox](http://tox.readthedocs.org/en/latest/install.html) one
command:

```shell
tox
```

5.  Commit your changes and push your branch to GitHub:

```shell
git add .
git commit -m "Your detailed description of your changes."
git push origin name-of-your-bugfix-or-feature
```

6.  Submit a pull request through the GitHub website.

## Pull Request Guidelines

If you need some code review or feedback while you're developing the code just
make the pull request.

For merging, you should:

1.  Include passing tests (run ``tox``).
2.  Update documentation when there's new API, functionality etc.
3.  Add a note to ``CHANGELOG.rst`` about the changes.
4.  Add yourself to ``AUTHORS.rst``.

> If you don't have all the necessary python versions available locally you
> can rely on Travis - it will [run the tests](https://travis-ci.org/plus3it/watchmaker/pull_requests)
> for each change you add in the pull request. It will be slower though...

## Tips

To run a subset of tests:

```shell
tox -e envname -- py.test -k test_myfeature
```

To run all the test environments in _parallel_ (you need to `pip install
detox`):

```shell
detox
```