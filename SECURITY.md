# Security

dovy installs software as root, so a flaw in dovy, in a recipe or in a
release can reach many machines. Report it privately, never in a public
issue.

## Reporting

- On GitHub: the repository's **Security** tab, then **Report a
  vulnerability**.
- By email: getdovy@tuta.io.

Include what is affected (dovy's version, the recipe, or the catalog or
kernel release), how to reproduce it, and what it allows.

## What counts

- dovy accepting a catalog, release or download it should refuse:
  signature, checksum or rollback checks bypassed.
- A recipe that installs something other than what it says, or a vendor
  script that does more than the recipe declares.
- Files or folders dovy leaves writable by users other than root.
- A dovy-kernel package that differs from its build record.

Flaws in the software a recipe installs belong to its vendor; flaws in
Debian's packages, to [Debian](https://www.debian.org/security/).

## Supported

The latest dovy release, the latest catalog release and the latest
dovy-kernel release. Fixes come as new releases; a published release is
never changed.

## Response

Reports are acknowledged within a week. Once a fix is released, the
report is published as an advisory, crediting the reporter unless they
ask otherwise.
