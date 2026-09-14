# polin-plugins

Oh My Pi marketplace. Lists independently installable plugins.

## Install

```
/marketplace add polin-x/omp-plugins
/marketplace install bilingual@polin-plugins
```

CLI:

```bash
omp plugin marketplace add polin-x/omp-plugins
omp plugin install bilingual@polin-plugins
```

Then restart the omp session. Extension modules are not hot-reloaded by `/reload-plugins`.

## Plugins

| ID | Repo |
|---|---|
| `bilingual@polin-plugins` | [polin-x/omp-bilingual](https://github.com/polin-x/omp-bilingual) |
| `omp-quick-commit@polin-plugins` | [3xian/omp-quick-commit](https://github.com/3xian/omp-quick-commit) |

### omp-quick-commit

One-key Git commit and push by [3xian](https://github.com/3xian). `/commit` or `Alt+C` runs the official `omp commit --push` pipeline; `/quick-commit` or `Alt+Q` generates a conventional commit message from recent agent session context using the configured commit model role, then commits and pushes.

```bash
omp plugin install omp-quick-commit@polin-plugins
```

Restart OMP after installation. Requires `git` and `omp` on `PATH`.
