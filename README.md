# Kotlin removeIf() function unexpected behavior on different collections

This repository demonstrates an unexpected behavior of the `removeIf()` function in Kotlin when used with different collection types (Lists, Sets, and Maps).

## Description

The `removeIf()` function is designed to remove elements from a collection that satisfy a given predicate. While it works consistently with Lists and Sets, it might show unexpected behavior with Maps.

## Bug

The main issue is that with the `removeIf()` function on Maps, it operates on the `key`, not the `value` in the entry.

## Solution

The bug is addressed by providing separate solutions for Maps using `filter` and creating a new map for clarity and predictable behavior.