# Security

## Report a vulnerability

Please do not open a public issue. Use "Report a vulnerability" under the
Security tab of the affected repository, or write to hello@jjsm.science.

Say what you found, how to reproduce it, and which version you used. You will
get a reply within a week. Once a fix is released you are credited in the
release notes, unless you prefer not to be.

## What counts

- A way to make `texshelf init` write outside the project folder, run code, or
  accept an archive whose checksum does not match the index.
- A template in the registry that runs commands, downloads files or reads
  data outside its folder when compiled.
- A way to change a published template version or its archive.
- A flaw in the install scripts, the website or its download counter.

## Supported versions

Only the latest release of the CLI gets fixes.

## How templates are checked

Every template version is scanned before it is published, and the result is
shown on its page at [tex.jjsm.science](https://tex.jjsm.science). The scan
reads files and compiles nothing. It catches common problems and is not a
guarantee, so read a template's build files before compiling with
`--shell-escape`.
