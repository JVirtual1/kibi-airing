# Kibi airing schedule (`kibi-airing` v1)

`airing.json` is a small weekly file with the broadcast slot, last aired and next scheduled episodes of currently running anime. `airing.manifest.json` describes it (size, sha256, validity). The app downloads both, checks the sha256 and uses the file only until `valid_until`.

## Source, licence and attribution
This data is **adapted from TVmaze** (https://www.tvmaze.com/), which is licensed under **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**, https://creativecommons.org/licenses/by-sa/4.0/.

What was changed (adaptation): the TVmaze shows and seasons were matched to Kibi catalog ids (`uid`), and the weekly slot (ISO weekday 1-7 = Monday-Sunday, Japan time), the episode numbers (TVmaze number minus a per-season offset), the episode total and the state (`airing`, `upcoming`, `hiatus`, `finished`) were computed. Air times are UTC instants.

This file (`airing.json`) is shared under the same licence, **CC BY-SA 4.0**, as required by the share-alike term. Please keep this note, the attribution and the link to the licence when you reuse or redistribute it. The Kibi application shows the attribution "Data adapted from TVmaze (CC BY-SA 4.0)" with a link to https://www.tvmaze.com/.

The file contains no personal data and no data from other sources: the public (open) policy `P-airing-open` is built from TVmaze only.

## Files
| File | Purpose |
|---|---|
| `airing.json` | the schedule (policy `P-airing-open`; entries keyed by catalog `uid`) |
| `airing.manifest.json` | format, size, sha256, `generated_at`, `valid_until`, attribution, licence |
| `README.md` | this note |

The file is refreshed weekly and is valid for 14 days.
