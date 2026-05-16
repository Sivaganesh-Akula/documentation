# Commit history

command:

- `git log`

output:

- commit 2425f2700ae680e171a03315d9236114d7a3f0f9 (HEAD -> main, origin/main, origin/HEAD)
  Author: Siva Ganesh <akulasivaganesh1996@gmail.com>
  Date: Sat May 16 19:14:25 2026 +0530

      checking the passphrase delete for commit and push

- commit aea9210333d7722029d5ac31371084a98cff589d
  Author: Siva Ganesh <akulasivaganesh1996@gmail.com>
  Date: Sat May 16 16:24:54 2026 +0530

      moved the git doc files to git folder

- commit 90bdd16bc3ba689a5b36a57dbd8c552350479de3
  Author: Siva Ganesh <akulasivaganesh1996@gmail.com>
  Date: Tue Feb 10 22:02:12 2026 +0530

      updated the location

extensions:

- `-p` or `--patch` -> shows the difference (patch output)
- `-2` -> to limit the number of commits to show as patched
- `--stat` -> prints a commit entry a list of modified files
- `--shortstat` -> displayed only changes from the stat
- `--pretty=options` options - [`oneline, short, full, fuller, format`] - output in roughly the same format but with
  less or more information, respectively
- `--pretty=format:"%h - %an, %ar : %s"` -> to specify our own log output
  - `%H` Commit hash
  - `%h` Abbreviated commit hash
  - `%T` Tree hash
  - `%t` Abbreviated tree hash
  - `%P` Parent hashes
  - `%p` Abbreviated parent hashes
  - `%an` Author name
  - `%ae` Author email
  - `%ad` Author date (format respects the --date=option)
  - `%ar` Author date, relative
  - `%cn` Committer name
  - `%ce` Committer email
  - `%cd` Committer date
  - `%cr` Committer date, relative
  - `%s` Subject
- `--grapg` to show as ASCII graph based output
- `--name-only` Show the list of files modified after the commit information.
- `--name-status` Show the list of files affected with added/modified/deleted information as well.
- -`-abbrev-commit` Show only the first few characters of the SHA-1 checksum instead of all 40.
- `--relative-date` Display the date in a relative format (for example, “2 weeks ago”)
- `--since=` eg: `2.weeks` - command works with lot of formats
- `--author` -> allows you to filter specific author
- `grep` -> allows let you search keyword in the commit message
- `--all-match` -> further limits the output to match all search criteria
- `S` -> Only show commits adding or removing code matching the
  string.
- `-- path/to/file` ->
