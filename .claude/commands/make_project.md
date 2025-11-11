Set up a new Python project in the current directory with the following requirements:

* Initialize a Python project using uv (assume it's installed). Use Python 3.11 or later.

Add development dependencies:

* `pytest` for testing, including code coverage
* `black` for code formatting
* `ruff` for linting

Initialize a git repository in the current directory

Add standard files:

* Create a LICENSE file containing the MIT license text. Use the standard template with [year] and [fullname] as placeholders.
* Create a README.md with basic sections: Project Title, Description, Installation, Usage, Testing, License
* Add a {name}/ folder, defaulting to the project name, {slug-kebab-case}. Confirm with user the name.
* Add a tests/ folder and create a dummy pytest: test_ci.py that just asserts True.
* Add GitHub Actions workflows to run the pytest test suite in CI on PR
* Commit all present files with an 'initial commit' message, nothing more, nothing less
* Create a new repository $ARGUMENTS on GitHub using `gh` (assume installed)
* Push the current state
* Verify that CI runs green with the single dummy test

Execute these tasks in order. Use appropriate commands and create necessary configuration files. The project should be ready for development after completion.

For the MIT license, use the standard template with [year] and [fullname] as placeholders.

For the README, include placeholder text that can be filled in later.