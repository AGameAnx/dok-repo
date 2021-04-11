# Jaraci patch v12 changes so far

**Focus behind patch**:
- Fix the situation of 3 base greed being too easy and stable to execute.
- Provide a more permanent solution to C/S carrier move outs being the center point of their metagame.
- Improve G/K midgame variety - allow aggressive options which require two production slots without buffing
    faction greed.
- Improve lategame - reduce overall cruiser count while preserving cruiser usefulness, increase flanking
    opportunities.
- Create a greater emphasis on population capacity without making army size prohibitively small, allow players
    to make army trading mistakes increase overall trading in lategame through population limit and resource
    income changes.
- Reduce the strength of mid-lategame strike craft counters while keeping strike craft balanced for early game.
- Tighten up interactions of all midgame units.
- Make railgun midgame plays more viable, fix C/S railgun balance in general.
- Increase power level of individual battlecruiser units, make them more capable of operating outside the main
    blob.
- Reduce coin-flippy nature of certain early game build orders.
- Improve the feeling of C/S carriers feeling too squishy in the early game.
- Improve UX consistency and bug situation.

## Changes:
* General:
	* Salvagers: 
		* Population cost: `1 => 2`
			> Population cost change helps out aggressive styles in terms of keeping up with greedy styles
			> because greedy styles need the first and second population upgrade / module at around the same
			> time with the new population cost change
		* Fixed an issue where G/K RU storage wasn't modified": `40 => 20`
			> This change was implemented since the start of jaraci, but G/K salvagers were never modified.
			> LDM will become less efficient, but less manual dropoffs will be required for normal gameplay
		* Salvager mining (extends resource patch duration):
			> General result of these changes is that players receive exact amount of resources per unit of
			> time as before, but the patches run out at half speed. Note that the numbers displayed above
			> patches will also deplete at half rate now, so people min-maxing their dropoffs and scouting
			> enemy patches will need to account for this. Unfortunately there isn't a way to globally
			> modify the actual patches for now. In testing, this results in main base never mining out and
			> therefore an extra overall area of ground needing to be defended. Population cap starts to play a
			> role as income doesn't dry out by the time it becomes a factor, producing many more fights and
			> action in games than previously
			* Each collected RU resource now worth 2 when dropping off
			* CU collected from patch per cycle: `2 => 1`
			* RU cycle duration multiplier: `1 => 2`
		* Reduced target priority
	* Baserunner AA range: `1100 => 1250`
		> This change is mostly to improve baserunner capability to zone out probe, but soft-countering air
		> with baserunners has also proven mostly not viable without the AA turret
	* "Incoming missile" (nuke) indicators:
		> Nukes providing sight is more important than one would expect. Having perfect vision in an area helps
		> plan your attack, helps units pick their targets, helps the player assess the situation better as well
		> as the damage the nuke has caused while there is no logical justification for sight in the area to
		> exist, aside from letting the player watch the fireworks. Unfortunately that will have to be
		> sacrificed in order to improve lategame fights. Additionally, fixing a plethora of weird edge-case
		> bugs that these indicators had
		* No longer provide sight in the targeted area
		* Fixed an issue where these indicators could get destroyed by area of effect damage
		* Fixed additional issues where these indicators cost population
	* Railgun:
		> Railgun range reduction helps the case of them fighting around the carrier. The carrier becomes a much
		> bigger nuisance for the railguns in the vicinity. Generally speaking, this should provide a positive
		> effect gameplay-wise in terms of playing around railguns and allowing me to increase overall railgun
		> power without being too afraid of railgun blobbing becoming a large issue. The range reduction was
		> always planned, but couldn't be done without new Subsystem functionality. The other modified fields
		> are to make railguns approach the target properly when a-move, ctrl-box or right click commands are
		> used
		* Max range: `2050 => 1850`
		* Aggro range: `2050 => 1850`
		* Max desired combat range: `2050 => 1780`
		* Damage modifier against strike craft: `60% => 50%`
	* Sunder:
		> This, along with v11 changes, increases railgun synergy with midgame units drastically. After testing
		> this seemed to only increase the overall micro and fun potential of midgame combat, as well as scaling
		> fine in lategame. A good buff for railguns without also buffing railgun blobbing strategies
		* Armor reduction: `5 => 7`
		* Fixed ability descriptions
	* Target prioritization adjustments for low damage units (AAV, AS, Sandskimmer, LAV)
		> Many of these units did not get properly affected by unit personal target priority, but now do. Should
		> result in more logical target selection in all cases
* Coalition/Soban:
	* Carrier:
		> Carrier mobility upgrade is a lever that will finally allow properly balancing carrier move-outs and
		> all-ins without having to gimp the feeling of the carrier in the lategame. There are also implications
		> of this change defensively, which I've addressed with additional early game firepower of the carriers.
		> It's also not out of the question to make moveouts without the mobility upgrade but with cheaper
		> overall power for the carrier and earlier nuke
		* Base speed: `45 => 37`
		* Max ease into turn time: `0.5s => 0.25s`
		* Carrier systems upgrades:
			* Renamed to exclude carrier systems 2
			* Level 2 upgrade repurposed:
				* Name: `Carrier Systems 2 => Carrier Mobility`
				* No longer requires power lever 1 to be purchasable
				* Cost: `400CU 175RU => 600CU 300RU`
				* Hitpoints granted: `150 => 0`
				* Extra speed granted: `1 => 13`
				* Grants 2 power as before (can't modify)
			* Level 3 (shows up as level 2):
				* Dependency: `Carrier systems 2 => Carrier systems 1`
				* Cost: `650CU 250RU => 600CU 200RU`
			* NOTE: Cruise missile now available at power level 4 and microwave emitter upgrade at power level 3
	* Production upgrade level 1 cost: `350CU 40RU => 500CU 50RU`
		> Part of the effort to make stabilization after greed more difficult
	* Baserunner probe cost: `100CU => 150CU`
		> Probe is a central part of C/S greed being overpowered and completely safe. This is somewhat of a band
		> aid solution for now, as there are other issues, such as cases where players buy probe right away and
		> still salvage the baserunner, resulting in that being objectively the best play every time. More
		> testing is required to determine the validity of such concerns
	* Support cruiser:
		> The problem with support cruisers being fast to build is the ability of players to quickly mix them in
		> in the middle of aggressive plays and going back with pressure, essentially making midgame pressure
		> plays unbelievably difficult to answer (taking any damage is guaranteed to put the defender too far
		> behind). This also helps address the situation of stabilizing too quickly after very greedy plays. The
		> hitpoint reduction is due to lategame blobbing being too powerful where area of effect abilities could
		> not properly address support cruiser blobbing together with other cruisers. Movement parameter changes
		> are to somewhat mitigate the frustrations of controlling these units and to help out with using these
		> units as heal providers outside blobbing strategies, for generally quicker repositioning without the
		> frustration of these units getting "stuck" behind. Note that 2 bombers now kill support cruisers in
		> mirror
		* Build time: `35s => 40s`
		* Hitpoints: `3200 => 2700`
		* Armor: `4 => 5`
		* Acceleration time: `1.5s => 0.9s`
		* Max ease into turn time: `0.8s => 0.25s`
	* LAV:
		> LAV were heavily affected by turret rotation in brawl situations. Using hold position or chase
		> situations resulted in much higher damage output on LAVs than anticipated. Besides this, strike craft
		> has been somewhat too weak in high level play due to various sources of AOE being utilized to properly
		> prevent run-ins. Damage modifier against air is also due to turret rotation changes, they might even
		> be stronger right now despite the nerf due to how much this affected their weapon previously
		* Hitpoints: `420 => 440`
		* Boost ability research cost: `200CU 125RU => 150CU 200RU`
		* Accuracy: `90%/85%/56% => 85%/82%/55%`
		* Burst duration: `0.95-0.115s => 0.95-0.105s`
		* Turret rotation: `250 => 390`
		* Damage against air: `70% => 50%`
	* Vehicle armor upgrades cost:
		> Part of the general effort to increase viability of midgame strategies
		* Level 1: `250CU 100RU => 200CU 100RU`
		* Level 2: `250CU 200RU => 250CU 175RU`
		* Level 3: `300CU 300RU => 300CU 250RU`
	* AAV:
		> AAVs felt a bit too strong in terms of their damage output. Their survivability is nerfed for a
		> general shift of the unit towards a more balanced role where this unit is countered by railguns but is
		> generally a solid choice for stalling/flanking/midgame tempo plays. Reintroducing AOE for the 3rd time
		> mainly to give a slight deterrent to enemies from stacking things together. It was undoubtedly the
		> best way to fight AAV with AS before, for instance, where stacking only had upsides
		* Tech cost: `400CU 75RU => 350CU 75RU`
		* Cost: `260CU 20RU => 270CU 20RU`
		* Armor: `8 => 7`
		* Movement speed: `82 => 83`
		* AOE: `0 => 40` (Linear falloff)
		* ROF: `15 => 13`
		* Range: `1000 => 975`
		* Suppression slow effect: `55% => 40%`
	* Railgun:
		> Much easier access early on for aggro purposes. Much harder to spam. Higher alpha-damage overall and
		> higher DPS. It was deemed that railgun strategies are too weak overall and needed changes. Wind up and
		> higher base damage allow railguns to function better around rough terrain
		* Tech cost: `300CU 100RU => 200CU 100RU`
		* Research time: `55s => 45s`
		* Cost: `280CU 70RU => 300CU 80RU`
		* Production time: `16s => 22s`
		* Armor: `2 => 1`
		* Damage: `155 => 180`
		* Wind-up: `1.6s => 1.2s`
		* Reload C/S: `1.8s/4.2s => 1.8s/4.7s`
		* Range: `1850 => 1900`
		* Aggro range: `2050 => 1900`
		* Max desired combat range: `2050 => 1830`
		* Mag accelerator:
			* Research cost: `150CU 220RU => 150CU 250RU`
			* Damage increase: `25 => 20`
	* Strike fighter and gunship fabrication tech cost: `400CU 200RU => 500CU 200RU`
		> Coalition air and air switches were deemed too powerful overall
	* Strike fighter cost: `200CU 90RU => 220CU 90RU`
	* Gunship:
		> Part of nerfs to lategame strike craft counters
		* Population cost: `3 => 4`
		* Damage: `42 => 38`
	* Bomber:
		> Bombers were quite difficult to kill even when interceptors were out on the field, and are generally
		> an insanely powerful counter to railguns and assault railguns. Slight nerfs while still keeping unit
		> power level high
		* Hitpoints: `1350 => 1300`
		* Armor: `15 => 10`
		* AOE: `200 => 190`
	* Battlecruiser:
		> The result of these changes should be a much more intimidating unit on its own that's a lot less
		> susceptible to AOE damage than before and much more capable of barreling through enemy defensive
		> setups. The self heal makes this unit a lot more useful on flanks and stops the problem of these units
		> requiring a whole extra crew of support cruisers to sustain. High number of BCs was deemed oppressive,
		> however, therefore the unit cost was increased rather drastically, even if tech availability was
		> improved. The fact that field repair immobilizes the unit makes it a lot harder to use this ability
		> when already in combat (albeit still highly viable), as well as granting this unit the trait of being
		> a slow tank rather than a unit which can respond to threats
		* Research cost: `550CU 300RU => 500CU 250RU`
		* Research time: `110s => 100s`
		* Cost: `650CU 250RU => 700CU 400RU`
		* Population cost: `6 => 9`
		* Hitpoints C/S: `3400/3200 => 3800`
		* Armor C/S: `17/16 => 20/19`
		* Reload: `3.2s/8.5s => 3.8s/6.3s`
		* Self-Smoke ability:
			* Renamed to: `Field Repairs`
			* Now immobilizes the unit for the duration of being covered by smoke
			* Now heals the unit while active:
				* Tick period: `0.2s`
				* Heal amount per tick: `30`
				* Duration: `10s`
				* Total heal amount: `1500`
	* Assault cruiser:
		> The nerfs are part of the effort to reduce cruiser numbers in the lategame, and this unit was pretty
		> much overpowered in general against nearly all targets. It was performing amazingly well despite the
		> railgun buffs, it was also quite strong as a hard counter to strike craft plays
		* Research cost: `500CU 250RU => 450CU 200RU`
		* Cost: `550CU 220RU => 550CU 260RU`
		* Population cost: `5 => 6`
		* Hitpoints: `2900 => 2800`
		* Ability cooldown: `30s => 40s`
		* Number of bursts: `4 => 3`
		* Damage: `50 => 54`
		* Adjusted target prioritization
	* Artillery cruiser:
		> This unit is performing very well as an option against slow moving enemy units (railguns, HGC) but its
		> power level was overall too high. Making it easier to snipe and making autofire not nearly as insane
		> as it used to be (having a few artillery cruisers would hard counter G/K HRs even without barrages
		> previously)
		* Hitpoints: `1900 => 1600`
		* Autofire:
			* Damage: `140 => 80`
			* Reload: `6.5s => 7.5s`
		* Barrage:
			* Damage: `240 => 220`
			* Cooldown: `80s => 70s`
		* Precision barrage:
			* Damage: `200 => 180`
			* Cooldown: `60s => 70s`
* Coalition:
	* Carrier:
		> C carrier felt too tanky in lategame, but too squishy in the early game. Addressing both and
		> increasing PD damage output to help early game defense after speed reduction
		* Hitpoints: `8900 => 8700`
		* PD rate of fire: `3 => 4`
		* Fixed PD rate of fire tooltip on the weapons system power shunt
		* Reactive armor power systems armor:
			* Level 0: `15 => 20`
			* Level 1: `20 => 25`
			* Level 2: `25 => 30`
		* Cruise missile:
			> Cruise missile often felt underwhelming, even if impossible to dodge. Slight adjustments to both
			> aspects
			* AOE: `500 => 550`
			* "Incoming missile" indicator delay: `2.75s => 1.5s`
* Soban:
	* Carrier:
		> S carrier felt too tanky in lategame, but too squishy in the early game. Addressing both. However,
		> previous iteration of the carrier was quite overpowered damage-output-wise in lategame, therefore the
		> weapons power shunt has been rebalanced
		* Hitpoints: `8500 => 8400`
		* Fixed PD reload and cooldown tooltips on the weapons system power shunt
		* Weapons power shunt reload and cooldown bonuses:
			* Level 1: `35% => 25%`
			* Level 2: `55% => 40%`
			* Level 3: `70% => 55%`
			* Level 4: `85% => 70%`
			* Level 5: `95% => 85%`
		* Range systems range max range:
			* Level 1: `1250 => 1200`
			* Level 2: `1450 => 1350`
			* Level 3: `1650 => 1500`
			* Level 4: `1900 => 1650`
			* Level 5: `2150 => 1850`
		* Reactive armor power systems armor:
			* Level 0: `10 => 15`
			* Level 1: `15 => 20`
			* Level 2: `20 => 25`
		* Microwave emitter:
			> The missile that's being launched has the same visuals as the C cruise missile but had its target
			> revealed much sooner. Normalizing this now. The target icon was also displayed way for a way too
			> short duration in jaraci, which should now be fixed
			* Target icon display duration: `20s => 39s`
			* "Incoming missile" indicator delay: `0.1s => 1.5s`
	* Battlecruiser:
		> This unit still lacks strong identity, but should now be much closer in role to C battlecruiser - a
		> tanky brawler and a lot more powerful in general. It's possible this unit will become overpowered
		> because previous iterations of the unit could already feel oppressive when this unit reached critical
		> mass. The hope is that the new cost as well as population cost push the timing of the critical mass of
		> this unit much further back in the game, and options like EMP are actually possible to get on time to
		> offset the power of such cruisers
		* Damage: `340 => 300`
		* Wind-up: `2.2s => 1.6s`
		* Reload: `7.25s => 6.5s`
		* Accuracy: `7%/6%/5% => 40%/100%/65%`
		* Accuracy modifier against strike craft: `500% => 100%`
		* Damage modifier against strike craft: `100% => 50%`
* Gaalsien/Khaaneph:
	* Salvager cost: `150CU => 180CU`
		> Part of the effort to allow midgame plays for the factions while keeping greed styles in check. Keep
		> in mind that other parts of G/K greed are improved, which hopefully results in greed styles having a
		> similar power level to before. Increasing salvager or det pack costs are the only two levers for
		> slowing down expansion without further nerfing production cruiser cost, which was prohibitively high
		> before
	* Population capacity upgrades:
		> These changes were somewhat required due to salvager population cost increase. The flow of midgame and
		> greed styles was too inhibited by having to stop and purchase these upgrades. Instead G/K now have an
		> inherent advantage early in the game if they want to actually produce units, and a disadvantage/lever
		> of balance for the lategame (where their armies are generally considered to ramp up more quickly)
		* Level 1:
			* Cost: `250CU => 150CU`
			* Research time: `10s => 5s`
		* Level 2:
			* Cost: `310 => 250`
			* Research time: `10s => 7s`
		* Level 3 cost: `390 => 350`
		* Level 4 cost: `490 => 500`
		* Level 5 cost: `610 => 700`
	* Production cruiser cost: `650CU 60RU => 550CU 50RU`
		> 2 PC back on the menu? Not sure yet, but this change at least allows midgame plays
	* Refinery mode tech cost: `550CU 80RU => 550CU 60RU`
		> After extensive testing the greed styles weren't lining up correctly (these tiny cost adjustments are
		> very impactful for early game), and extra edge added to aggro styles which involved 2PCs was deemed
		> acceptable
	* Sandskimmer:
		> After a barrage of nerfs the sandskimmer has received in past months the unit was starting to feel
		> highly underwhelming. It was also affected by reduced combat effectiveness while brawling which should
		> now be fixed with increased hover turn acceleration. Additionally, increasing lategame hitpoint
		> scaling to incentivize lategame usage
		* Hitpoints: `480 => 500`
		* Hover turn acceleration: `75 => 130`
		* Armor upgrade hitpoints granted per upgrade: `20 => 30`
	* Assault ship:
		> The unit was proving very strong in the meta and in early game aggro scenarios. It's receiving slight
		> tweaks to better place it within the new balance and should hopefully breathe some longevity in the
		> unit's usefulness as well, because the unit fell off quite drastically in the lategame in v11 versions
		* Tech research time: `65s => 60s`
		* Build time: `17s => 18s`
		* Hitpoints: `900 => 850`
		* Movement speed: `72 => 76`
		* Damage: `27 => 28`
		* AOE: `140 => 125`
	* Railgun armor upgrade RU cost:
		> Part of the effort to bring midgame units back in the meta, and artillery was having too easy of a
		> time demolishing railguns
		* Level 2: `200 => 175`
		* Level 3: `300 => 250`
	* Assault railgun:
		> ARs were proving to be insanely strong when spammed due to their alpha strike. Rolling back some of
		> the decisions that were made some while ago in making this unit an alpha strike unit, it is now
		> slightly more capable of brawling, but doesn't as easily one shot LAV or other things when spammed.
		> Overall, an expensive but highly versatile option. Aggro range fixes issues with red line appearing
		> incorrectly when a-moving this unit. Dart maneuver has become an essential part of this unit over time
		> and therefore that upgrade has been deemed strong and had its cost increased back to what a normal
		> useful upgrade should cost (still on the cheap side for now, but might change)
		* Cost: `200CU 60RU => 250CU 55RU`
		* Number of bursts: `6 => 5`
		* Reload: `3.6s => 3s`
		* Range: `1100 => 1050`
		* Aggro range: `1650 => 1050`
		* Dart maneuver:
			* Research cost: `50CU 80RU => 150CU 80RU`
			* Cooldown: `35s => 50s`
			* Duration: `3s => 2.7s`
	* Heavy railgun:
		> The damage output of HR has been increased drastically, but it will now suffer from a heavy range
		> disadvantage over C/S railguns, hopefully allowing the railgun rush to be controllable much more
		> easily overall. The power of this unit was deemed much too low in general, so it received many buffs
		> overall, and the only problematic scenario of this unit being blobbed should be counterable now by
		> quite a few means that have become available over the last set of updates to the patch
		* Production time: `24s => 20s`
		* Movement speed: `52 => 61`
		* Hover turn acceleration: `10 => 120`
		* Wind-up: `1.6s => 1.2s`
		* Range: `2100 => 1700`
		* Max desired combat range: `2050 => 1630`
		* Aggro range: `2050 => 1700`
		* Reload: `0.6s => 0s`
		* Ranged calibration:
			> Bringing back power to this upgrade because it is now almost required to fight C/S railguns. Will
			> have to keep an eye on how railgun rush plays out, but LAV is still strong enough to be able to
			> overwhelm players who choose to invest in HRs only. It'll be up to C/S players to properly read
			> the situation and switch from building railguns or LAV with upgrades to defeat the rush, in theory
			* Research cost: `200CU 300RU => 200CU 250RU`
			* Range bonus: `330 => 400`
			* Speed modifier: `-65% => -40%`
	* Interceptor damage packets: `2 => 3`
		> Interceptors were proving too good at sniping cruisers/armored targets
	* Precision bomber:
		> Damage output adjustments, increases hits to kill a production cruiser which is very important for the
		> mirror matchup
		* Damage: `900 => 800`
		* Armor: `15 => 12`
	* Siege cruiser EMP:
		> Highly useful and used upgrade in current testing
		* Upgrade cost: `250CU 100RU => 300CU 100RU`
		* Cooldown: `45s => 75s`
	* Honourguard cruiser:
		> After the initial reduction to polarizing effect this unit had on strike craft battle, this unit was
		> deemed underpowered. Various statistical buffs to the unit, but it is also now more squishy, resembling
		> a railgun more as well as making it more susceptible to consolidated attacks. Hover turn acceleration
		> increase does help this unit keep its target better and turn when it's being outflanked, but should
		> mostly only help with usability. Outflanking this unit should remain rewarding
		* Research cost: `500CU 280RU => 550CU 200RU`
		* Research time: `65s => 60s`
		* Cost: `550CU 250RU => 500CU 250RU`
		* Hitpoints: `2700 => 2400`
		* Speed: `50 => 55`
		* Hover turn acceleration: `1.5 => 5`
		* Damage: `550 => 570`
		* Wind-up: `2.2s => 1.6s`
		* Reload: `5.5s => 5s`
		* AOE: `210 => 170`
		* Fixed AOE inconsistency for K variant
		* Range: `2100 => 1850`
		* Max desired combat range: `2050 => 1780`
		* Falloff: `Quadratic => Linear`
		* AA research cost: `300CU 300RU => 300CU 200RU`
		* AA weapon reload: `3s => 2.7s`
* Gaalsien:
	* Carrier:
		* Hitpoints: `8100 => 8300`
		* Super-sonic missile barrage:
			> Using this ability often feels hard due to its minimum range and vision range being hard to
			> acquire. The fact that it does its damage over a prolonged period of time and over a large area
			> can be useful as a zoning tool but this is almost never the plan that gaalsien wants to execute in
			> a big fight
			* Damage: `240 => 260`
			* AOE: `230 => 245`
	* Baserunner:
		> Self healing often made G baserunners very difficult to snipe. Fast movement speed was providing very
		> reliable scouting information, sometimes allowing G players to get both refinery tech and an extra
		> production cruiser before skimmer tech. Overall the baserunner should still feel very powerful and
		> tanky, these are minor changes
		* Hitpoints: `2000 => 1900`
		* Speed: `80 => 75`
	* Siege cruiser:
		> Now that people have started extensively using this unit, it has become a staple of G metagame. Cost
		> changes are a part of the effort of making cruisers less spammable. The hitpoint and speed reductions
		> should help this unit actually be counterable by means other than air and enemy artillery
		* Cost: `450CU 180RU => 550CU 180RU`
		* Hitpoints: `2000 => 1700`
		* Speed: `66 => 64`
		* Autofire damage: `170 => 150`
		* Barrage damage: `195 => 210`
		* Barrage packets: `2 => 3`
* Khaaneph:
	* Carrier cruise missiles:
		> Cruise missiles were again verging on the too spammable territory. These changes reduce level 5 damage
		> output quite drastically, while helping out with overall aiming of the missiles which should mostly
		> affect early game
		* Base recharge time: `8s => 9s`
		* Damage: `670 => 700`
		* AOE: `140 => 150`
	* Blast drone hitpoints: `540 => 600`
		> BDs are somewhat central to variety of K early game where baserunner isn't retired, buffing hitpoints
		> to increase BD dancing potential with enemy strike craft and to generally increase the appeal of the
		> unit
	* Siege cruiser cost: `700CU 250RU => 700CU 280RU`
		> Part of the effort to reduce cruiser numbers in lategame
