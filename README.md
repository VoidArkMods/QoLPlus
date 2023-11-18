# QoLPlus
ARK: Survival Ascended mod. Adds quality of life changes.

QoL+ is a fork and migration of Structures Plus (S+) by orionsun. All credits to him and everybody who helped on this awesome mod!

The code of QoL+ is open source. You are encouraged to experiment with it.
[QoL+ on CurseForge](https://www.curseforge.com/ark-survival-ascended/mods/qol)

## Disclaimer
Some assets have been pre-migrated up to a point where the whole content compiles properly, but have not been properly tested. Anything that is not referenced in `PrimalGameData_QoLPlus` or `ModDataAsset_QoLPlus` still need some more work to be considered production-ready, but they can be played around if wanted.

## Ini settings

Every QoL+ settings must appear under the tag `[QoLPlus]` in the GameUserSettings.ini configuration file (under `\ShooterGame\Saved\Config` for clients, under `\ShooterGame\Saved\Config\WindowsServer` on servers running on Windows)

If you were using `S+` in Ark: Survival Evolved: the name of the settings did not change, only the header must be changed from `[StructuresPlus]` to `[QoLPlus]`.

| Name  | Default value | Description |
| ------------- | ------------- | ------------- |
| PullResourceAdditions  |  | Allows you to add any resource to the pull resource list. It is a comma separated list of nearly the entire spawn code (everything between the ' ) |
| RemoveFloorRequirementFromStructurePlacement | False | Will allow structures that normally require placement on a floor to be placed on the ground (ie smithy, forge, etc) |
| DisableResourcePulling | False | Disable resource pulling from inventories |
| ResourcePullRangeInFoundations | 25 | Sets the distance crafting stations can pull from (max 100) |
| ResourceTransferCooldown | 1.0 | The delay between all resource transfers like pulling (min: 0.1) |
| PullResourceRemovals |  | Allows you to remove items from the default resource pull list. It is a comma separated list of everything between the ' of the spawn code for that item |
| PullResourceAdditions |  | Allows you to add any resource to the pull resource list. It is a comma separated list of nearly the entire spawn code (everything between the ' ) |
| AdvTransferItemBlacklist |  | Allows you to prevent certain items from being transferred via the Omni-Tool & other similar transfers. It is a comma separated list of everything between the ' of the spawn code for that item |
| PullingIgnoresPinCodes | False | Allows resources transfers in/out of locked structures that have pin codes |
| QoLPlusEngramWhitelist |  | This is a comma separated list of QoL+ Engrams you want to use, all others will be hidden |
| EnableExtendedDeathCache | False | Replaces the default death bag with one that can support more than 600 slots (may interfere with death helper mods) |
| RaidTimerLimitMultiplier | 1.0 | Multiplier for the time limit of defeating raid bosses (ie value of 2 will allow 30 minutes to kill the Broodmother instead of 15 minutes) |
| OmniToolBlacklist |  | This is a comma separated list of modes you wish to hide from the user: BasicTransfer,AdvancedTransfer,InventoryAssistant |
| MultiToolBlacklist |  | This is a comma separated list of modes you wish to hide from the user: Structure,Dino,Remote,Repair |
| SmallStorageSlotCount | 30 | Amount of slots in the Small Storage |
| LargeStorageSlotCount | 90 | Amount of slots in the Large Storage |
| MetalStorageSlotCount | 100 | Amount of slots in the Metal Storage |
| PropagatorSlotCount | 100 | Amount of slots in the Propagator |
| PropagatorMatingSpeedMultiplier | 1.0 | Similar to the vanilla mating speed multiplier, higher numbers mean less time mating |
| PropagatorMatingIntervalMultiplier | 1.0 | Similar to the vanilla mating interval multiplier, smaller numbers means less time between mating |
| PropagatorFuelClass |  | Use to override the fuel used, eg PropagatorFuelClass=/Game/PrimalEarth/CoreBlueprints/Resources/PrimalItemResource_Wood.PrimalItemResource_Wood |
| PropagatorFuelInterval | 86400 | The time in seconds that a single piece of fuel will last 86400 seconds = 24 hours |
| PropagatorModCostItemClass |  | Overrides the item used by modifications, eg PropagatorModCostItemClass=/Game/PrimalEarth/CoreBlueprints/Resources/PrimalItemResource_Wood.PrimalItemResource_Wood |
| PropagatorModCostMutate | 1 | Cost per mutation pulse applied (-1 will cause it to be free) |
| PropagatorDisableDinoMods | False | Prevents using any of the dino modifications (mutate, gender change, allow breeding) |
| MutatorBuffMaxStackCount | 2 | How many stacks the Mutator buff is capped at.(max: 100) |
| PropagatorDinoBlacklist |  | Comma separated list of dino classes, eg PropagatorDinoBlacklist=Rex_Character_BP_C |
| PropagatorRespectMutationLimit | False | Will prevent mutations if over the vanilla cap of 20 |
| EnableUpdateDurability | False | Will stop the Vivarium, Propagator & Tek fridge from preventing durability lose for items inside... This allows Soul Traps to update mating timers & other things but will cause Cryo Pods to lose charge... ONLY ENABLE IF USING DINO STORAGE (Which is not available in ASA yet :D) |
| PropagatorDisableEggDrop | False | Stops the Propagator from dropping eggs |
| TribePropagatorLimit | 0 | Tribe Limit of Propagator |
| NannySlotCount | 100 | Amount of slots in the Nanny |
| NannyRangeInFoundations | 10 | The range of the Nanny's feeding and imprinting bonus.(max: 50) |
| NannyMaxImprint | 100 | The highest the Nanny will imprint a dino. (max: 100) |
| DisableNannyImprinting | False | Stops the Nanny from boosting imprinting |
| NannyIntervalInSeconds | 35 | Time between the Nanny's feeding & imprinting |
| NannyFeedingStartThreshold | 20 | The percentage of food value below which the Nanny will start feeding (accepts values between 1 & 100) |
| DisableHitchingPostMatingBonus | False | Disables the hitching post mating bonus |
| HitchingPostRange | 4 | Range, in foundations, that dinos can be leashed to a hitching post (max: 100) |
| HitchingPostDinoLimit | 0 | Max number of dinos that can be hitching to a hitching post |
| HitchingPostTribeLimit | 0 | Tribe Limit of Hitching Post |
| MutatorBuffMaxStackCount | 2 | How many stacks the Mutator buff is capped at (max: 100) |
| TransmutatorSlotCount | 100 | Amount of slots in the Mutator |
| MutatorPulseCost | 10 | How many element each pulse of the Mutator will cost, accepts a single value for all or a comma separated list of all the modes (ie =2,2,2,7,1,9) (max: 1000) |
| MutatorPulseCooldowns | 300 | How long the mutator is unable to be used for after a pulse, accepts a single value for all or a comma separated list of all the modes (ie =300,60,60,5,300,30) |
| MaxMutatorRangeInFoundations | 50 | Maximum range that mutators can be set to ingame (min: 5, max: 50) |
| MutatorModeBlacklist |  | Allows you to disable any mode of the mutator: Mutation,SwapGender,AssignGender,AllowBreeding,Imprint,FreezeGrowth,BoostGrowth |
| MutatorAllowBreedingNeutered | False | Allow breeding of neutered/spayed creatures in the mutator |
| MutatorDinoBlacklist |  | Stops all mutator pulses from affecting dinos on this list. Accepts a comma separated list of dino names that can either be exact classes or partial classes |
| GardenerSlotCount | 300 | Amount of slots in the Gardener |
| GardenerRangeInFoundations | 25 | Collection and distribution range of the Gardener, in foundations (max: 100) |
| FarmerSlotCount | 300 | Amount of slots in the Farmer |
| FarmerRangeInFoundations | 25 | Collection range of the Gardener, in foundations (max: 100) |
| AllowTekItemBlueprintCreation | False | Allows the Blueprint Maker to turn tek items into blueprints |
| AllowMakingWeaponsAndArmorBPs | False | Allows the Blueprint Maker to create blueprints from armor & weapons |
| BeeHiveSlotCount | 24 | Amount of slots in the Domesticated Bee Hive |
| BeeHiveWateringRangeInFoundations | 30 | How far away from the hive the bees will deliver water (max: 100) |
| BeeHiveHoneyIntervalInSeconds | 180 | Time between honey generation in the bee hive. 180 seconds = 3 minutes |
| AmmoBoxSlotCount | 300 | Amount of slots in the Ammo Box |
| DisableMultiToolDinoKillMode | False | Disables the Kill sub-mode of the Multi-Tool from functioning (will still be visible but unable to be used) |
| DisableMultiToolDinoChibiMode | False | Disables the Chibify sub-mode of the Multi-Tool from functioning (will still be visible but unable to be used) |
| AllowMultiToolNeuterAll | False | Allows the Neuter sub-mode of the Multi-Tool to neuter dinos that normally can't be neutered |
