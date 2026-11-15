# scoop-bucket

[![Tests](https://github.com/ItsN3rdy/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/ItsN3rdy/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/ItsN3rdy/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/ItsN3rdy/scoop-bucket/actions/workflows/excavator.yml)

Personal [Scoop](https://scoop.sh) bucket. The Excavator workflow checks each
app's GitHub releases every 4 hours and commits updated manifests.

## Apps

| App | Source |
| --- | --- |
| `switch-frame-tap` | [TomasUribe/switch-frame-tap](https://github.com/TomasUribe/switch-frame-tap) (Windows viewer) |
| `orbspoofer` | [ZavalaSebas/OrbSpoofer](https://github.com/ZavalaSebas/OrbSpoofer) |

## Use

```pwsh
scoop bucket add my https://github.com/ItsN3rdy/scoop-bucket
scoop install my/switch-frame-tap
```

## Add an app

Copy `bucket/app-name.json.template` (or an existing manifest) to
`bucket/<app-name>.json`, fill in `checkver` and `autoupdate`, then push.
