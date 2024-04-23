
# Commands I don't know

- `git gui` -- A gui! I don't think I need this.
- `git restore` -- Restore file contents
  - Overwrites given file in working tree with contents of source (default `HEAD`)
  - If `--staged`, instead overwrites file in staging area
- `git stage` [= git add]
  - File contents are hashed
  - File contents are stored in repository DB
  - File contents in working tree are registered to `.git/index` file
