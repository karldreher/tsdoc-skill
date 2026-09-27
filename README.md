# tsdoc-skill

A Claude Code plugin marketplace providing the **tsdoc** plugin: a skill that helps
Claude write and improve [TSDoc](https://tsdoc.org/) comments on TypeScript code
(classes, methods, functions, properties, and exported types/interfaces).

## Install

From a Claude Code session:

    /plugin marketplace add karldreher/tsdoc-skill
    /plugin install tsdoc@tsdoc-skill

Or locally, from a clone of this repo:

    claude plugin marketplace add .
    claude plugin install tsdoc@tsdoc-skill

## What it does

The `tsdoc` skill adds `/** ... */` doc comments with `@param`, `@returns`,
`@throws`, and other TSDoc tags to classes, functions, methods, properties, and
exported types/interfaces. Invoke it manually with `/tsdoc:tsdoc` when you want
TypeScript code documented.

See [tsdoc/SKILL.md](tsdoc/SKILL.md) for the full skill definition.

## License

MIT — see [LICENSE](LICENSE).
