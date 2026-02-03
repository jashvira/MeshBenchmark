# Clean Benchmark Tasks

This branch keeps the task implementations under `tasks/` using descriptive filenames.

- Root-level `N.py` files are **auto-generated shims** that import from `tasks/` for the focused set.
- All other `N.py` files are **stubs** (`skip = True`) to keep the runner's sequential indexing intact without carrying legacy task code.

The focused task list lives in `tasks/registry.json`.

To run only the focused set, pass `-t` with the indices listed in `tasks/registry.json`.
