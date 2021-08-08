# Argon scanner action

Protect the first phase of your software supply chain

## Inputs

#### `argon-token`

**Required** Token provided by Argon. It is highly recommended to add it as a secret.

#### `scanners`

Multiline list of checks to run. Defaults to all.

#### `audit-only`

If true the action will never fail the workflow. defaults to false.

#### `should-notify`

If true a notification will be sent to the configured Slack/Teams channel on new findings. defaults to false.

## Example usage

```
uses: actions/argon-scanner@v1
with:
  audit-only: true
  should-notify: true
  argon-token: "${{ secrets.ARGON_TOKEN }}"
```
