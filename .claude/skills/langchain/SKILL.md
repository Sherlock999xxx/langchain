```markdown
# langchain Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and conventions used in the `langchain` TypeScript codebase. You'll learn how to structure files, write imports and exports, follow commit message conventions, and write tests in alignment with the repository's established practices.

## Coding Conventions

### File Naming
- Use **camelCase** for file names.
  - Example: `myModule.ts`, `dataProcessor.ts`

### Import Style
- Use **relative imports** for referencing other modules.
  - Example:
    ```typescript
    import { processData } from './dataProcessor';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    export function processData(input: string): string {
      // ...
    }
    ```

### Commit Messages
- Follow **conventional commit** format.
- Use the `chore` prefix for routine tasks.
  - Example:
    ```
    chore: update dependencies to latest versions
    ```

## Workflows

### Code Contribution
**Trigger:** When adding new features or making changes  
**Command:** `/contribute`

1. Create a new branch for your changes.
2. Implement your changes following the coding conventions.
3. Write or update tests in files matching `*.test.*`.
4. Commit your changes using the conventional commit format (e.g., `chore: ...`).
5. Push your branch and open a pull request.

### Testing
**Trigger:** Before submitting or merging code  
**Command:** `/test`

1. Identify or create test files using the `*.test.*` pattern.
2. Run the test suite using the project's test runner (framework unknown; check project scripts).
3. Ensure all tests pass before merging.

## Testing Patterns

- Test files follow the `*.test.*` naming convention.
  - Example: `dataProcessor.test.ts`
- The testing framework is not specified; check project scripts or documentation for details.
- Place tests alongside or near the files they test.

## Commands
| Command      | Purpose                                 |
|--------------|-----------------------------------------|
| /contribute  | Start the code contribution workflow    |
| /test        | Run the test suite                     |
```