# git-clean-old-busted

This utility will remove branches which exist locally but do not exist on the remote, e.g. branches which have been deleted on GitHub but still exist on your local machine.

To prevent losing local work which has not yet been pushed to a remote, branches will not be deleted if their latest commit is less than 30 days old.

## Usage

```bash
# through a direct script call
$ ./git-clean-old-busted

# or, through a git alias
$ git config --global alias.clean-old-busted '!/path/to/git-clean-old-busted'
$ git clean-old-busted
```
