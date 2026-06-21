```markdown
# use-gesture Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and conventions used in the `use-gesture` repository, a TypeScript codebase built with React. You'll learn how to structure files, write imports/exports, follow commit message conventions, and understand the project's testing patterns. This guide will help you contribute code that fits seamlessly with the existing style and workflow.

## Coding Conventions

### File Naming
- Use **camelCase** for file names.
  - Example: `useDrag.ts`, `gestureHandler.ts`

### Import Style
- Use **relative imports** for internal modules.
  - Example:
    ```typescript
    import { useDrag } from './useDrag'
    ```

### Export Style
- Use **named exports**.
  - Example:
    ```typescript
    export function useGesture() { ... }
    export { useDrag }
    ```

### Commit Messages
- Follow **Conventional Commits** format.
- Use the `chore` prefix for maintenance or non-feature commits.
- Keep commit messages concise (average 74 characters).
  - Example:
    ```
    chore: update dependencies to latest versions
    ```

## Workflows

### Adding a New Feature or Hook
**Trigger:** When you want to add a new gesture or feature.
**Command:** `/add-feature`

1. Create a new file using camelCase in the appropriate directory.
2. Implement the feature using TypeScript and React patterns.
3. Use relative imports for any internal dependencies.
4. Export your feature as a named export.
5. Add or update relevant tests in a corresponding `*.test.*` file.
6. Commit your changes with a conventional commit message.

### Refactoring or Maintenance
**Trigger:** When performing code cleanup, dependency updates, or other maintenance.
**Command:** `/chore`

1. Make your changes (refactor, update, etc.).
2. Ensure all imports/exports follow the project conventions.
3. Update or add tests if necessary.
4. Commit with a `chore:` prefix and a concise description.

## Testing Patterns

- Test files follow the `*.test.*` naming pattern (e.g., `useDrag.test.ts`).
- The specific testing framework is not detected, but tests are colocated with the code.
- When adding or modifying features, always include or update corresponding tests.

  Example test file name:
  ```
  useGesture.test.ts
  ```

## Commands
| Command      | Purpose                                    |
|--------------|--------------------------------------------|
| /add-feature | Start the process for adding a new feature |
| /chore       | Use for maintenance or refactoring tasks   |
```
