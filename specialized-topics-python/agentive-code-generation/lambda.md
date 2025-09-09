
Use the Agent mode to perform all steps.

## Instructions to create an app using Agentive AI (Python)

1. Create a new Python file named `main.py` in the current directory.

2. At the top, import the necessary modules for input/output and collections:
   - `typing` (for type hints, if desired)
   - `functools` (optional, for advanced function handling)

3. Define a class or module-level functions for lambda generation:
   - `sqr_gen`: Returns a lambda that squares a float argument.
   - `cube_gen`: Returns a lambda that cubes a float argument.

4. In the main logic:
   - Create a list to store functions matching the signatures of `sqr_gen` and `cube_gen`.
   - Prompt the user to enter up to 10 real numbers, stopping if the user enters -1.
   - Store the input numbers in a list of floats.
   - Add the `sqr_gen` and `cube_gen` functions to the function list.
   - For each input number, print its value, its square, and its cube in a formatted row (e.g., `n: 2.5   Squared: 6.25    Cubed: 15.625`).

5. Create a `.gitignore` file to exclude unnecessary files, then run the program in a terminal using `python main.py`.
