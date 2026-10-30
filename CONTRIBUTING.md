# Persona Exporter - Contributing

## Branches
### Major branches
`develop` - dev branch which contains the latest (potentially breaking) code.

`unstable` - Focused on product testing and bug fixing.

`release-candidate` - A branch for full product testing. 
Code merged into it is considered polished and 
ready for widespread use, but still requires feedback.

`main` - Release branch. The contains a stable and polished product ready for use.
### Your branches

Create your branches using the 'purpose/functionality' format.

**Purpose levels:**
- **feature** For new features
- **bugfix** For bug fixes
- **docs** For documentation
- **refactoring** For refactoring (improving and optimizing) existing code
- **experimental** For experimental features that might not appear in future updates.

**Example:** "*feature/my-branch*", "*docs/update-system-module*"

## Commit naming
Commits should follow this naming pattern:

```<type>(<scope>): <description>```

Example: 

```refactor(net): Added batching```
### Type

Specify one of the following commit categories:
- **feat** (for *features*): New functionality
- **fix**: Bug fixes
- **docs**: Changes to documentation
- **lint** (for *formatting*): Changes to code formatting or style—essentially, any code changes that do not affect functionality
- **refactor** (for *refactoring*): Code restructuring to improve application optimization or readability

### Scope

Indicates which part of the codebase was modified *(e.g., "auth", "ui", "api", etc.)*

### Description

A brief description of the commit

## Pull Request
**Before send pull request, check your code:**

check code
```bash
cargo check
```

check formatting
```bash
cargo clippy -- -D warnings
cargo fmt --all -- --check
```

check documentation
```bash
cargo test --all
```

Now that all tests have passed successfully, you can submit 
a pull request specifically to the `develop` branch


