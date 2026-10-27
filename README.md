# Mega Man W — Nintendo Switch homebrew runtime

This repository contains the tested Switch homebrew runtime and its required support files. It does **not** include the Mega Man W game resource pack.

## Included

```text
Mega Man W.nro  Custom Godot-NX runtime
cntrl.cnf       Control configuration
opt.cnf         Game options
player.stat     Player save data required by the tested setup
timetrials.stat Time-trial data required by the tested setup
```

The NRO’s Homebrew Menu metadata is:

- Title: `Mega Man W`
- Author: `JDE and Team W`

## Required game data

You must provide your own `Mega Man W.pck` from a legitimate installation of Mega Man W. It is not included in this repository.

## SD-card layout

Copy the included files and your own PCK to this exact location:

```text
sd:/switch/Mega Man W/
├── Mega Man W.nro
├── Mega Man W.pck      # obtain separately; not distributed here
├── cntrl.cnf
├── opt.cnf
├── player.stat
└── timetrials.stat
```

The NRO and PCK names must match exactly, including spaces, so the runtime can discover the resource pack.

## Notes

- This is a homebrew runtime test and is not affiliated with Capcom or the original Mega Man W creators.
- First level loads, including retries, can take close to a minute on Switch.
- Do not hand-edit `opt.cnf`, `player.stat`, or `timetrials.stat`; they are encrypted Godot data.

