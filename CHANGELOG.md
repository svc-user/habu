### 20231117

#### Windows support

Habu now works on Windows! Note that I'm not a daily Windows user myself, so I'm happy to hear about any bugs or weird behavior Windows users come across.

#### Add `stopped` modifier to chains.

Stopping a chain is useful when you are no longer interested in tracking it but you want to keep the history and stats around.
Use `modify <index> stopped <date>` to stop a chain, or `modify <index> stopped false` to make a stopped chain active.
Stopped chains are not displayed by default, and their stats only include the dates from the creation date up to the stopped date.
Also add a new `--show` parameter to choose which chains to display.

#### Minor features

- Add `habu version` command.

#### Bugfixes

- Compute stats for the entire chain in `info` command, not just the last 30 days.
- Fix args check for `habu help <command>`, it takes 1 optional arg, not 0.

### 20230810

- Initial release
