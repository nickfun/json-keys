# json-keys

cli tool to print json keys of a json file

## Usage

1. `chmod +x json-keys`
2. `mv json-keys /usr/bin` or somewhere in your path
3. `json-keys <json-file-path>`

A fun thing is to use `fzf` to pick a key, then `jq` to print the value

```shell
jq $(json-keys data.json | fzf) data.json
```

## Requirements

* nodejs

Tested with Node v16.17.1
