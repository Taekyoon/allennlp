# Contributing

Thanks for considering contributing!  We want AllenNLP to be *the way* to do cutting-edge NLP research, but we cannot
get there without community support.

## How Can I Contribute?

### Did you find a bug?

First, do [a quick search](https://github.com/allenai/allennlp/issues) to see whether your issue has already been reported.
If your issue has already been reported, please comment on the existing issue.

Otherwise, open [a new GitHub issue](https://github.com/allenai/allennlp/issues).  Be sure to include a clear title
and description.  The description should include as much relevant information as possible.  The description should
explain how to reproduce the erroneous behavior as well as the behavior you expect to see.  Ideally you would include a
code sample or an executable test case demonstrating the expected behavior.

### Did you write a fix for a bug?

Open [a new GitHub pull request](https://github.com/allenai/allennlp/pulls) with the fix.  Make sure you have a clear
description of the problem and the solution, and include a link to relevant issues.

Once your pull request is created, our continuous build system will check your pull request.  Continuous
build will test that:

* [`pytest`](https://docs.pytest.org/en/latest/) All tests pass
* [`pylint`](https://www.pylint.org/) accepts the code style (our guidelines are based on PEP8)
* [`mypy`](http://mypy-lang.org/) typechecks the Python code
* The docs can be generated successfully
* Test coverage remains high.  Please add unit tests so we maintain our code coverage.

If your code fails one of these checks, you will be expected to fix your pull request before it is considered.

You can run most of these tests locally, which will be faster than waiting for cloud systems to run tests.  To see
exactly what our continuous build system runs, look at `.travis.yml`.  The most common checks you should run
locally are:

* `pytest -v`.  If you run this in the root AllenNLP directory, this will run all of our tests.
* `./scripts/pylint.sh`.  This will make sure your code conforms to our automatically-checkable style guidelines.
* `./scripts/mypy.sh`.  This will run the mypy typechecker over the code.

### Do you have a suggestion for an enhancement?

We use GitHub issues to track enhancement requests.  Before you create an enhancement request:

* Make sure you have a clear idea of the enhancement you would like.  If you have a vague idea, consider discussing
it first on the users list.

* Check the documentation to make sure your feature does not already exist.

* Do [a quick search](https://github.com/allenai/allennlp/issues) to see whether your enhancement has already been suggested.

When creating your enhancement request, please:

* Provide a clear title and description.

* Explain why the enhancement would be useful.  It may be helpful to highlight the feature in other libraries.

* Include code examples to demonstrate how the enhancement would be used.
