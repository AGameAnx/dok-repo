
* General:
	* Carrier nuke-class weapons are no longer affected by high ground. *This change doesn't impact Khaaneph cruise missiles*
	* Carrier PDs and missiles high ground advantage: `removed`. *there's no + indicating high ground, removed this ambiguous functionality*
	* Improved carrier PD tracer graphics. *The tracers should land around the target they're firing at, rather than sometimes flying off to random directions*
	* Target prioritization fixes: `implemented`. *more intelligent unit targeting, railguns should switch targets towards armored units*
	* Carrier/railgun reveal time: `increased`. *all railguns stay visible until next shot, allowing enemy units to not lose their forced attack target orders*
	* Air sortie duration: `15s => 40s`. *should make air control a lot less straneous, air units will float around their loiter destination longer, making it easier to keep them in the air for as long as necessary*
	* Aircraft hangar size: `15 => 12`. *Reducing carrier snipe potential*
	* Removed nuke sight reveal fake units popcap cost
* Coalition/Soban:
	* Carrier: *should result in much more responsive handling*
		* Max ease into turn time: `5s => 1s`
		* Acceleration / deceleration times: `2s => 1.1s`
		* Turn radius: `150 => 130`
	* Support cruiser movement dynamics max ease into turn time: `3s => 0.8s`
	* AA turret - no longer affected by high ground
	* Gunship range: `700 => 1050`. *This fixes issues with it targeting what it's firing
* Coalition:
	* Turret - adjusted world height offset. *Turret will be capable of shooting slightly over hills, making their placement slightly easier.*
* Soban:
	* Carrier:
		* MWE range: `35000 => 4500`. *Prevents base denial cheese*
		* Railgun ranges:
			* Level 1: `800 => 1100`. *Level 0 range is 900, meaning this power level was reducing carrier range in vanilla*
			* Level 2: `1100 => 1300`
			* Level 3: `1400 => 1500`
			* Updated descriptions
			* Adjusted some mid/short range brackets slightly
			* Fixed an issue where front right turret range wasn't updated correctly at Level 4 power level
		* ALM:
			* Adjusted world height offset. *ALMs will be capable of shooting slightly over hills, making their placement slightly easier.*
			* Adjusted aggro range
		* Baserunner deployable ECM - Fixed an issue of this unit always being "contacted"
* Gaalsien/Khaaneph:
	* Missile ship:
		* Turret rotation base speed and firing cone reduced slightly
		* Radar guided missiles upgrade now correctly increases turret rotation speed
* Khaaneph:
	* Siege cruiser barrage is no longer affected by high ground. *Makes that consistent with other artillery barrages.*
