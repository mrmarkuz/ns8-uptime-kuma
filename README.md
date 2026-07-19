# ns8-uptime-kuma

Uptime Kuma – A Fancy Self-Hosted Monitoring Tool

## Install

Install via Software Center by adding my [repository](https://repo.mrmarkuz.com)

Or on CLI:

    add-module ghcr.io/nethserver/uptime-kuma:latest 1

## Configure

In the app settings at least the FQDN needs to be set.
Browse to the FQDN, choose "Embedded MariaDB" for production or "SQLite" for small environments and create a user at the next step.

## Uninstall

The app can be uninstalled by using the Software Center or the CLI:

    remove-module --no-preserve uptime-kuma1

## Testing

Test the module using the `test-module.sh` script:


    ./test-module.sh <NODE_ADDR> ghcr.io/nethserver/uptime-kuma:latest

The tests are made using [Robot Framework](https://robotframework.org/)

## UI translation

Translated with [Weblate](https://hosted.weblate.org/projects/ns8/).

To setup the translation process:

- add [GitHub Weblate app](https://docs.weblate.org/en/latest/admin/continuous.html#github-setup) to your repository
- add your repository to [hosted.weblate.org]((https://hosted.weblate.org) or ask a NethServer developer to add it to ns8 Weblate project
