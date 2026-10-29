# PodBridge Privacy Policy

Effective date: September 9, 2026

PodBridge does not require an account, contain advertising, or sell personal
information. The app may send a small number of pseudonymous product-usage events
to measure transfer reliability and improve the app. These events do not
contain names, account identifiers, filenames, paths, music metadata, audio,
or iPod identifiers.

## Data stored on the device

PodBridge accesses only the source and destination folders that the user
selects through Apple's document picker. Music files, their metadata, iPod
library databases, device-profile choices, iPod signature identifiers,
backups, and diagnostic logs are processed locally on the user's devices.
PodBridge does not upload audio files, iPod databases, signature identifiers,
diagnostic logs, or file paths.

Local PodBridge data can be removed by deleting the app. Backups written to an
iPod remain on that iPod until the user removes them.

## Anonymous product analytics

When an analytics-enabled version of PodBridge is installed, the app sends
pseudonymous events such as app launch, source
scan completion, transfer start, transfer success, and broad transfer failure
category. A randomly generated installation identifier keeps events from the
same installation together for aggregate funnels and retention. It is not an
Apple device identifier and is not linked to an account or used for tracking
across apps or websites. The events are used only for product analytics and
reliability improvements. The analytics provider is PostHog, and the app uses
its US endpoint with server-side GeoIP enrichment disabled.

## Optional self-hosted ALACarte connection

This section applies only to the separately built `PodBridgeALACarte` target.
The standard `PodBridge` target contains no ALACarte client. When the user
chooses the self-hosted library feature, PodBridgeALACarte connects only to the
server address entered by that user. The server address and username are stored
in the app's local preferences. The password is used to sign in and is not
saved; the resulting session token is stored in the iPhone Keychain.

The user's own server receives the network address of the iPhone and requests
for the selected library items. Compatible audio and playlist files are copied
to temporary app storage, written to the selected iPod, and then deleted from
temporary storage. PodBridge does not send the server address, credentials,
library data, or audio files to the project author or to a PodBridge-operated
service.

## Online artwork search

Online artwork search is optional and runs only after the user requests it.
PodBridge sends the relevant artist, album, or track name to the public
MusicBrainz API and downloads matching artwork through the Cover Art Archive.
These requests may expose the search terms, IP address, and PodBridge version
to those services. Their handling of requests is governed by their own
policies and terms.

- [MusicBrainz](https://musicbrainz.org/)
- [Cover Art Archive](https://coverartarchive.org/)
- [MetaBrainz privacy policy](https://metabrainz.org/privacy)

## Diagnostics

Diagnostic logs remain on the device unless the user explicitly exports and
shares them. The report does not include audio contents, cover-image bytes,
absolute source paths, or the iPod signature identifier.

## Contact

Questions and privacy requests can be submitted through the
[PodBridge issue tracker](https://github.com/dbalantaev/PodBridge-Store/issues).
