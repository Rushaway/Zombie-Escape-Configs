
# Zombie Escape Configs

Collection of stuff I have made and modified for ZE.

All vscripts under the `csgo` folder must be uploaded in the exact same folder structure.

The configs I make/modified are mainly for Zeddy or for my ports. I'm trying to publish everything publicly as a lot of configs are getting lost either in time or by dead/closed repositories. While I try to avoid posting configs made by other people, I may or may not accidentally push configs made by others. If you want credit, just contact me via the options below.

All entwatch configs are made to work with **DarkerZ's Entwatch-DZ Plugin**. I will not guarantee compatability with other forks of entwatch plugin.

All BossHud configs are made to work with either GFL's or AntiTeal/Strellic's plugins, although the `config` options will vary a bit.

## Contact Me

Feel free to contact me for anything via the methods below:

- [Steam](https://steamcommunity.com/id/notkoen/)
- Discord: **not koen #4977**
- QQ: **2432543644**
- Submit an **issue** in the issues tab in GitHub

## Special Shoutout

- [Memories](https://steamcommunity.com/profiles/76561197995817113) who taught me entwatch and stripper configs originally
- [RynerTheWolf](https://steamcommunity.com/id/2132423) who gave me a lot of support and motivation, as well as advice regarding maps and configs.

This repository is a culmination of their teaching and support, as well as several other people who've helped a lot. If you guys read this, thank you for all the help and support you gave me. I appreciate it.

## Config Formatting

### BossHud

```text
"math_counter"
{
    "config" // Optional
    {
        "HitMarkerOnly"             "" // Set to 1 if map has HPbar
        "BossBeatenShowTopDamage"   "" // Set to 0 to disable top boss damage stat display (Def. 1)
        "MaxBreakableHP"            "" // set max breakable HP before bossHP ignores it (Def. 900000)
        "MinBars"                   "" // Set minimum amount of HP bars before forced (Def. 6)
        "MaxBars"                   "" // Set maximum amount of HP bars before forced (Def. 16)
        "ForceBars"                 "" // Set forced amount of HP bars (Def. 12)
    }
    "0"
    {
        // math_counter
        "HP_counter"        "" // targetname of the hp math_counter
        "HPbar_counter"     "" // HP bar math_counter targetname (if applicable)
        "HPinit_counter"    "" // Init HP math_counter (if applicable)
        "HPbar_max"         "" // Max HP bar size (if applicable)
        "HPbar_min"         "" // Min HP bar size (if applicable)
        "HPbar_default"     "" // Starting value of HP bar math_counter (if applicable)
        "HPbar_mode"        "" // 1 = OnHitMin outputs; 2 = OnHitMax outputs (if applicable)
        "CustomText"        "" // Display name
    }
    "1"
    {
        // func_breakable, func_physbox or func_physbox_multiplayer
        "Type"              "breakable"
        "BreakableName"     "" // targetname of the func_breakable, func_physbox or func_physbox_multiplayer
        "CustomText"        "" // Display name
    }
}
```

```text
"math_counter"
{
    "config"
    {
        "HitMarkerOnly"             ""
        "BossBeatenShowTopDamage"   ""
        "MaxBreakableHP"            ""
        "MinBars"                   ""
        "MaxBars"                   ""
        "ForceBars"                 ""
    }
    "0"
    {
        "HP_counter"        ""
        "HPinit_counter"    ""
        "HPbar_counter"     ""
        "HPbar_max"         ""
        "HPbar_min"         ""
        "HPbar_default"     ""
        "HPbar_mode"        ""
        "CustomText"        ""
    }
    "0"
    {
        "HP_counter"        ""
        "CustomText"        ""
    }
    "1"
    {
        "Type"              "breakable"
        "BreakableName"     ""
        "CustomText"        ""
    }
}
```

### Entwatch

```text
"entities"
{
    "0"
    {
        "name"              ""      // Item Name (Chat)
        "shortname"         ""      // Item Name (Hud)
        "color"             ""      // Item Color (Read below for list of available colors)
        "buttonclass"       ""      // game_ui or func_button (Leave blank if only cosmetic item)
        "filtername"        ""      // filter_activator_name given to player on pickup (Leave blank if vscript assigns filtername OR AddContext output)
        "blockpickup"       "false" // Block weapon pickup
        "allowtransfer"     "true"  // Allow weapon to be etransfered
        "forcedrop"         "true"  // Force weapon to drop if player dies/disconnects
        "chat"              "true"  // Does item show up in the chat
        "hud"               "true"  // Does item show up in the hud
        "hammerid"          ""      // Hammer ID of the weapon_* entity
        "mode"              ""      // Item mode (Read Below)
        "maxuses"           ""      // Max uses item has (0 for infinite)
        "cooldown"          ""      // Item cooldown
        "trigger"           ""      // Hammer ID of entity that strips weapons (trigger_once, if applicable)
        "buttonid"          ""      // Hammer ID of button/game_ui to be tracked for items with multiple buttons (if applicable)
        "energyid"          ""      // Hammer ID of math_counter that handles the ammo count of items (if applicable)
        "buttonclass2"      ""      // game_ui or func_button of second button/game_ui (if applicable)
        "mode2"             ""      // Mode of button 2 (if applicable)
        "maxuses2"          ""      // Maxuses of button 2 (if applicable)
        "cooldown2"         ""      // Cooldown of button 2 (if applicable)
        "buttonid2"         ""      // Hammer ID of button 2 (if applicable)
        "energyid2"         ""      // Hammer ID of math_counter for ammo count of button 2 (if applicable)
        "pt_spawner"        ""      // point_template for spawning the item (if applicable)
    }
}
```

```text
"entities"
{
    "0"
    {
        "name"              ""
        "shortname"         ""
        "color"             ""
        "buttonclass"       ""
        "filtername"        ""
        "blockpickup"       "false"
        "allowtransfer"     "true"
        "forcedrop"         "true"
        "chat"              "true"
        "hud"               "true"
        "hammerid"          ""
        "mode"              ""
        "maxuses"           ""
        "cooldown"          ""
        "trigger"           ""
        "buttonid"          ""
        "energyid"          ""
        "buttonclass2"      ""
        "mode2"             ""
        "maxuses2"          ""
        "cooldown2"         ""
        "buttonid2"         ""
        "energyid2"         ""
        "pt_spawner"        ""
    }
    "0"
    {
        "name"              ""
        "shortname"         ""
        "color"             ""
        "buttonclass"       ""
        "filtername"        ""
        "blockpickup"       "false"
        "allowtransfer"     "true"
        "forcedrop"         "true"
        "chat"              "true"
        "hud"               "true"
        "hammerid"          ""
        "mode"              ""
        "maxuses"           ""
        "cooldown"          ""
        "trigger"           ""
        "buttonid"          ""
        "energyid"          ""
        "pt_spawner"        ""
    }
}
```

#### Entwatch Modes

Mode | Description
--- | ---
0 | No Button
1 | Spammable items with little to no CD
2 | Items with unlimited uses and normal CD
3 | Items with limited uses and no CD
4 | Items with limited uses and normal CD
5 | Items with several uses before CD (lightning on cosmo)
6 | Items with limited ammo (OnHitMin outputs)
7 | Items with limited ammo (OnHitMax outputs)

#### Entwatch Colors

- {red}
- {darkred}
- {lightblue}
- {blue}
- {yellow}
- {olive}
- {green}
- {lightgreen}
- {lime}
- {orange}
- {darkorange}
- {default}
- {purple}
- {pink}

### Entwatch stripper commands

- `sm_setcooldown [hammerid] [cooldown]`
- `sm_setmaxuses [hammerid] [uses]`
- `sm_addmaxuses [hammerid] [uses]`
- `sm_ewsetmode [hammerid] [mode] [cooldown] [maxuses] [used?]`
- `sm_ewsetname [hammerid] [name]`
- `sm_ewsetshortname [hammerid] [shortname]`
- `entwatch_blockepick [0/1]`
- `sm_setcooldown2 [hammerid] [cooldown2]`
- `sm_setmaxuses2 [hammerid] [uses2]`
- `sm_addmaxuses2 [hammerid] [uses2]`
- `sm_ewsetmode2 [hammerid] [mode2] [cooldown2] [maxuses2] [used?]`
- `sm_ewblock [0/1]`
- `sm_ewlockbutton [hammerid] [0/1]`
- `sm_ewlockbutton2 [hammerid] [0/1]`

### Save Level Config

```text
"levels"
{
    "0" //Number of the level, starting at 0 and increasing by 1 per level. In general level 0 should be set to as if it were a newly joined player with no levels.
    {
        "name" ""     //The name of the level to be used with the sm_level command. Typically Level 0, Level 1, Level 2, etc.
        "match"       //Block used to detect which level a player is. If this is the default/unset level, this block is unneeded.
        {
            //Use only 1 of outputs, math, or props in a match block. The set one determines which method is used to check entities for the level.
            "math"       //Matches an output's number parameter on an add or subtract input.
            {
                "" ""    //Datamap to check. Typically used with m_OnUser# (ie. "m_OnUser1" "leveling_counter,Add,1" would check against a 1 there).
            }
            "props"      //Matches a networked property of an entity.
            {
                "" ""    //Datamap to check. Typically used with m_iName. (ie. "m_iName" "1" checks for a targetname of 1)
            }
            "outputs"    //Matches an output. Typically use math or props instead of outputs if possible.
            {
                "" ""    //Datamap to check. May use any output datamap.
            }
        }
    "0"
    {
        "name"                  ""
        "match"
        {
            "math"
            {
                ""              ""
            }
            "props"
            {
                ""              ""
            }
            "outputs"
            {
                ""              ""
            }
        }
        "restore"
        {
            "AddOutput"         ""
            "DeleteOutput"      ""
            ""                  ""
        }
    }
}
```
