# domainprofiles

Profiles of the security support and user account systems of various sites.

[![Test Status](https://img.shields.io/circleci/project/opws/domainprofiles/master.svg?style=flat&label=tests)][tests]
[![Gitter Chat](https://img.shields.io/badge/gitter-discuss_%E2%86%92-1dce73.svg?style=flat)][gitter]

[tests]: https://circleci.com/gh/opws/domainprofiles/tree/master
[gitter]: https://gitter.im/opws

## Where you would use this

On sites, or in browser extensions, that deal with user accounts across sites.
For instance, this was originally curated as a component of blot.pw (now
[Blotpass](https://www.blotpass.com/)).

## Further info

Information on the subject of deleting accounts on sites can be found at
accountkiller.com and justdelete.me (and the
[sites.json](https://github.com/rmlewisuk/justdelete.me/blob/master/sites.json)
it uses).

## Layout

Entries for domains are in [YAML](http://yaml.org/) files in the "profiles"
directory. The filename of each file, minus the .yaml extension, is the
significant domain name components of the site being profiled.

Domains are listed by the least-specific component of the domain necessary to
distinguish it from others: therefore, most sites are listed simply by the
second-level domain (regardless of whether or not they use a further domain
like www).

When lower-level domains have their own profiles (such as Arch Linux's AUR and
BBS), their filenames include the lower domain components, like
aur.archlinux.org.yaml and bbs.archlinux.org.yaml.

## Notes on URLs

Where fields include a link, if the site supports HTTPS optionally, the link
provided will be HTTPS.

For pages that contain several sections, only one of which is pertinent to the
link, the link will include an anchor / fragment for the relevant section
(where possible).

When URLs include a variable (such as a username), the URL will be separated by
spaces and plusses (for concatenation).

## Fields

See [docs/fields.md](docs/fields.md) for documentation on the format used to
describe the profiles for each domain.

## License

This database is licensed under the
[Open Database License (ODbL) version 1.0][odbl]. See [LICENSE.md](LICENSE.md)
for more information.

[odbl]: http://opendatacommons.org/licenses/odbl/1.0/
