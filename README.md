# pass-helper

A helper script for working with pass in a team

This [blog post] outlines the concepts we are automating in this script.

This script will help you use [pass](https://www.passwordstore.org) to securely backup and share secrets either for yourself or within a team.

## Setup

Download this script:

```bash
git clone git@github.com:ruarfff/pass-helper.git
```

Optionally add it to your path.

__Examples:__

If you use `~/bin`

```bash
git clone git@github.com:ruarfff/pass-helper.git
cp ./pass-helper/pass-helper ~/bin/
```

Or add it to your `.bashrc` or `.zshrc`

```bash
git clone git@github.com:ruarfff/pass-helper.git && cd pass-helper && cp pass-helper.sh pass-helper
PH="$(cd "$(dirname "$1")"; pwd -P)/$(basename "$1")pass-helper" && echo "export PATH=\"${PH}:\$PATH\"" >> ~/.bashrc
```

Test it out by typing `pass-helper`. You should see the help output.

## Functionality

`add-user`

To add a user to a pass store, the user must export a public key. Anyone who can already encrypt the store can add a new user.






