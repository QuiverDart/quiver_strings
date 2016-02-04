Quiver strings
==============

A set of string utilities for Dart.

[![Build Status](https://travis-ci.org/QuiverDart/quiver_strings.svg?branch=master)](https://travis-ci.org/QuiverDart/quiver_strings)
[![Coverage Status](https://img.shields.io/coveralls/QuiverDart/quiver_strings.svg)](https://coveralls.io/r/QuiverDart/quiver_strings)

## Documentation

[API Docs](http://www.dartdocs.org/documentation/quiver_strings/latest)

`isBlank` checks if a string is `null`, empty or made of whitespace characters.

`isEmpty` checks if a string is `null` or empty.

`isNotEmpty` checks if a string is not `null` and not empty.

`equalsIgnoreCase` checks if two strings are equal, ignoring case.

`compareIgnoreCase` compares two strings, ignoring case.

`flip` flips the order of characters in a string.

`nullToEmpty` turns `null` to empty string, and returns non-empty strings
unchanged.

`emptyToNull` turns empty string to `null`, and returns non-empty strings
unchanged.

`repeat` concatenates a string to itself a given number of times.

`loop` allows you to loop through characters in a string starting and ending at
arbitrary indices. Out of bounds indices allow you to wrap around the string,
supporting a number of use-cases, including:

  * Rotating: `loop('lohel', -3, 2) => 'hello'`
  * Repeating, like `repeat`, but with better character-level control, e.g.:
`loop('la ', 0, 8) => 'la la la'  // no tailing space`
  * Tailing: `loop('/path/to/some/file.txt', -3) => 'txt'`
  * Reversing: `loop('top', 3, 0) => 'pot'`
