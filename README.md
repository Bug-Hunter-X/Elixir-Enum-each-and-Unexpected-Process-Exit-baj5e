# Elixir Enum.each and Unexpected Process Exit

This repository demonstrates a subtle bug that can arise when using `Enum.each` in Elixir.  The provided code snippet shows how an exception within the anonymous function passed to `Enum.each` will lead to unexpected process termination without proper handling.

The `bug.ex` file contains the buggy code. The `bugSolution.ex` file provides a solution using `Enum.try_each` to handle potential exceptions more gracefully.

This example highlights the importance of considering exception handling when working with Elixir's enumeration functions.

## Solution

The solution involves using `Enum.try_each`, which allows you to handle potential errors within the enumeration process.