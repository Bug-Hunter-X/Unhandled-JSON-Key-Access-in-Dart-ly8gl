# Unhandled JSON Key Access in Dart

This repository demonstrates a common error in Dart when handling JSON responses: accessing a key that may not exist in the JSON data.  The `bug.dart` file shows the problematic code, while `bugSolution.dart` provides a solution.

## Problem

The `fetchData` function in `bug.dart` makes an HTTP request and attempts to access the `'key'` from the JSON response. If the JSON response does not contain the `'key'`, the code throws an exception.

## Solution

The `bugSolution.dart` file addresses the issue by checking for the existence of the `'key'` before accessing it.  This prevents the runtime exception and handles the case where the key is missing gracefully.