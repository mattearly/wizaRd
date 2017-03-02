Readme
================

wizaRd
======

Spell data taken from <https://github.com/thebombzen/grimoire>, originally <https://github.com/ephe/grimoire/>.

Installation
------------

    devtools::install_github('oganm/diceSyntax')
    devtools::install_github('oganm/wizaRd')

Usage
-----

``` r
spells$Immolation
```

    ## **5th-level evocation**
    ## 
    ## **Casting Time**: 1 action
    ## 
    ## **Range**: 90 feet
    ## 
    ## **Components**: V
    ## 
    ## **Duration**: Concentration, up to 1 minute
    ## 
    ## Flames wreathe one creature you can see within range. The target must make a Dexterity saving throw. It takes 7d6 fire damage on a failed save, or half as much damage on a successful one. On a failed save, the target also burns for the spell’s duration. The burning target sheds bright light in a 30-foot radius and dim light for an additional 30 feet. At the end of each of its turns, the target repeats the saving throw. It takes 3d6 fire damage on a failed save, and the spell ends on a successful one. These magical flames can’t be extinguished through nonmagical means.
    ## 
    ## If damage from this spell reduces a target to 0 hit points, the target is turned to ash.
    ## 7d6 3d6
    ## [1] "Rolls: [ 3 5 2 6 6 3 3 ]"
    ## [1] "Rolls: [ 3 6 2 ]"
    ## 7d6 3d6 
    ##  28  11

``` r
spells %>% filterSpells(level=c(0,1),class= 'bard',sources='PHB',school='evocation')
```

    ## Cantrips
    ## ========
    ## Dancing Lights
    ## Light
    ## 
    ## Level 1
    ## =======
    ## Cure Wounds
    ## Faerie Fire
    ## Healing Word
    ## Thunderwave

``` r
makeBook(level=3)
```

    ## 
    ## Level 1
    ## =======
    ## Alarm
    ## Ray of Sickness
    ## Detect Magic
    ## Feather Fall
    ## Longstrider
    ## Sleep
    ## Mage Armor
    ## False Life
    ## 
    ## Level 2
    ## =======
    ## Detect Thoughts
    ## Hold Person
