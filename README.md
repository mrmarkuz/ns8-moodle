# ns8-moodle

Moodle is a web learning platform

## Install

Install via Software center:

  - Add a Software repository pointing to `https://repo.mrmarkuz.com/ns8/updates/`, check out the [repo webpage](https://repo.mrmarkuz.com) how to do it.

The first startup takes about 4 minutes as Moodle gets freshly installed by an install script. You can follow the process on the logs page.

## Configuration

Set the FQDN and the admin name and password in the app settings.
Browse to the set FQDN.

## Uninstall

To uninstall the instance:

    remove-module --no-preserve moodle1

## UI translation

Translated with [Weblate](https://hosted.weblate.org/projects/ns8/).

To setup the translation process:

- add [GitHub Weblate app](https://docs.weblate.org/en/latest/admin/continuous.html#github-setup) to your repository
- add your repository to [hosted.weblate.org]((https://hosted.weblate.org) or ask a NethServer developer to add it to ns8 Weblate project
