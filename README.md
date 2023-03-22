# MinecraftServerSettings
Useful MC server (Spigot, Paper, Purpur) plugins and settings

## Basic Features

I want the server to feature the following:

- Vanilla-like survival
- Diamond-based economy with player chest shops
- Shops either in player's bases (preferred) or in a central market
- Residences and homes
- No /back command
- Quite a small creative flat world divided into rectangular "plots"

## Permission Hierarchy

```
Anonymous
  +-- Player
    +-- VIP
      +-- EVIP aka Extended VIP
        +-- Helper
          +-- Admin
            +-- Owner aka OP
        +-- Builder
```

### Anonymous
This role grants access to the following commands:
- /register
- /login

### Player
A role with a standard set of permissions including:
- /ignore

### VIP
TBD
- /wb

### EVIP
TBD
- /gsit *

### Helper
A whitelisted player.
The same as above plus the following:
- /tp
- /mute
- /unmute
- /tmpban
- /tmpunban

### Admin
A whitelisted player.
The same as above plus:
- /lp *
- /vanish
- /ban
- /unban
- restart server
- /we *
- /awr *
- /warp *

### Builder
A whitelisted player.
Same as EVIP plus:
- /vanish
- ability to build / destroy in protected areas
