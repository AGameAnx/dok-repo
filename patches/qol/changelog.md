# About

QoL patch is focused on improving base gameplay flow and bug fixes, without directly changing vanilla gameplay balance.

# Applying the patch

Requires [more-maps 1.1t](https://github.com/AGameAnx/dok-repo/releases/tag/maps-v1.1)

Type `/p qol` in a multiplayer lobby to apply the patch!

# Table of contents

- [About](#about)
- [Applying the patch](#applying-the-patch)
- [Table of contents](#table-of-contents)
- [General changes](#general-changes)
	- [Target prioritization](#target-prioritization)
	- [Carrier weapons](#carrier-weapons)
	- [Nuke-class weapons](#nuke-class-weapons)
	- [Carrier point defense weapon tracer graphics](#carrier-point-defense-weapon-tracer-graphics)
	- [Unit reveal time](#unit-reveal-time)
	- [Air sortie duration](#air-sortie-duration)
	- [Aircraft hangar size](#aircraft-hangar-size)
	- [Nuke costing popcap while active/in flight](#nuke-costing-popcap-while-activein-flight)
- [Coalition/Soban](#coalitionsoban)
	- [Carrier handling](#carrier-handling)
	- [Support cruiser handling](#support-cruiser-handling)
	- [Turrets](#turrets)
	- [Gunship range](#gunship-range)
	- [Soban Carrier](#soban-carrier)
		- [Microwave emitter range](#microwave-emitter-range)
		- [PD railgun ranges](#pd-railgun-ranges)
		- [ALM](#alm)
	- [Baserunner deployable ECM jammer](#baserunner-deployable-ecm-jammer)
- [Gaalsien/Khaaneph](#gaalsienkhaaneph)
	- [Missile ship radar guided missiles](#missile-ship-radar-guided-missiles)
	- [Khaaneph Siege cruiser barrage](#khaaneph-siege-cruiser-barrage)

# General changes

## Target prioritization
> *All units should have more intelligent targeting. Certain units used to have very high base priority, and railguns didn't properly have weapon effectiveness weight set to matter in most situations. Railguns should now switch targets based on weapon effectiveness, for example, from strike craft/salvagers to enemy railguns.*

* Implemented target prioritization fixes

## Carrier weapons
> *There's no + indicating high ground, removed this ambiguous functionality.*

* Removed carrier point defense and missile high ground advantage

## Nuke-class weapons
> *This change doesn't impact Khaaneph cruise missiles*

* Carrier nuke-class weapons are no longer affected by high ground

## Carrier point defense weapon tracer graphics
> *The tracers should land around the target they're firing at, rather than sometimes flying off to random directions.*

* Switched carrier PD tracers to flak mode targeting mode on missed shots

## Unit reveal time
> *All railguns (includes honourguard cruisers) stay visible until next shot, allowing enemy units to not lose their forced attack target orders. Carriers get the same change due to their range often being longer than unit vision range*

* Increased railgun and carrier reveal time: `2.5s => 4.5s`

## Air sortie duration
> *For optimal use of air in Deserts of Kharak it is often important to keep them in the air for a long time. This requires constantly queuing a lot of move commands to them, straining the player for a menial task. Increased sortie duration should make this a lot simpler, air units will float around their loiter destination longer, making it easier to keep them in the air for as long as necessary.*

* Air sortie duration: `15s => 40s`

## Aircraft hangar size
> *Filling out carrier aircraft hangers is almost never achievable in Deserts of Kharak except for situations of 3v3. In those instances, it is a common strategy to snipe carriers with the massive payload that these highly mobile units can deliver almost anywhere on the map. Reducing the strength of this strategy specifically to prevent this almost certainly unintended gameplay interaction.*

* Aircraft hangar size: `15 => 12`

## Nuke costing popcap while active/in flight
> *The fake unit that gets created at the point of impact of some nukes used to cost population.*

* Removed nuke sight reveal fake units popcap cost

# Coalition/Soban

## Carrier handling
> *Changes should result in much more responsive CV handling.*

* Max ease into turn time: `5s => 1s`
* Acceleration / deceleration times: `2s => 1.1s`
* Turn radius: `150 => 130`

## Support cruiser handling
> *Should result in much more responsive handling.*

* Max ease into turn time: `3s => 0.8s`

## Turrets
> *Gun turret will be capable of shooting slightly over hills, making their placement easier.*

* AA turret - no longer affected by high ground
* Adjusted turret - adjusted world height offset.

## Gunship range
> *This fixes issues with it targeting what it's firing, without constant human micro the gunship will still float around the target when attacking at the same distance as before.*

* Gunship weapon range: `700 => 1050`

## Soban Carrier

### Microwave emitter range
> *Prevents base denial cheese*

* MWE range: `35000 => 4500`

### PD railgun ranges
> *Level 0 range is 900, meaning this power level was reducing carrier range in vanilla.*

* Level 1: `800 => 1100`
* Level 2: `1100 => 1300`
* Level 3: `1400 => 1500`
* Updated descriptions
* Adjusted some mid/short range brackets slightly
* Fixed an issue where front right turret range wasn't updated correctly at Level 4 power level

### ALM
*ALMs will be capable of shooting slightly over hills, making their placement slightly easier.*

* Adjusted world height offset
* Adjusted aggro range

## Baserunner deployable ECM jammer
> *ECM jammer would previously always be visible in fog of war with a ping.*

* Fixed soban ECM jammer always being "contacted"

# Gaalsien/Khaaneph

## Missile ship radar guided missiles
> *Radar guided missiles used to reduce turret rotation instead of increasing it.*

* Turret rotation base speed and firing cone reduced slightly
* Radar guided missiles upgrade now correctly increases turret rotation speed

## Khaaneph Siege cruiser barrage
> *Made KSC barrage behavior consistent with other artillery barrages.*

* KSC barrage is no longer affected by high ground
