# mbtoolz

**Author:** Joseph Irwin

Some tools for using the MusicBrainz web API for archiving CDs. (Article on
archiving music CDs forthcoming.)

`mb-search`: Python script for searching using the MusicBrainz API

`mb-get-release-xml`: Bash script for retrieving XML metadata for a release from MusicBrainz

`encode-tracks`: Python script for turning the MusicBrainz XML metadata into commands for
encoding tracks from a FLAC image into Ogg files tagged with MusicBrainz recording ids


## Examples

### search for MusicBrainz releases by title

    mb-search -r '<title>'

This will show you a crappy ASCII table with release artist, title, id, and a ready-made folder name quoted for you.

### get metadata XML

    mb-get-release-xml <release-id> >metadata.xml

### encode tracks from a FLAC file (named 'disc1.flac')

    mkdir tracks
    encode-tracks <metadata.xml | parallel


## Permissions

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the author(s) have dedicated all copyright
and related and neighboring rights to this software to the public domain
worldwide. This software is distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with
this software. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
