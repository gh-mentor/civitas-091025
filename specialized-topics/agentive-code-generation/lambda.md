Use the Agent mode to perform all steps.

## Instructions to create an app using Agentive AI (.NET C#)

1. Create a new C# file named `Program.cs` in the current directory.

2. At the top, include the necessary `using` directives for input/output and collections:
   - `System`
   - `System.Collections.Generic`

3. Define the namespace `Lambda` and place all code inside it.

4. Inside the namespace, create a static class `LambdaGen` and place the following methods inside it:
   - `SqrGen`: Returns a `Func<double, double>` that squares a double argument.
   - `CubeGen`: Returns a `Func<double, double>` that cubes a double argument.

5. In the `Main` method:
   - Declare a `List<Func<double, double>>` to store functions matching the signatures of `SqrGen` and `CubeGen`.
   - Prompt the user to enter up to 10 real numbers, stopping if the user enters -1.
   - Store the input numbers in a `List<double>`.
   - Add the `SqrGen` and `CubeGen` functions to the function list.
   - For each input number, print its value, its square, and its cube in a formatted row (e.g., `n: 2.5   Squared: 6.25    Cubed: 15.625`).

6. Create a C# project file for the program, add a '.gitignore' file to exclude unnecessary files, then build and run the program in a PowerShell terminal.
