# Modifying List During Enum.each Iteration in Elixir

This repository demonstrates a common mistake in Elixir when attempting to modify a list while iterating over it using `Enum.each`.  The code attempts to remove the element `3` from the list, but due to Elixir's immutable nature, this doesn't work as expected.  The `Enum.each` function iterates over a copy of the list, and the modification is not reflected in the original list.

The `bug.exs` file contains the erroneous code, while `bugSolution.exs` provides a correct approach using `Enum.filter` or `List.delete`. 