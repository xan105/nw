NW: No window
=============

Chainload binary silently (no window) using `SysProcAttr{HideWindow: true}`

Usage
-----

`nw.exe [-config /path/to/config.json]`

If no arg provided default to `./nw.json`

config file: 
```json

{
  "bin": "/path/to/exe", //required
  "args": "",
  "cwd": "./",
  "fileCheck": [
    {"sum": "sha256", "size": 0}, //self (bin value)
    {"file": "/path/to/file", "sum": "sha256", "size": 0}
  ]
}

```

Build
-----

>= go1.12.1
Use `buildme.cmd`