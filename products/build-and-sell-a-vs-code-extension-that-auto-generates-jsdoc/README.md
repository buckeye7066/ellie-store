# Build and sell a VS Code extension that auto-generates JSDoc comments from TypeScript code

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/28E7sMg5E8bHdNx38rawo1w) · delivered as a Markdown file you can import or edit.

JSDoc Generator for TypeScript - delivered as a Markdown file you can import or edit.

*Product line: Write and license a small software utility*

---

## Preview

# JSDoc Generator for TypeScript

## Overview
This VS Code extension automatically generates JSDoc comments for TypeScript functions and arrow functions. Select a function or place the cursor on its line, run the **Generate JSDoc Comment** command, and a properly formatted JSDoc block will be inserted above it.

## Installation
1. Download the latest `.vsix` file from the [Releases page](https://github.com/yourname/jsdoc-generator-ts/releases) (or build it yourself with `vsce package`).
2. In VS Code, open the Extensions view (`Ctrl+Shift+X`), click the **…** menu, choose **Install from VSIX…**, and select the downloaded file.
3. Reload VS Code if prompted.

## Usage
1. Open a TypeScript (`.ts` or `.tsx`) file.
2. Either:
   - Highlight the entire function declaration, **or**
   - Place the cursor anywhere on the function line.
3. Open the Command Palette (`Ctrl+Shift+P`) and run **Generate JSDoc Comment**.
4. A JSDoc comment is inserted directly above the function.

### Example
**Before:**
```typescript
function add(a: number, b: number): number {
    return a + b;
}
```

**After running the command:**
```typescript
/**
 * add
 * @param {any} a - Description
 * @param {any} b - Description
 * @returns {number} - Description
 */
function add(a: number, b: number): number {
    return a + b;
}
```
*(The extension currently marks parameter and return types as `any`; you can edit the generated comment to refine types and descriptions.)*

## Development
### Prerequisites
- Node.js (≥18)
- VS Code (≥1.85.0)
- `vsce` (install via `npm install -g vsce`)

### Setup
```bash
git clone https://github.com/yourname/jsdoc-generator-ts.git
cd jsdoc-generator-ts
npm install
```

### Build
```bash
npm run compile   # produces ./out/extension.js
```

### Run in Extension Development Host
```bash
code --extensionDevelopmentPath=$(pwd)
```
Then test the command as described in **Usage**.

### Package
```bash
vsce package   # produces jsdoc-generator-ts.vsix
```

### Running Tests
```bash
npm test
```

## License
MIT License

Copyright (c) 2025 Your Name

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/28E7sMg5E8bHdNx38rawo1w)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
