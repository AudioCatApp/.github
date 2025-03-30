# :sparkles: Code and Comments Style Guideline :sparkles:

We strive for code readability and scalability!  


## Content
- [Naming](#naming)
- [Code Formatting](#code-formatting)
- [Directives](#directives)
- [Comments](#comments)

## Naming
- Use `PascalCase` for class names, `camelCase` for variables and method, and `SCREAMING_SNAKE_CASE` for constants.
- Long, but self-explanatory name is better than short, but unclear one. Avoid abbreviations unless they're widely understood (`mainSoundManager`, not `msm`).

## Code Formatting
- Use `{ braces }` even for single-line statements, leaving room for future additions.  
Example:
```csharp
if (myFlag == true)
{
    return myFlag;
}
```
<!-- TODO: Describe attribute alignment. -->

## Directives
<!-- TODO: Add #region and #if directives. -->
- Use `#region` and `#if` directives. When? I'll fill it out later.

## Comments
- Always begin any comment text with an uppercase letter and end it with a period. Place comments on a separate line, not at the end of a line of code. Insert one space between the comment `// delimiter` and its text. Avoid using `/* multiline */` comments.  
Example:
```csharp
// This is a good comment.
var myVariable = 5;
```

- Use `<summary>` tag for function and class comments describing details above it. Omit `<param>` and `<returns>` if the description is redundant (e.g. `<returns>` can be omited for Coroutines).  
Example:
```csharp
/// <summary>
/// Do something with a variable (as a number).
/// </summary>
/// <param name="myVariable">My number.</param>
/// <returns>Another number.</returns>
private int MyFunction(int myVariable)
{
    ...
}
```