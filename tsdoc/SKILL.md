---
name: tsdoc
description: Generate and improve TSDoc-style /** ... */ documentation comments on TypeScript classes, interfaces, types, functions, methods, and properties. Invoke manually with /tsdoc:tsdoc when the user asks to "add TSDoc", "document this function/class", "add doc comments", or "improve documentation" on TypeScript code.
disable-model-invocation: true
---

# tsdoc

Always use proper TSDoc on all TypeScript code elements: classes, interfaces, types, functions, methods, and properties.

## Instructions

1. Identify every class, interface, type alias, function, method, and property in the file(s) being touched.  
2. For each one, write a `/** ... */` block directly above the declaration:
   - Start with a one-sentence summary of what it does/represents.
   - Add a longer description paragraph only if the summary isn't sufficient.
   - Document each parameter with `@param name - description`.
   - Document the return value with `@returns description` (omit for `void`/constructors).
   - Document thrown errors with `@throws {ErrorType} description` when the function can throw.
   - Use `@remarks` for implementation notes, `@example` for usage examples, `@deprecated` where applicable, and `@see` to cross-reference related symbols.
   - For generics, document type parameters with `@typeParam T - description`.
3. Keep comments accurate to the actual signature and behavior — never invent parameters, return types, or behavior that isn't in the code.
4. Match the project's existing TSDoc conventions/style if a pattern is already established elsewhere in the codebase.
5. When editing an existing comment, preserve accurate content and correct only what has drifted from the current code.
6. Skip purely local, trivial variables inside function bodies — focus on classes, exported functions/types, public methods, and properties.

## Tag reference

Follow standard TSDoc tags: `@param`, `@returns`, `@throws`, `@typeParam`, `@remarks`, `@example`, `@deprecated`, `@see`, `@defaultValue`, `@readonly`.

## References

- [TSDoc Official Documentation](https://tsdoc.org/)
