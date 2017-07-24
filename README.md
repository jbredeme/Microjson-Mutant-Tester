# Building a Good Random Test Harness
This test harness when run with the random tester, does not produce any failing tests with microjson.py (assuming microjson.py is correct and has no bugs). Next I want to detect as many bugs that could be introduced into microjson.py as possible found in the mutants subdirectory which has over 400 small variations on microjson.py. Mutants are Python modules that are almost identical, but syntactically modified in some way: these can serve as a way to detect a good test suite. Some of these are trivially different (or just don't work at all), others are different in some very subtle way. The goal is to detect as many of these as possible, with a budget of only 30 seconds testing. Detection means producing a failing test case (ignoring mutants that produce infinite loops).

## Usage
```python
tstl microjson.tstl
tstl_rt
```
## Dependencies
* [Python 2.7.x](https://www.python.org/) - Implementation language.
* [TSTL](https://github.com/agroce/tstl) - Template Scripting Testing Language.

## Author
* **Jarid Bredemeier**

## Resources
* [Template Scripting Testing Language Tool]
* [An introduction to property-based testing]
* [Change history for Coverage]

[Template Scripting Testing Language Tool]: https://github.com/agroce/tstl
[An introduction to property-based testing]: http://fsharpforfunandprofit.com/posts/property-based-testing/
[Change history for Coverage]: https://coverage.readthedocs.io/en/coverage-4.3.4/changes.html
