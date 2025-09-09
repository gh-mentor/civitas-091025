Use Copilot Chat 'Ask', 'Edit', or 'Agent' mode for the following prompts:

1) Add a method `comb` to generate the count of combinations in a Python class.

2) Refactor the revised class to make use of memoization 

3) Add PyDoc documentation to the class and all methods.

4) Translate the class into idiomatic Python, using type hints and best practices.

```python
# This file contains a class that provides operations in the mathematical field of combinatorics.

class Combinatorics:

    @staticmethod
    def fact(n: int) -> int:

        if n <= 1:
            return 1
        return n * Combinatorics.fact(n - 1)

    @staticmethod
    def perm(n: int, r: int) -> int:

        return Combinatorics.fact(n) // Combinatorics.fact(n - r)


```




