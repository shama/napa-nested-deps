# nested dependency example with napa

This shows how one would use napa with nested dependencies:

1. Clone this repo: `git clone git://github.com/shama/napa-nested-deps`
2. Go into Project B: `cd napa-nested-deps/projectB`
3. Install: `npm install`
4. Run: `npm start`

`projectB` installs `projectA`. `projectA` installs `napa` and uses it to
install `qunit` (or any repo without a `package.json`).

`projectB` never needs to know about `qunit` or `projectA`'s dependencies.
