# :sparkles: Code and Comments Style Guideline :sparkles:

## Content
- [Naming](#naming)
- [Code Formatting](#code-formatting)
- [Directives](#directives)
- [Comments](#comments)

## Naming
- Use `PascalCase` for class names, `camelCase` for variables and method, and `SCREAMING_SNAKE_CASE` for constants.
- Long, but self-explanatory name is better than short, but unclear one. Avoid abbreviations unless they're widely understood (`mainSoundManager`, not `msm`).

## Code Formatting
We strive for code readability and scalability!  

- Use `{ braces }` even for single-line statements, leaving room for future additions. Example:
```csharp
if (myFlag == true)
{
    return myFlag;
}
```

## Directives
<!-- TODO: Add #region and #if directives -->

## Comments
- Use `<summary>` tag for function comments describing details above it.