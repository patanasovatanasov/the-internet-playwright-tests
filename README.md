UI tests for the-internet.herokuapp.com

Tech stack: Python, Playwright, pytest

The following pages are covered: login, checkboxes, hovers, dropdown, inputs, 
tables, logout, key presses, dynamic controls, add and remove elements

Structure: pages/ : page objects, tests/ : tests, conftest.py : fixtures

How to run: 
pip install -r requirements.txt
playwright install
pytest

Approach: This tests are for personal exercise purposes in which I learned how to use Page Object Model (POM), fixtures and parametrized tests. 