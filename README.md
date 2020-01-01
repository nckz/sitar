# sitar
Sitar (simplified incremental tape archive) is designed to make it easy to
setup a cron job for incrementally backing up files via tar's tried-and-true
incremental backup capability. Sitar simplifies this process by:

* homogenizing backup file naming scheme
* providing common backup patterns into one function call
   * rolling/ring-buffer backup archives
   * rolling incremental archives (where full archives are made at intervals)
* auto-initialize on first run
* written with python3 standard library for portability

# Dependencies
* A tar program that implements the `--listed-incremental` option.
* Python 3
