### 1.8.5:

* ADDED: JourneyMap implementation; sneak r-click a sample to add as a waypoint automatically!
* FIXED: Debug message in the output with the geolosys_ores.json location

### 1.8.4b:

* FIXED: Crashes with null dimension blacklist
* FIXED: Debug print statements left in

### 1.8.4:

* ADDED: Beryl, a mineral resource for emeralds!
* ADDED: New JSON file for ore generation settings (offers more refined settings). See your /config/geolsys_ores.json for more!
* ADDED: New texture for cassiterite samples, to make them distinguishable
* ADDED: Ability for osmium to be enabled *alone*
* CHANGED: Ingot textures to new beta-style ingot texture
* CHANGED: Samples now generate based on the mineral deposit size (still respecting the max samples config)
* CHANGED: Default ore generation values (in the JSON config)
* FIXED: Prospector's pick sending its message on both sides
* FIXED: Gold and Iron not being obtainable via silk-touch
* FIXED: Duplicate smelting registration

### 1.8.3:

* ADDED: Info for Sphalerite, Osmium & Yellorium to the Field Manual
* ADDED: Automatic modularity for additional pages (this means that users can add as many entries as they'd like!)
* FIXED: Yellorium and Osmium dropping when disabled, instead of the other way around.

### 1.8.2:

* ADDED: Sphalerite; this is a resource for Zinc, and can be disabled and configured like all other orers
* ADDED: Osmium drop to Platinum, if enabled
* ADDED: Yellorium drop to Autunite, if enabled
* FIXED: Bugs with smelting.. I hope.

### 1.8.1:

* ADDED: Field Manual! Crafted with an undamaged wooden pickaxe and book


### 1.8:

* ADDED: User Entries for mineral deposits can now have a custom "sample" specified - particularly useful alongside ContentTweaker if you want to make your own sample replicas. `See config for usage` - Thanks Darkosto for the suggestion!
* ADDED: Config option to disable the cluster smelting recipes, since their recipes are registered in `postInit` (and *have* to be) so they can't be CraftTweak'd out - Thanks Darkosto for the suggestion!
* CHANGED: Internal refactors that the user should probably never have to worry about 
* CHANGED: Game no longers crash if `enableIngots` is false but you lack an ingot; it'll just log it and move on :)
* CHANGED: In-game config now notifies of restart requirement


### 1.7:

* ADDED: Prospector's Pick
* ADDED: Prospector's Pick feature config
* FIXED: Odd ore generation in the Twilight Forest dimension

**I will be in contact with the Twilight Forest devs to see if we can come up with a means of replacing the ore generation in Hollow Hills**

### 1.6:

* ADDED: Config to prevent samples from actually dropping anything
* ADDED: Config to add custom ore entries again; "samples" for these entries are the block themselves.
* ADDED: Config for samples spawning in the water
* CHANGED: New textures by Wiiv!!
* FIXED: Samples on samples not spawning samples at all
* FIXED: Snow and other things spawning on top of samples


### 1.5:

**WARNING: You should disable 'cascading chunk lag' logging in the Forge Config. More explained below**

* ADDED: ExU2 Compatibility for Cinnabar!
* REMOVED: Config for custom ores... if this is chaos, let me know, but I decided to remove it ultimately because the samples wouldn't ever be able to be dynamic like that..
* CHANGED: Mineral deposits below Y=24 now generate magma blocks instead of lava to prevent frustration and be more geologically accurate
* CHANGED: Mineral deposits of lesser minerals (cassiterite, malachite & hematite) generate in smaller clusters by default (delete config entries to reset them!)
* CHANGED: Mineral deposits now generate... differently. Still in the same chunk and the same formation, but at . It's bound to cause "cascading chunk lag", but I've tested this extensively and it **does not progress for long** before stopping :)
* FIXED: Some chunks not generating mineral deposits even though there was a sample
* FIXED: Samples on samples
* CHANGED: Some new textures by Wiiv! When the rest are done, a new version will be released :D


### 1.4:

* ADDED: Config options for vanilla ores
* CHANGED: Vanilla ore rate defaults... again
* CHANGED: Diamonds are now called "Kimberlite"
* CHANGED: Diamond texture to be more Kimberlite-y
* FIXED: A few bad names in the configs... best to double check them

### 1.3:

**Warning, this is basically the 'Samples' update :P**

* ADDED: Right click interaction to samples
* FIXED: Samples not always generating
* FIXED: Samples spawning in superflat
* FIXED: Unused config option for # of veins per chunk (obviously it's ### 1. always)
* CHANGED: Samples generate in clusters of ### 1.to 4
* CHANGED: Samples behave more realistically
* CHANGED: Tweaked vanilla ore-gen values one last time. 5/7 are balanced now ;)

### 1.2:

* ADDED: Custom vanilla ore variants - these can be silk touched for the Vanilla ores. All drop values are directly referenced from their vanilla variants
* ADDED: Assorted Quartz Clusters can drop Certus Quartz, Charged Certus Quartz or Black Quartz if available.
* ADDED: Ore Samples on the surface above where that type of ore will generate. Mining within the chunk you find one will lead you to a deposit.
* ADDED: Separate user entries in the config for custom "stones" / "rocks"
* CHANGED: Mineral deposits found below Y = 24 can contain pockets of magma
* CHANGED: Rarities - a lot - only one ore type can generate per chunk
* CHANGED: Cluster Sizes - since ores are rarer, these are much larger
* CHANGED: Stone variants have their own separate chances to spawn, preventing them taking an OreGen oppportunity
* CHANGED: Minor refactors to be more similar to vanilla
* FIXED: Config GUI not prompting user to restart their game
* FIXED: Various smelting recipe issues
* FIXED: Rocks replacing more valuable minerals

### 1.1-alpha:

* ADDED: User configurable plutons entries (ideal for mods that I didn't include)
* CHANGED: Vanilla ore gen weights. Most things are more rare, except the stone variants; those are more common
* CHANGED: Default ore gen options. Materials with 2 variants are half as rare now.

### 1.0-alpha:

* Initial Release
