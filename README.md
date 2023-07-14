# man2pdf

## What the script does

This script does one two things:

### Create a temporary pdf file from a `man` *page*
  - If Documentation exists on [OpenBSD manpages](https://man.openbsd.org) it will convert that `html` to a temporary pdf using `pandoc`
  - Else it will create a temporary pdf file using `man -t` and then processing that output with `ps2pdf`

### Open the pdf immediately for viewing
It will open the temporary pdf in a pdf viewer. Currently it's hardcoded to open with with evince.

## How to use it

### Required Dependencies
You will need to make sure you have the following packages:
- `pandoc`
- A **LaTeX Distribution** such as  **TeX Live** or **MikTeX**.
- `mktemp`
- `ps2pdf`
- `evince`

### Usage

```bash
$ man2pdf <program-name>
```
