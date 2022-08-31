## LetterBomb client-side-only implementation

This is the LetterBomb Wii System Menu 4.3 exploit implementation, modified
to work without a backend.

In case you're wondering, `country_regions.txt` is based on reporting data
from Homebrew Channel updates. This was implemented because we found out
that about 30% of our users are stupid and won't pick the correct system
menu version (and then complain that it doesn't work), so we use GeoIP to
guess the right default for them. Similarly, the MAC address check was
implemented because people would type in garbage for the MAC address and
then complain that it doesn't work.

This does not include the HackMii Installer bundle. Those files would go
compressed in `bundle.zip`.

NOTE: This does not work over the `file://` protocol. Please use with a
webserver. A quick one is: `python3 -m http.server`

### License

GPL-2.0
