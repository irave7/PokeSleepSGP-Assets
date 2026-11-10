# PokeSleepSGP public art data

Public names, game-internal catalog mappings and static images for PokeSleepSGP.
This repository contains no app source, observer scripts, player data, account
identifiers, captured responses, sessions, certificates or private signing keys.

The app verifies the Ed25519 signature on `manifest.json`, then verifies the
package hash and size before validating and installing the data on the device.
`public-key.json` is public verification material, not a signing secret.

The initial `2026.11.10.1` data package uses the verified game 3.9.1 catalog
already bundled in PokeSleepSGP. It contains 245 internal species entries,
119 item entries and 538 images. Internal species numbers are not National
Pokédex numbers. Unverified forms remain unbound; missing images are not guesses.

Future packages must keep verified game-internal ID mappings and attribution.
An upstream image change alone is not proof of a new game ID or form mapping.
Only static data and images are published; changing the collector or decoding
logic still requires a separately built app update.

See `NOTICE.txt` for image and data provenance. This is an independent project
and is not affiliated with Pokémon, SELECT BUTTON, or The Pokémon Company.
