# yarn-audit-json-issue

Showcases an issue with yarn v4 (4.0.1 through to stable, as of writing) where running `yarn npm audit --json` outputs the JSON incorrectly.

## How to reproduce

* run `yarn install` to install dependencies
* run `yarn audit:json` to output the npm audit to `test-audit.json`
* observe the incorrect JSON `test-audit.json`

This wasn't the case with yarn v3 or yarn v4.0.0

## The problem

In yarn 4.0.1 it seems a bug was introduced that causes the JSON output of `yarn npm audit --json` to be invalid.


