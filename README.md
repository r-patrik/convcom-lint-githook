# **Commit Message Lint Git Hook**

This Git hook ensures that commit messages follow the Conventional Commits format and include a reference URL at the end.

## **Installation**

1. Save the script as `commit-msg` in your project's `.git/hooks` directory (or add it to the existing one if you already have one).
2. Make the script executable

```bash
chmod +x .git/hooks/commit-msg
```

## **Usage**

This hook will automatically run before each commit to validate the commit message.

### **Commit Message Format**

1. **Conventional Commits Format**:
    - The commit message must start with one of the following types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`, `revert`.
    - Optionally, a scope can be included in parentheses after the type.
    - The type and scope must be followed by a colon and a space, then a brief description.
    
    Example: `feat(parser): add ability to parse arrays`
    
2. **Reference URL**:
    - The last line of the commit message must be a reference URL starting with `Refs:` .
    
    Example: `Refs: https://example.com/issue/123`