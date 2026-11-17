# UI tests for the-internet.herokuapp.com

Automated UI tests written with **Python**, **Playwright** and **pytest**.

## Covered pages

Login, logout, checkboxes, dropdown, hovers, inputs, key presses, tables, dynamic controls, add/remove elements.

## Project structure

```
pages/            Page Objects (locators + actions)
tests/            Test files
tests/conftest.py Fixtures that open each page
pytest.ini        pytest configuration
```

## How to run

```bash
pip install -r requirements.txt
playwright install
pytest
```

## Approach

- **Page Object Model:** locators and actions live in page classes; assertions stay in the tests.
- **Fixtures:** each test gets new, already opened page from `conftest.py`.
- **Parametrized tests:** one test covers several inputs (e.g. invalid logins, key presses).
- **Positive and negative cases**, including boundary inputs and error messages.