# Waypoint Fix

[![CI](https://github.com/Sam-DarkBall-Mods/Waypoint-Fix/actions/workflows/ci.yml/badge.svg)](https://github.com/Sam-DarkBall-Mods/Waypoint-Fix/actions/workflows/ci.yml)

Waypoint Fix repairs the landing command in the UAV Terminal. It marks the
selected waypoint as a landing waypoint, waits for the UAV to touch down, then
recreates the UAV crew and reconnects the operator.

## Requirements

- Arma 3 2.22 or newer

## Building

```bash
python3 -B -m unittest discover -s tests -p "test_*.py" -v
hemtt check
hemtt build --no-bin
```

The `DB_wpFix` patch, `DB_fnc_*` functions and `wpFix` prefix are kept for
missions that already use them.

## License

The SQF code, config and repository tools use GPL-2.0-or-later. See
[LICENSES.md](LICENSES.md).
