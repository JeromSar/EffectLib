# CHANGELOG

## 3.6
 
 - Fix LineEffect, broken in 3.5
 - Add "duration" parameter, a value in ms that can convert to period/iterations for you.

## 3.5

 - Add KCauldron support (Thank you, tpnils1!)
 - Add setParticleRange method to set default particle visibility range
 - Particles now use the "long range" flag when range is greater that 16 blocks
   - The old range of 256 seemed way too high, particles appear to vanish after 16 blocks if not long-range
 - Add generalized parameter support for Configuration-driven effects
   You can put variable names that start with "$" in the configuration, e.g. "$radius"
   Then when starting an effect, you can set $radius to a value in the parameterMap
   to automatically replace the variables in the config.
 - Add a DynamicLocation class to encapsulate an Entity or Location.
   This can be used to create a virtual entity, by controlling the location while the effect is runnning.

## 3.4

 - Effects now track an Entity relative to the given starting Location
 - Added some simpler versions of EffectManager.start()
 - Removed references to Apache Commons classes

## 3.0

 - Update particle names to match current ParticleEffect lib- please check code and configs!
 - Added colorizeable spell_mob, spell_mob_ambient and redstone particles
 - Full 1.8 support
 - Better error handling, config options for turning on/off log messages

## 2.1

 - Add MC 1.8 particle FX (will work even on Spigot protocol hack- avoid on Craftbukkit 1.7!)
 - Add displayTo methods for showing a particle to only one player.

## 2.0

 - Refactored Effect system. Most Effect class names have changed!
 - Combined Entity and Location Effects.

## 1.8

 - Last backward-compatible version of EffectLib.
 