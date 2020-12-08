# Git Commit Semantic
This guide can make you a better programmer.

The commit message should be structured as follow:
```
<type>(<scope>): <subject>
```
| Grammar      | Optional | Description | Possible Values |
| ----------- | ----------- | ----------- | ----------- |
| `type` | FALSE | Type of contribution or changes. | `feat`, `fix`, `refactor`, `style`, `test`, `docs`, `chore` |
| `scope` | TRUE | A scope may be provided to a commit's type, to provide additional contextual information | any |
| `subject` | FALSE | Describe your changes. | any |

## Type Possible Value Explaination
1. **fix**: a commit of the type `fix` patches a bug in your codebase (this correlates with `PATCH` in semantic versioning).
2. **feat**: a commit of the type `feat` introduce a new feature to the codebase (this correlates with `MINOR` in semantic versioning).
3. **BREAKING CHANGE**: a commit that has the text `BREAKING CHANGE:` at the optional body section introduce a breaking API change (correlating with `MAJOR` in semantic versioning). A breaking change can be part of commits of any type. e.g., a `fix`, `feat` & `chore` types whould all be valid.
4. **refactor**: a commit of the type `refactor` introduce new implementation of things.
5. **style**: a commit of the type `style` introduce changes of formatting copywriting, missing semi colons, etc.
6. **test**: a commit of the type `test` introduce unit test.
7. **docs**: a commit of the type `docs` introduce an update to the documentation (README and CHANGELOG).
8. **chore**: a commit of the type `chore` introduce an update of grunt task.

## Example
### Commit message with description and breaking change in body
```
feat: allow provided config object to extend other configs

BREAKING CHANGE: `extends` key in config file is now used for extending other config files
```

### Commit message with no body
```
docs: correct spelling of CHANGELOG
```

### Commit message with scope
```
feat(lang): added polish language
```

### Commit message for a fix using an (optional) issue number.
```
fix: minor typos in code

see the issue for details on the typos fixed

fixes issue #12
```
