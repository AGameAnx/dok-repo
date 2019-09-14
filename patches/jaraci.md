# General changes

## Carrier power level upgrades
> *Intention of this rebalance is to slightly shift away:** `Strike-craft-centric playstyles when using the carrier as well as reduce the incentive to power up the carrier as early as possible (it should be risky doing this on low tech).*

* **Cost rework:**
    * **Level 1:** `140CU 80RU => 150CU 60RU`
    * **Level 2:** `280CU 160RU => 350CU 150RU`
    * **Level 3:** `460CU 260RU => 650CU 250RU`
    * **Level 4:** `720CU 400RU => 900CU 350RU`
    * **Level 5:** `1100CU 600RU => 1200CU 600RU`
    * **Level 6:** `1300CU 700RU => 1300CU 700RU`
    * **Level 7:** `1500CU 800RU => 1400CU 800RU`

## Carrier range power systems (Gaalsien/Coalition)
> *All railgun and carrier ranges are reduced in the mod as part of the effort to reduce the prevalence of railgun-based strategies.*

* **Level 3:**
    * **Turret max range:** `1400 => 1350`
    * **Missile max range bonus:** `900 => 850`
    * **Sight and contact range:** `600 => 550`
* **Level 4:**
    * **Turret max range:** `1700 => 1550`
    * **Missile max range bonus:** `1200 => 1050`
    * **Sight and contact range bonuses:** `900 => 800`
* **Level 5:**
    * **Turret max range:** `2000 => 1750`
    * **Missile max range bonus:** `1500 => 1250`
    * **Sight and contact range bonuses:** `1200 => 1050`

## Carrier point defense weapons
> *Carrier point defense weapons are some of the most unintuitively designed weapons in the game. A couple of issues include - they do very little damage even at level 5 power systems, they do very low amounts of damage so going from `level 4 to level 5 weapon systems power level makes no difference in a carrier fight (even with changes they still don't, in most cases). Additionally, early in the game on some of the carriers they do almost nothing. These changes make defending against strike craft-based attacks easier in the early game which is a change forced by a particular Khaaneph Blast Drone rush.*

* **Accuracy profiles:**
    * **Short:** `5% or 100% => 50%`
    * **Medium:** `4.5% or 90% => 45%`
    * **Long:** `4% or 80% => 35%`
* **Weapon damage:** `8 or 10 => 18`
* **Penetrating weapon damage:** `17 => 33`
* **Rate of fire:** `See per-carrier changes below`
* **Normalized all modifiers against different target sizes:**
    * **Small:** `5 or 8 => 1`
    * **Medium:** `1, 15 or 18 => 1.15`
    * **Large:** `1 or 2000 => 1.3`
    * **XLarge, Carrier:** `1 or 25 => 1.3`
* **Improved visuals of PDs missing their target**

## Carrier missile systems
> *Missile systems do the majority of carrier's damage, and thus the missile weapon is receiving a reduction in fire rate across all carriers.*

* **Wind-up:** `0 => 0.5s`

## Carrier indirect fire systems (nukes)
> *The range change stems mostly from the fact that soban MWE can be used to extend the lead of a soban player in a really uninteractive way of spamming MWE onto enemy mining operations. Shouldn't affect 1v1 games too much but will be a pretty big change for team games.*

* **Affected by high ground:** `Yes => No`
* **Range:** `35000 to 4500`

## Medium vehicle armor upgrades
> *Armor upgrades affect some combat situations very drastically, making certain units weaker than intended. Maximum armor on upgraded units will be reduced slightly overall, but base armor increased in select cases.*

* **Armor granted:** `Fixed to +1`

## Strike craft damage upgrades
> *This change is aimed at helping strike craft counter heavily upgraded railguns & increasing potential of fully upgraded strike craft strategies. This change wouldn't be a good idea on its own without the consideration of all the other mod changes. Almost all strike craft counts have seen updates/buffs, therefore it has become logical to provide a small bonus to strike-craft based strategies.*

* **CU Cost:** `500 => 400`

## Strike craft armor upgrades
> *Main ways to counter strike craft always involve area of effect but that also means that getting strike craft armor upgrades wasn't very impactful at preventing strike craft:** `getting quickly wiped by their area of effect counters.*

* **Added bonus:** `30 extra hitpoints per upgrade`
* **CU Cost:** `200 => 300`

## Railgun and carrier fog of war reveal duration after firing
> *This is done to make sure slower rate of fire railguns do not cloak in fog of far after firing before firing off the next shot. Previously, soban and coalition railguns would disappear in fog of war between their shots which messes up player micro and makes enemy railguns switch targets or lose targets. Additionally, carriers have the same penalty applied to make it more dangerous to stay on max sensor power shunt and fire at the enemy from a great distance.*

* **All railgun and carrier reveal duration after firing:** `2.5s => 4.5s`

## Railgun target prioritization
> *Railgun target prioritization weights have been reworked to ensure more predictable and smart behavior. Range and angle make less of an impact on railgun target prioritization, but weapon effectiveness is now more important (meaning railguns will prioritize targets that have lower armor but also take high received accuracy from the railguns, which is most likely enemy railguns).*

* **Weapon effectiveness weight:** `10 => 50`
* **Distance weight:** `0.1 => 0.05`
* **Angle weight:** `25 => 10`

## Air sorties
> *The optimal way to use air is to always keep them in the air (as there is no fuel system in the game). The micro requirement for keeping air units in the air was to queue as many commands as possible to make the units fly back & forth and not return to carrier. This change should simply lessen the amount of tedious micromanagement required to use air optimally.*

* **Duration:** `10s => 40s`

## Small arms anti-air weapons
> *In vanilla, anti-air weapons have height advantages against air units. This is very counterintuitive and feels thematically wrong. It also makes balancing air units much more complicated, particularly against small arms based anti-air vehicles.*

* **Affected by high ground:** `Yes => No`

## Salvager RU hold size
> *The combination of RU hold size and mining rate makes long-hauling RUs vastly more efficient than long-hauling CUs. In order to bring the two in line so that long-hauling has the same impact on both resource types, the RU hold size would need to be reduced to 16 RUs. (This is the exact number.) However, 16 RUs would not be an ergonomic hold size. This is part of an effort to reduce the effectiveness of early game RU-based rush strategies (coalition/soban carrier rush, gaalsien railgun rush).*

* **RU hold size:** `40 => 20`

## Baserunner cost
> *Early artifact pressure has become very standard meta and even adjusting artifact timings wouldn't solve some of the issues which are present on certain maps where fast investment into mid-game railgun army could completely lock down the game due to extraction corridor being close enough to artifact pick up locations and main base. Extracting artifacts with multiple baserunners at a time will now require a moderate investment, hopefully reducing the size of an aforementioned railgun army. Additionally, this allows baserunner abilities and baserunner AA weapon to be tuned stronger without the concern of making it a better air counter unit than actual AA tech.*

* **Cost:** `250CU => 250CU 60RU`

## Baserunner anti-air
> *These changes should add some soft early game anti-air to all factions. Surprise air tech can be game ending and blind teching against air is almost a necessity for almost all matchups.*

* **AA weapon dmg:** `5 => 17`
* **Packets:** `0 => 1`
* **Turret rotation speed:** `95(180) => 200`
* **Damage against probes:** `100% => 50%`
* **Ranges:**
    * **Short:** `600(300) => 700`
    * **Medium:** `900(600) => 1100`
* **Accuracy:**
    * **Short:** `100(75) to 90`
    * **Medium:** `100 to 80`
* **Gaalsien BR long range:** `Set to unused`
* **Removed unused modifiers against ground targets**

## Artillery barrages (except Khaaneph)
> *These changes don't apply to Khaaneph Siege Cruiser, although it has seen a different rework (see below). The idea behind these changes is to make immediate impact of artillery barrages lower but allow them to deny an area for longer and have a larger overall impact on the battle. This should allow artillery to better counter railgun high ground positions and better punish less attentive play.*

* **Damage against small targets:** `100% => 50%` 
* **Damage against carriers:** `100% => 60%`
* **Autofire:** `Has same modifiers as main barrage`
* **Burst:** `1s => 1.7s`
* **Rate of fire:** `4 => 3`
* **Number of bursts:** `8(3) => 6`
* **Cooldown:** `0.5s => 1.6s`

# Coalition / Soban

## Coalition carrier general statistics
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. Worth noting that these changes coinside with railgun nerfs, however. Movement speed nerf is part of an effort to fix a particularly strong early game 1 base carrier timing push.*

* **Hitpoints:** `15000 => 12000`
* **Movement speed:** `60 => 53`

## Cruise missile:
> *Coalition cruise missile's destructive potential is unmatched. A reduction of its effectiveness against smaller units should make it tougher to extract very high value from it on a consistent basis while keeping overall strategic value of an expensive nuke-class weapon appropriately high.*

* **Cooldown:** `120s => 150s`
* **Damage:** `5000 => 2500`
* **AOE:** `500 => 470`
* **Damage against cruisers and carriers:** `100% => 180%`

## Coalition point defense weapons
> *Lower level PD performance increased (due to BD rush), but higher level rate of fire reduced (due to damage rework of carrier PD weapons)*

* **Rate of fire:** `2 => 7`
* **Weapon Systems power shunt PD rate of fire bonuses:**
    * **Level 1:** `'set to 5' => 'increase by 25%'`
    * **Level 2:** `'set to 10' => 'increase by 50%'`
    * **Level 3:** `'set to 20' => 'increase by 100%'`
    * **Level 4:** `'set to 40' => 'increase by 150%'`
    * **Level 5:** `'set to 40' => 'increase by 25%'`

## Soban carrier general statistics
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. The soban carrier hitpoint nerf is larger than other carriers because it gets strong railgun weaponry from the beginning of the game and extra range for safer positioning. Movement speed and armor changes are part of an effort to fix a particularly strong early game 1 base carrier timing push*

* **Hitpoints:** `15000 => 10700`
* **Movement speed:** `60 => 53`
* **Base armor:** `25 => 15`

## Soban carrier armor system power shunt
> *Soban carrier is particularly strong for the carrier rush. It is meant to be a long range support carrier and thus it is getting its armor reduced across all levels of armor power shunt, including the base armor*

* **Level 1:** `30 => 25`
* **Level 2:** `40 => 35`
* **Level 3:** `60 => 50`
* **Level 4:** `100 => 70`

## Soban carrier point defense railguns
> *The new iteration of these railguns works much closer to how soban railgun units work.*

* **Damage:** `165 => 195`
* **Number of bursts:** `10 => 2`
* **Burst:** `1s => 0.25s`
* **Cooldown:** `5s => 10s`
* **Reload:** `10s => 15s`
* **Wind-up:** `1.6s => 0.8s`
* **Range:**
    * **Medium:** `600 => 550`
    * **Long:** `900 => 850`
* **Accuracy:**
    * **Medium:** `5.3% => 5%`
    * **Long:** `5% => 4.5%`

## Soban carrier turret network power shunt
> *The goal is to make soban carrier a relatively powerful brawler against armored targets, while keeping its overall damage output at bay and keeping the carrier weak against strike craft.*

* **Level 1:**
    * **Reload:** `'Set to 10s => 'decrease by 35%'`
    * **Cooldown:** `'Set to 5s' => 'decrease by 35%'`
    * **Accuracy bonus:** `10% => 15%`
* **Level 2:**
    * **Reload:** `'Set to 6s => 'decrease by 55%'`
    * **Cooldown:** `'Set to 3s' => 'decrease by 55%'`
* **Level 3:**
    * **Reload:** `'Set to 4s => 'decrease by 70%'`
    * **Cooldown:** `'Set to 2s' => 'decrease by 70%'`
    * **Accuracy bonus:** `40% => 35%`
* **Level 4:**
    * **Reload:** `'Set to 2s => 'decrease by 85%'`
    * **Cooldown:** `'Set to 1.5s' => 'decrease by 85%'`
    * **Accuracy bonus:** `50% => 45%`
* **Level 5:**
    * **Reload:** `'Set to 2s => 'decrease by 95%'`
    * **Cooldown:** `'Set to 1s' => 'decrease by 95%'`
    * **Accuracy bonus:** `60% => 55%`
* **Fixed a number of issues with reload and cooldowns of select PD weapons being updated incorrectly**
* **No longer setting the damage of the dummy weapon to 160 on every power level**

## Soban carrier range systems power shunt
> *Soban carrier receives slightly more range than other carriers across all power levels*

* **Ranges:**
    * **Level 1:** `800/550/300 => 1100/800/450`
    * **Level 2:** `1100/750/400 => 1450/1200/700`
    * **Level 3:** `1400/950/500 => 1650/1300/900`
    * **Level 4:** `1700/1150/600 => 1850/1500/1100`
    * **Level 5:** `2000/1350/700 => 2050/1800/1300`
* **Fixed an issue where front right turret range wasn't updated correctly at Level 4 power level**

## Soban carrier ALM power shunt
> *Generally, ALM should be much worse at stun-locking opponent units, but also more capable at dealing damage which helps win defensive engagements (see ALM unit changes below).*

* **Sensors range:**
    * **Level 1:** `1100 => 1000`
    * **Level 2:** `1300 => 1100`
    * **Level 3:** `1600 => 1200`
    * **Level 4:** `1900 => 1300`
    * **Level 5:** `2200 => 1500`
* **Contact radius:** 
    * **Level 1:** `1400 => 1300`
    * **Level 2:** `1600 => 1400`
    * **Level 3:** `2100 => 1500`
    * **Level 4:** `2500 => 1700`
    * **Level 5:** `3000 => 1900`
* **Reload time:**
    * **Level 1:** `4s => 7s`
    * **Level 2:** `3s => 6s`
    * **Level 3:** `2s => 5s`
    * **Level 4:** `1s => 4s`
    * **Level 5:** `0.4s => 3s`
* **Deployment range bonus:**
    * **Level 2:** `1000 => 800`
    * **Level 3:** `1500 => 1000`
    * **Level 4:** `1800 => 1200`
    * **Level 5:** `2000 => 1500`
* **Damage bonus:**
    * **Level 4:** `10 => 30`
    * **Level 5:** `20 => 50`

## Soban microwave emitter:
> *Microwave emitter is the weakest nuke-class weapon and therefore is receiving some buffs.*

* **Cooldown:** `90s => 110s`
* **Cost:** `500CU => 400CU`
* **Impact damage falloff:** `Linear => Quadratic`
* **Duration:** `20s => 30s`
* **Damage packets:** `1 => 0`
* **Base damage per tick:** `170 => 100`
* **Burst:** `1s => 0.25s`
* **Damage against strike craft and salvagers:** `100% => 50%`
* **Damage against Carrier, XLarge and Large class targets:** `100% => 120%`
* **Removed the 500 damage per second status affect on friendly units**

## Armed logistics module
> *It's a bit too difficult to micro around ALMs and they provide too much early game safety. To offset the reload and area of effect changes ALM damage is upped considerably.*

* **Damage:** `40 => 120`
* **Damage packets:** `1 => 2`
* **AOE:** `100 => 90`
* **Target prioritization fixes:**
    * **Distance weight:** `0.1 => 0.25`
    * **Angle weight:** `25 => 10`

## Support cruiser
> *Aim of the cost change is to slow down tech progression when expanding. Currently, there's almost no downside and slow down when expanding from 2 to 3 base, this should make the tech progression just slightly slower which could prove meaningful vs aggressive enemy strategies. Added repair rate helps C/S sustain in lategame positional battles*

* **Cost:** `600CU => 580CU 40RU`
* **Turn radius:** `100 => 85`
* **Population:** `6 => 5`
* **Armor:** `2 => 3`
* **Repair rate:** `10 => 12`

## Support cruiser anti-air
> *Support cruiser AA is the strongest AA in the game by a large margin. Such a high hitpoint body shouldn't have strong AA capability. This capability is also achieved through a single upgrade while SC is already a very useful and needed unit. The strength of this upgrade currently makes most other AA sources obsolete, and is a very easy and obvious choice of an upgrade to purchase.*

* **Upgrade cost:** `500CU 320RU => 450CU 250RU`
* **Wind-up:** `0ms => 50ms`
* **Rate of fire:** `2 => 1`
* **AOE:** `40 => 80`
* **Range:** `1550 => 1400`

## Baserunner probe
> *Probe is slightly too fragile and it often feels random whether it dies or not when it flies into any kind of early game anti-air even if pulled back instantly. The probe is rebalanced along with production cruiser AA and baserunner AA to be more consistent in its interactions with them. Cost is changed due to probes being a bit too much of a no-brainer choice for covering flanks & scouting the enemy.*

* **Hitpoints:** `100 => 170`
* **Sensors radius:** `1000 => 1130`
* **Cost:** `100CU => 150CU`

## Baserunner AA turret
> *Generally using this turret is quite undesirable and almost never worth the original cost investment.*

* **Anti-air turret post cost:** `350CU => 200CU`

## Baserunner gun turret
> *Turrets become slightly less self-sufficient. Hitpoints is a change to prevent blast drones from 1-shotting the turret.*

* **Vision range:** `1200 => 1000`
* **Hitpoints:** `600 => 700`
* **Armor:** `5 => 2`

## Baserunner gun turret weapon rework:
> *The goal of this rework is to make baserunner turret slightly more effective against armored targets and to also fix some issues with its performance such as it firing behind dunes. This new iteration of the turret will allow for greater micro potential against it with strike craft and it'll be slightly better at countering highly upgraded tanks. With accuracy always being 100% the turret will always 1-shot skimmers which aren't upgraded with level 2 armor or aren't pulled away.*

* **Base damage:** `30 => 55`
* **Rate of fire:** `14 => 5`
* **Number of bursts:** `2 => 12`
* **Cooldown:** `0.1s => 0`
* **Burst:** `0.8-1s => 0.2s`
* **Reload:** `2s => 2.2s`
* **Accuracy:** `95%/85%/75% => 100%/100%/100%`
* **Turret rotation speed:** `180 => 150`

## Soban baserunner targeting jammer
> *Extremely situational ability which wasn't very useful even when used in its perfect case scenarios.*

* **Cost:** `150CU => Free`
* **Sensors radius:** `0 => 270`
* **Contact radius:** `0 => 400`
* **Fixed an issue of this unit always being "contacted"**
* **Status effect:**
    * **Max speed reduction:** `10% => 20%`
    * **Turn radius increase:** `5% => 10%`
    * **Acceleration increase:** `0 => 10%`
    * **Added a unit behavior modifier which makes units try to keep a distance of 400 units away from their target while inside ECM field (this is to prevent AI from endlessly circling the ECM with strike craft)**

## Tank armor upgrades
> *It was previously too much of an obvious choice to always upgrade level 3 on armored vehicles which massively increased their combat performance without much of an initial investment.*

* **Level 3 cost:** `300CU 300RU => 300CU 400RU`

## LAV
> *LAV have been revealed as a centerpoint of effective coalition play. Oppressive early game strategies along with LAV providing a strong mid/late game defensive core for the coalition army is the main reasoning behind the reduction of overall LAV effectiveness. Due to the mod increasing the power of various strike craft counters, LAV have become extremely fragile in the lategame and their large discrepancy with sandskimmer hitpoints has been a big issue in balancing various area of effect units. New LAV hitpoints will make them sustain damage a bit better. New LAV weapon makes them slightly weaker against lightly armored targets but slightly more effective against armored ones.*

* **Build time:** `8s => 9s`
* **Hitpoints:** `500 => 570`
* **Armor:** `0 => 1`
* **Weapon:**
    * **Base damage:** `15 => 16`
    * **Rate of fire:** `5 => 4`
    * **Burst:** `0.8s-1.2s => 0.95s-1.05s`
    * **Burst count:** `4 => 2`
    * **Cooldown:** `0.8s => 0.42s`
    * **Turret rotation speed:** `180 => 250`
    * **Damage against probes:** `100% => 50%`

## AAV survivability
> *The hitpoints are reduced on AAV to make soft-countering them with units such as assault ships or interceptors more of an option than it previously was. Previously, AAV would drive past a lot of things to target the squishier targets such as enemy salvagers. This is still possible, but the enemy can react to it easier.*

* **Hitpoints:** `1400 => 1200`
* **Base armor :** `8 => 10`

## AAV pricing
> *AAV timing on small maps is a bit too oppressive. Due to an increase of unit's lategame utility, the base cost is going up slightly. AAV are not very effective late game units and are cheap, their population cost doesn't reflect this.*

* **Tech research time:** `50s => 55s`
* **Cost:** `180CU 30RU => 240CU 25RU`
* **Production time:** `14s => 16s`
* **Population:** `3 => 2`

## AAV weapon
> *AAV weapon has notoriously one of the weakest late game weapons present in the game (for example, it dealt only 1 damage per shot to upgraded railguns). These changes will allow it to maintain some damage output against units with upgrades.*

* **Damage:** `11 => 17`
* **Rate of fire:** `20 => 14`
* **Burst:** `0.5-0.6s => 0.5-0.55s`

## Railgun tech
> *These changes are part of an effort to fix a particularly strong early game 1 base carrier timing push. Additionally, mag accelerator is overall too much of a no-brainer upgrade and a cost increase will make it slightly more difficult to acquire, making it more of a decision in midgame to get it quickly.*

* **Research cost:** `450CU 135RU => 450CU 165RU`
* **Build time:** `14s => 16s`
* **Mag accelerator upgrade cost:** `280CU 165RU => 280CU 190RU`

## Railgun movement speed
> *The speed now matches gaalsien heavy railgun speed. This makes it possible to retreat the gaalsien railguns from a fight.*

* **Max speed:** `66 => 57`

## Railgun accuracy
> *These changes are part of an effort to make high ground more impactful for railguns (as it affects unit accuracy).*

* **Medium range:** `5.3% => 5%`
* **Long range:** `5% => 4.5%`

## Railgun range
> *All railgun and carrier ranges are reduced in the mod as part of the effort to reduce the prevalence of railgun-based strategies.*

* **Range:** `2100 => 1900`

## Coalition railgun
> *Railguns have seen a large redesign in the mod, where their damage per shot has been reduced, cost increased, but hitpoints also increased. Railgun battles now resolve themselves slower, and high ground advantage plays a much larger role.
Coalition railguns have also seen some reload time buffs to go alongside target priority & reveal time changes to bring cost / damage output closer to the insanely high values that gaalsien railguns have in that category.*

* **Cost:** `200CU 60RU => 220CU 85RU`
* **Hitpoints:** `670 => 750`
* **Armor:** `3 => 2`
* **Experience value:** `350 => 450`
* **Damage:** `225 => 195`
* **Reload:** `3.5s => 2.3s`

## Soban railgun
> *Railguns have seen a large redesign in the mod, where their damage per shot has been reduced, cost increased, but hitpoints also increased. Railgun battles now resolve themselves slower, and high ground advantage plays a much larger role.
Soban railguns are extremely powerful, they have superior dps, superior hitpoint pool, superior armor and mag accelerator upgrade benefits them more than the coalition railgun. Additionally, they have mark target ability which comes for free. The gap between coalition and soban railgun performance has been lessened significantly, but soban railgun remains the most cost efficient railgun in the game.*

* **Cost:** `210CU 60RU => 240CU 85RU`
* **Hitpoints:** `680 => 750`
* **Armor:** `4 => 1`
* **Experience value:** `350 => 470`
* **Damage:** `165 => 135`
* **Cooldown:** `2s => 1.5s`
* **Reload:** `2.5s => 1.85s`

## Missile battery
> *The largest factor of AA doing its work vs normal air strategies is the first shot. Increased reload duration means AA will have a much harder time quickly killing off large numbers of air and heavy air and both of those strategies are underused, however it won't affect the early game air rush situations very much. Additionally rebalancing cost, lowering armor to make out of position batteries more punishable and increasiing speed to ease the use of this unit*

* **Cost:** `350CU 80RU => 300CU 90RU`
* **Speed:** `50 => 60`
* **Armor:** `5 => 3`
* **Reload:** `2s => 3s`

## Missile battery mortar ability
> *Mortar damage was extremely polarizing. When hitting enemy units from the high ground it had the potential to make game-winning plays of wiping entire enemy strike craft forces, but when hitting normally the damage could end up irrelevant. These changes should make this ability much more consistent in its performance, killing off strike craft in the center, and damaging a good chunk around them in a healthy area of effect.*

* **Benefits from high ground:** `Yes => No`
* **Falloff:** `None => Quadratic`
* **Damage packets:** `20 to 40`
* **AOE:** `180 to 205`
* **Damage:** `450 to 660`

## Assault cruiser
> *Assault cruiser becomes slightly worse at brawling against other cruisers and armored vehicles but gets help in other areas such as its cost, its hitpoints and its abilities. Weapon and armor changes will allow mid-tier units to soft-counter out of position assault cruisers in some fringe situations, whereas previously assault cruisers were very hard to weed out even by much superior numbers when they were positioned behind dunes.*

* **Tech research cost:** `600CU 350RU to 500CU 300RU`
* **Cost:** `500CU 250RU to 400CU 220RU`
* **Population:** `6 to 4`
* **Hitpoints:** `2700 to 2800`
* **Armor:** `15 to 12`
* **Missile barrage benefits high ground:** `Yes => No`
* **Cooldowns:**
    * **Missile barrage:** `60s => 40s`
    * **Active regeneration:** `50s => 40s`
    * **Overdrive:** `80s => 40s`
* **Overdrive armor bonus:** `100% => 25%`
* **Weapon:**
    * **Damage:** `70 => 55`
    * **Rate of fire:** `2 => 3`
    * **Number of bursts:** `2 => 4`
    * **Reload:** `2s => 3.5s`
    * **Wind-up:** `50ms => 0.25s`
    * **Burst:** `1s => 0.7s`

## Assault cruiser AA upgrade
> *This upgrade is very weak, especially because the AA weapon is weaker than normal AA, a cost reduction should make it more desirable.*

* **AA upgrade cost:** `500CU 340RU => 300CU 150RU`

## Battlecruiser
> *The unit is overall unreasonably expensive for utility and options that it provides for the player. Area of effect changes allow battlecruisers to deal somewhat meaningful damage against strike craft forces. Unit is receiving large tech and production cost reductions but reduced survivability*

* **Tech cost:** `700CU 450RU => 550CU 350RU`
* **Armor:** `25 => 16`
* **Movement dynamics characteristics:**
    * **Max speed:** `50 => 54`
    * **Acceleration time:** `1.5s => 1.2s`
    * **Braking time:** `1s => 0.9s`
    * **Turn radius:** `200 => 130`

## Coalition battlecruiser
> *Damage is reduced in favor of higher rate of fire. This helps the unit deal with medium vehicles easier while also curbing its insane damage potential against carriers*

* **Cost:** `800CU 225RU => 550CU 250RU`
* **Hitpoints:** `6500 => 4200`
* **Damage:** `300 => 180`
* **Reload :** `7s => 5s`
* **Falloff:** `Linear => Quadratic`
* **AOE:** `50 => 55`
* **Range:** `1250 => 1300`

## Soban battlecruiser
> *Long range high damage unit. Very dangerous to have such a unit be also extremely survivable.*

* **Cost:** `780CU 220RU => 550CU 250RU`
* **Hitpoints:** `6500 => 4200`

## Artillery cruiser
> *Getting to artillery should now be much faster and easier. This is designed this way to allow for players to play against enemy railguns without the need of using own railguns, albeit in a still risky way, especially against midgame railgun pushes. Survivability changed to make artillery battles resolve themselves much faster. This makes countering artillery with own artillery less desirable as it's more risky. Additionally, sniping artillery cruisers was too difficult overall.*

* **Tech research cost:** `500CU 350RU => 500CU 250RU`
* **Research time:** `100s => 55s`
* **Cost:** `450CU 250RU => 450CU 200RU`
* **Population:** `6 to 4
* **Construction time:** `70s => 60s`
* **Hitpoints:** `2500 => 2100`
* **Armor:** `5 => 6`
* **Movement dynamics characteristics:**
    * **Max speed:** `50 => 56`
    * **Acceleration time:** `1.5s => 1.2s`
    * **Braking time:** `1s => 0.9s`
    * **Turn radius:** `100 => 90`

## Artillery cruiser autofire
> *Autofire is an extremely unsatisfying mechanic, exceptionally annoying to deal with for an opposing player while requiring little-to-no effort on the part of artillery cruiser users to be effective. It'll remain useful for forcing enemy to constantly micro their units and force the opponent to displace if they are in range, but will ultimately be less punishing and easier to deal with.*

* **Damage:** `200 => 140`

## Artillery cruiser barrages
> *Barrages were pretty difficult to use on most maps against railguns, increased range should help with artillery cruiser usability on a larger variety of maps.*

* **Barrage and precision barrage ranges:** `2400 => 2650`
* **Precision barrage:**
    * **Benefits from high ground:** `Yes => No`
    * **Now has the same modifiers as normal barrage**

## Fighter and gunship fabrication
> *Extremely potent tech for air rushes. Rush potential is reduced substantially but some of its strength is returned through strike fighter, gunship and bomber buffs.*
* **Research cost:** `500CU 200RU => 450CU 280RU`
* **Research time:** `70s => 80s`

## Strike fighter
> *Strike Fighter timings are extremely powerful and strike fighter numbers can grow very fast. These changes aim to reduce strike fighter timing attack strength (especially in CvC matchups, but also against gaalsien railgun openings), and make soft countering strike fighters easier (hitpoint reduction).*

* **Production time:** `15s => 21s`
* **Cost:** `150CU 100RU => 180CU 85RU`
* **Hitpoints:** `650 => 490`
* **Armor:** `2 => 4`
* **Rocket count:** `10 => 8`
* **Rate of fire:** `2 => 3`
* **Burst:** `1000ms => 667ms`
* **Reload:** `3000ms => 3332ms`
* **Field of fire:** `50 => 55`
* **Range:** `1200 => 1250`
* **Max hangar size:** `15 => 12`

## Tactical bomber
> *Very underused unit in the metagame. Costed extremely prohibitively for what it's capable of accomplishing. The rebalanced version of the unit should be very useful at destroying clumped up mid tier army units. Damage changes are made specifically so that 2 bombs are not enough to destroy a production or support cruiser, but double bombers should still be a solid choice for destroying out of position cruisers, with some follow-up (possibly strike fighter).*

* **Research time:** `75s => 55s`
* **Research cost:** `550CU 200RU => 550CU 150RU`
* **Cost:** `500CU 250RU => 350CU 160RU`
* **Population:** `2 to 4`
* **Hitpoints:** `1050 => 1500`
* **Armor:** `15 => 12`
* **Damage:** `2500 => 1850`
* **Damage against Small:** `100% => 60%`
* **AOE:** `180 => 220`
* **Wind-up:** `50ms => 0ms`

## Gunship
> *Increased range to make weapon work more consistently as the gunship circles its target. Unit cost rebalanced to be more of a CU sink than an RU one. Armor decreased to make PC, BR and LAV be slightly more effective at chipping away at it, but total hitpoint pool increased. Weapon packet count reduced, making it significantly more effective against lightly armored targets. Area of effect is increased but added falloff should make gunship's area damage slightly less powerful overall.*

* **Cost:** `380CU 250RU => 500CU 100RU`
* **Production time:** `55s => 45s`
* **Population:** `2 => 3`
* **Hitpoints:** `1050 to 1250`
* **Armor:** `10 => 9`
* **Damage:** `60 => 42`
* **Damage packets:** `4 => 1`
* **AOE:** `150 => 220`
* **Falloff:** `None => Quadratic`
* **Range:** `700 => 1050`

# Gaalsien / Khaaneph

## Gaalsien carrier general statistics
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. Worth noting that these changes coinside with railgun nerfs, however.*

* **Hitpoints:** `12500 => 11000`
* **Armor:** ``40 => 35`

## Gaalsien carrier point defense weapons
> *Lower level PD performance increased, but higher level rate of fire reduced (due to damage rework of carrier PD weapons)*

* **Rate of fire:** `10 => 9`
* **Weapon Systems power shunt PD rate of fire:**
    * **Level 1:** `'set to 17' => 'increase by 25%'`
    * **Level 2:** `'set to 24' => 'increase by 50%'`
    * **Level 3:** `'set to 31' => 'increase by 75%'`
    * **Level 4:** `'set to 38' => 'increase by 125%'`
    * **Level 5:** `Bonus removed (30 => 10)`

## Gaalsien carrier speed
> *Slight reduction in power of this power system. Chasing down a lategame gaalsien carrier was previously extremely difficult.*

* **Base:** `10 => 15`
* **Speed systems power shunt:**
    * **Level 3:** `75 => 70`
    * **Level 4:** `95 => 85`
    * **Level 5:** `120 => 105`

## Hyper-sonic missile barrage
> *Nuke-style abilities have the potential to wipe big parts of enemy army without much chance for retaliation, only preemptive preparation is effective. A bigger window is required after their use so that players can have an engagement which will not involve another one. Hyper-sonic missile barrage is also one of the most inconsistent abilities, while also being extremely damaging when hitting larger targets. Damage reduced and increased area of effect should make the ability feel more consistent.*

* **Cooldown:** `90s => 120s`
* **Damage:** `600 => 400`
* **Damage against carriers:** `50% => 100%`
* **AOE:** `200 => 230`
* **Missile count per weapon:** `10 => 8`

## Khaaneph carrier general statistics
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. Worth noting that these changes coinside with railgun nerfs, however. Khaaneph armor was abnormally low compared to other carrier which, combined with its slow speed, was a bit too punishable in some situations.*

* **Hitpoints:** `12500 => 11500`
* **Armor:** `20 => 30`

## Khaaneph carrier cruise missiles
> *Khaaneph cruise missiles have proven themselves to be extremely powerful overal and especially against enemy carriers.*

* **Damage against carriers:** `150% => 100%`
* **Affected by high ground:** `Yes => No`

## Khaaneph carrier weapon systems
> *Khaaneph carrier does not have range systems on it, meaning the range of its basic weaponry can never be increased. This meant that weapons systems power shunt was mostly useless as it could never get range on the opponent. Increasing base range of carrier weapons can be dangerous for early game therefore khaan carrier is receiving some nerfs to its basic weapons for low levels. High power level PDs receive the highest available rate of fire compared to other carriers, however, to make this system more desirable.*

* **PD rate of fire:** `8 => 6`
* **PD ranges:** `250/500/750 => 350/650/950`
* **Missile systems range:** `750 => 950`
* **Power shunt now provides extra fire rate to missile systems**
* **Rate of fire bonuses:**
    * **Level 1:** `'set to 17' => 'increase by 50%'`
    * **Level 2:** `'set to 24' => 'increase by 100%'`
    * **Level 3:** `'set to 31' => 'increase by 200%'`
    * **Level 4:** `'set to 38' => 'increase by 300%'`
    * **Level 5:** `'set to 38' => 'increase by 50%'`
* **Fixed a bug where level 5 weapon system power shunt would decrease the range of one of the PD weapons**

## Khaaneph carrier speed suppor aura power shunt
> *The diameter of level 5 speed boost was larger than the range of a railgun. In team games this would allow for somewhat oppressive speed boost blobbing strategies which should now be slightly more difficult to execute correctly.*

* **Aura area of effect:**
    * **Level 1:** `600 => 420`
    * **Level 2:** `600 => 420`
    * **Level 3:** `800 => 560`
    * **Level 4:** `800 => 560`
    * **Level 5:** `1200 => 840`

## Gaalsien baserunner heal aura ability
> *It is no longer possible to abuse baserunner spam to quickly heal large amounts of hitpoints on targets such as the carrier, as the heal doesn't stack nearly as strongly as it used to. Overall effectiveness of this ability is increased immensely, however, heal amount per burst increased from 40 to 100, total heal amount increased from 400 to 1000*
* **Recharge time:** `50s => 80s`
* **Rate of healing:** `1 => 10`
* **Amount:** `40 => 5`
* **Burst:** `1s => 0.4s`
* **Cooldown:** `0 => 0.6s`
* **Now applies a non-stacking healing over time status effect to friendly units:**
    * **Rate of healing:** `20`
    * **Duration:** `0.1s`
    * **Healing:** `10`
* **Prevented from affecting air units**

## Gaalsien baserunner sensor ability
> *Slight ease of use improvement for this ability as it is considerably weaker than the combination of Khaaneph baserunner abilities*

* **Deployment range:** `2350 => 2600`

## Blast drone
> *A 1PC skimmer together with blast drones rush was nearly impossible to stop even with perfect response and good micro. Additionally, late game BD use was limited and expensive. The new BD iteration should hopefully provide extra motivation for getting them later in the game while fixing the issues with early game rushes.*

* **Cost:** `150CU => 100CU`
* **Hitpoints:** `500 => 400`
* **Construction time:** `20s => 40s`
* **Population:** `0 => 1`
* **Falloff:** `None => Quadratic`
* **AOE:** `200 => 260`
* **Damage:** `650 => 680`
* **Damage packets:** `10 => 20`

## Sandskimmer
> *Discrepancy between LAV and Skimmer hitpoints was very large and caused almost every area of effect weapon to be extremely difficult to balance. Skimmers also needed a slight decrease in power.*

* **Hitpoints:** `650 => 620`
* **Armor:** `0 => 1`

## Sandskimmer weapon
> *It is generally easier to counter strike craft in the mod, the extra dps was introduced in order to bring back the rock-paper-scissors mechanic, meaning strike craft will be capable of countering enemy railguns.*

* **Reload:** `0.1s => 0.5s`
* **Cooldown:** `0.398s => 0.22s`
* **Max burst:** `1s => 0.9s`

## Sandskimmer upgrades
> *These changes are part of the effort of reducing supply blocking due to upgrades for gaalsien.*

* **Raiding upgrade research time:** `50s => 40s`
* **Damage 2 upgrade research time:** `60s => 45s`

## Production cruiser
> *Strategies of quickly transitioning from heavy aggression to 3 base economy are extremely strong and need to be tuned down. This doesn't affect conventional fast expand strategies very much, early game units are getting tuned around this change. RU cost on production cruisers is there to slow down tech progression when expanding. Currently, there's almost no downside and slow down when expanding from 2 base to 3 base, this should make tech progression just slightly slower which could prove meaningful vs aggressive enemy strategies.*

* **Refinery tech cost:** `700CU => 600CU 40RU`
* **Cost:** `600CU => 640CU 60RU`

## Production cruiser anti-air weapon:
> *DPS was rebalanced slightly to be lower on short and medium range but stronger on long range, an additional slight range increase is introduced in order to help mitigate early game air plays. This should ensure that air is a bit harder to control and will most likely be bleeding hitpoints when attempting to operate close to production cruisers.*

* **Rate of fire:** `15 => 10`
* **Range:** `1100 => 1180`
* **Accuracy:**
    * **Short:** `55% => 70%`
    * **Medium:** `40% => 60%`
    * **Long:** `25% => 45%`
* **Hidden accuracy modifiers against probes removed**
* **Damage against probes:** `100% => 50%`

## Assault ship
> *Slightly reducing tech cost to make it this tech path more desirable in more situations. Range increase should help with unit usability issues as well as improve overall effectiveness, particularly against units it's intended to counter. The unit is extremely strong when it can get into position to fire, so, to reduce the impact of assault ship rushes and assault ship early game dominance, hitpoints of the assault ship are getting reduced. To mitigate midgame assault ship spam and all-in aggro strategies, their cost is getting increased. Additionally, now that assault ships have good range to do consistent damage to strike craft, their large area of effect is no longer required for them to be effective at countering them. Extra damage on the main gun makes assault ships extremely deadly against enemy workers with aoe, as well as more potent at countering enemy armor.*

* **Tech cost:** `600CU 100RU => 500CU 100RU`
* **Cost:** `220CU 40RU => 260CU 40RU`
* **Hitpoints:** `1400 => 960`
* **Armor:** `6 => 7`
* **Damage:** `24 => 29`
* **AOE:** `80 => 70`
* **Range:** `700 => 745`

## Assault ship armor upgrade cost
> *Ship armor upgrades are the least used upgrades and the least useful ones. Decreasing cost and time to purchase these upgrades to make them more desirable.*

* **Level 1:** `200CU 100RU 15s => 150CU 100RU 15s`
* **Level 2:** `200CU 200RU 20s => 200CU 150RU 20s`
* **Level 3:** `200CU 300RU 30s => 250CU 200RU 25s`

## Assault railgun
> *Assault railguns are pretty difficult to deal with on some maps and reaching critical mass of them is rather easy. A slight rebalance to their survivability and cost to better place the unit in terms of how it lines up with things it's supposed to counter, and its counters. Maneuverability changes should allow strike craft and other units which normally have a hard time catching them to be more capable of doing it and promotes the use of dart maneuver ability. Damage is reduced with other midgame unit balancing in mind, AR were a bit too good at countering a lot of them. Wind-up and reload time rebalanced to make AR weapon more responsive when AR are being flanked.*

* **Cost:** `200CU 35RU => 220CU 50RU`
* **Production time:** `24s => 20s`
* **Hitpoints:** `550 => 660`
* **Experience value:** `610 => 350`
* **Armor upgrade hitpoint bonus:**
    * **Level 2:** `100 => 50`
    * **Level 3:** `200 => 100`
* **Movement dynamics characteristics:**
    * **Acceleration time:** `0.85 => 0.93`
    * **Breaking time:** `0.85 => 0.93`
    * **Max speed:** `100 => 92`
* **Damage:** `50 => 45`
* **Wind-up:** `1s => 0.6s`
* **Wind-down:** `0.5s => 0.25s`
* **Reload:** `0.6s => 1.0s`
* **Dart maneuver:**
    * **Tech time:** `60s => 30s`
    * **Tech cost:** `100CU 100RU => 100CU 70RU`

## Heavy railgun
> *Railguns have seen a large redesign in the mod, where their damage per shot has been reduced, cost increased, but hitpoints also increased. Railgun battles now resolve themselves slower, and high ground advantage plays a much larger role. All railgun and carrier ranges are reduced in the mod as part of the effort to reduce the prevalence of railgun-based strategies. Gaalsien railgun range is slightly lower than coalition as a quality of life change where coalition railguns have had a harder time chasing the enemy due to having to stop when given new attack orders (ctrl-boxing enemy rails for instance). Additionally, the range difference will help out against Gaalsien early game 1PC railgun timings.*

* **Cost:** `280CU 90RU => 320CU 100RU`
* **Damage:** `225 => 195`
* **Hitpoints:** `670 => 750`
* **Max speed:** `62 => 57`
* **Experience value:** `450 => 550`
* **Range:** `2100 => 1860`

## Railgun EMP rounds upgrade:
> *This upgrade has seen very little use throughout the game's history. Giving slight buffs and large research time reductions to make it more desirable.*

* **Cost:** `250CU 150RU => 200CU 100RU`
* **Research time:** `45s => 30s`

## Railgun ranged calibration upgrade:
> *This upgrade has seen very little use throughout the game's history. Giving slight buffs and large research time reductions to make it more desirable.*

* **Cost:** `250CU 150RU => 150CU 150RU`
* **Research time:** `60s => 45s`

## Railgun armor level 3 upgrade cost
> *It was previously too much of an obvious choice to always upgrade level 3 on railguns which massively increased their combat performance without much of an initial investment. It should be slightly less of an obvious choice and supporting railgun units with other units rather than just beefing up railguns themselves should be slightly more desirable.*

* **Cost :** `200CU 300RU => 200CU 400RU`

## Interceptor
> *Cost changes are part of the effort to reduce the strength of assault ship rush follow-ups, but also this will help interceptor sustain and prevent them:** `bogging down the carrier production line as heavily.*
* **Tech cost:** `250CU 250RU => 550CU 250RU`
* **Tech research time:** `55s => 70s`
* **Cost:** `250CU 120 RU => 250CU 100RU`
* **Build time:** `15s => 12s`
* **Armor:** `1 => 2`
* **Hangar size:** `15 => 12`

## Interceptor weapon
> *Interceptor reload time was abnormally short (compared to 8s reload time of strike fighters), often allowing it to fire off the start of a second volley within a single pass over its target. This also made interceptors incredibly strong in dogfights and when they would circle very large targets (carriers), or when chasing the enemy. Overall rocket count per plane isn't changed, but 4 rockets are shot per burst instead of 3, decreasing the total number of bursts from 4 to 3. These changes will decrease the overall damage payload of interceptors per sortie. It will also decrease the RNG nature of interceptors fighting ground targets as more rockets will land resulting in more fair spread of damage to the intended targets. Damage per burst is going down from 450 to 440 (intent is to not change this very much), damage per sortie is going down from 1800 to 1320. Additionally, this set of changes will help mitigate the carrier sniping strategies utilized in team games.*

* **Reload:** `2s => 4s`
* **Weapon base damage:** `150 => 110`
* **Weapon rate of fire:** `3 => 4`

## Interceptor afterburner upgrade:
> *Afterburner upgrade is incredibly effective and can be oppressive in situations where a player can get it while being ahead in the game. Toned down its effects and increased the cost to make this upgrade more of a commitment.*

* **Cost:** `350CU 90RU => 200CU 120RU`
* **Research time:** `60s => 40s`
* **Max speed bonus:** `60% => 40%`
* **Turn radius reduction:** `60% => 40%`

## Siege cruiser range upgrade
> *This is the longest research in the game, abnormally so.*

* **Research time:** `135s => 110s`

## Gaalsien siege cruiser
> *Getting to artillery should now be much faster and easier. This is designed this way to allow for players to play against enemy railguns without the need of using own railguns, albeit in a still risky way, especially against midgame railgun pushes. Due to hitpoint changes, artillery battles will get resolved faster , this makes countering artillery with own artillery less desirable as it's more risky. Additionally, sniping artillery cruisers was too difficult overall.*

* **Tech research cost:** `600CU 450RU => 450CU 350RU`
* **Tech research time:** `90s => 65s`
* **Cost:** `600CU 200RU => 400CU 160RU`
* **Production time:** `60s => 50s`
* **Population:** `3 => 4`
* **Hitpoints:** `2500 => 2100`
* **Armor:** `3 => 5`
* **Barrage range:** `2000 => 2250`

## Gaalsien siege cruiser autofire
> *Autofire is an extremely unsatisfying mechanic, exceptionally annoying to deal with for an opposing player while requiring little-to-no effort on the part of artillery cruiser users to be effective. It'll remain useful for forcing enemy to constantly micro their units and force the opponent to displace if they are in range, but will ultimately be less punishing and easier to deal with.*

* **Autofire damage:** `200 to 140

## Khaaneph siege cruiser
> *Khaaneph siege cruiser is very strong and becomes problematic when spammed in team games, besides being very strong on maps with certain topology which allows siege cruisers to constrict players completely in their base. These changes should increase the critical mass required for siege cruisers to be able to counter its counters such as railguns, and reduce the potential of providing free damage on the enemy while keeping the barrage feeling powerful. Getting hit by KSC main weapon should be slightly less punishing overall, and microing against it is easier. However, the damage is applied over a considerably larger area, making it more consistent for the situations where units are trying to dodge it. Additionally, this cruiser was impossible to weed out from behind dunes. Armor reduction means that this cruiser can get swarmed even by lower damage weapon using units.*

* **Hitpoints:** `3350 to 3050`
* **Armor:** `15 to 13`
* **Main weapon:**
    * **Damage:** `125 => 150`
    * **AOE:** `150 => 210`
    * **Number of bursts:** `3 => 2`
    * **Falloff:** `Linear => Quadratic`
* **Barrage:**
    * **Damage:** `125 to 260`
    * **Damage packets:** `1 to 2`
    * **Falloff:** `None => Quadratic`
    * **AOE:** `150 => 240`
    * **Damage against small targets:** `100% => 65%`
    * **Damage against carriers:** `100% => 80%`
    * **Number of bursts:** `8 => 4`
    * **Cooldown:** `0.8s => 2.5s`
    * **Recharge:** `50s => 65s`

## Honourguard cruiser
> *It should now be easier to field honourguard cruisers and overall weapon performance is more more consistent. A rebalance to unit's hitpoint pool was required to curb the overall tankiness and make it slightly easier to counter. Honourguard cruisers had the potential to one-shot enemy strike craft force from long range when firing at them from high ground, which could often end the game very quickly. The damage that the weapon had also made its overall dps extremely low, meaning it was very bad at countering anything which had a meaningful hitpoint pool. The weapon should now perform much more consistently and feel powerful even against bulkier targets.*

* **Tech time:** `75s => 65s`
* **Cost:** `700CU 240RU => 550CU 270RU`
* **Production time:** `70s => 55s`
* **Hitpoints:** `3600 => 2700`
* **Max speed:** `60 => 54`
* **Main weapon:**
    * **AOE:** `200 => 220`
    * **Damage:** `400 => 550`
    * **Reload:** `5s => 4.5s`
    * **Falloff:** `None => Linear`
    * **Wind-down:** `0.5s => 0.25s`

## Honourguard cruiser anti-air
> *Honourguard cruiser anti-air is relatively weak and paying such a large sum for it is almost never worth it. The long wind-up also often meant that the target would fly out of range before the weapon could fire.*

* **Research time:** `75s => 45s`
* **Research cost:** `600CU 370RU => 300CU 200RU`
* **Wind-up:** `3s => 1.5s`
* **Reload:** `0 => 3s`

## Precision bomber
> *Improved accessibility of tech and the unit itself should make this tech path much more desirable. Precision bomber has incredible maneuverability parameters, curbing those to make the unit harder to control and slower to deliver follow-up bombs on target. The damage characteristics have been updated to make the bomber worse at destroying enemy AA vehicles but still potent at dealing with enemy cruisers. Area of effect improved, but modifier against small targets added to prevent the bombers from becoming too strong against strike craft and salvagers.*

* **Research cost:** `400CU 275RU => 300CU 175RU`
* **Research time:** `65s => 45s`
* **Cost:** `300CU 220RU => 300CU 140RU`
* **Production time:** `32s => 22s`
* **Population:** `2 => 3`
* **Hitpoints:** `1250 => 1050`
* **Max speed:** `550 => 450`
* **Turn radius:** `225 => 300`
* **Damage:** `1000 to 800`
* **Reload:** `1.5s => 3.5s`
* **Damage against small targets:** `100% => 60%`
* **AOE:** `60 => 140`
* **Falloff:** `None => Quadratic`

## Precision bomber upgrades
> *Extremely expensive to fully upgrade gaalsien bombers, making these upgrades very undesirable unless all-inning. Bomber usability falls off as counters get added to the battlefield, investing into both bomber count and their upgrades normally is a very bad idea, these changes along with other air and anti-air rebalances should help with these upgrades become more desirable.*

* **Rearm upgrade:**
    * **Cost:** `350CU 70RU => 200CU 70RU`
    * **Research time:** `40s => 20s`
* **Payload upgrade cost:** `500CU 200RU => 400CU 200RU`

## Missile ship
> *Gaalsien AA tanks take significantly lower to tech into and produce, a small production time buff should help gaalsien prepare for enemy air plays more easily. The largest factor of AA doing its work vs normal air strategies is the first shot. Increased reload duration means AA will have a much harder time quickly killing off large numbers of air and heavy air and both of those strategies are underused, however it won't affect the early game air rush situations very much.*

* **Cost:** `400CU 80RU => 350CU 90RU`
* **Armor:** `5 => 3`
* **Production time:** `28s => 24s`
* **Reload:** `1s => 2.5s`
* **Range:** `1400 => 1330`
* **Fixed an issue where veterancy 4 rate of fire increase did nothing for the unit, it now grants a 1s reduction to reload time**

## Missile ship radar guided missiles upgrade
> *Range upgrade pretty much has never seen use in competitive play. Gaalsien AA range is strong enough to cover most of what it needs to cover and the fact that it can regenerate hitpoints generally allows it to position itself more aggressively than the coalition AA tank counterpart. With base range being reduced, radar guided missile upgrade should become more of an important upgrade when facing more committed enemy air play.*

* **Radar upgrade range:** `1600 => 1500`
* **Research time:** `30s => 20s`
* **Fixed an issue where radar upgrade was reducing turret rotation speed rather than increasing it:**
    * **Turret field of fire:** `120 => 40`
    * **Base turret rotation speed:** `240 => 160`
    * **Upgraded turret rotation speed:** `180 => 240`

## Missile ship direct missile barrage
> *Direct missile barrage is now much better at hitting enemy strike craft and also more potent at dealing good damage to medium vehicles. The recharge upgrade was considerably underutilized and for good reason. Reducing cost and time to purchase the upgrade, making it less of a commitment and more of a quality of life upgrade to occasionally get in case there are already multiple MS out on the field.

* **Weapon:**
    * **Recharge:** `60s => 90s`
    * **Damage:** `150 => 170`
    * **AOE:** `80 => 150`
    * **Falloff:** `None => Linear`
    * **Benefits from high ground:** `Yes => No`
* **Recharge upgrade cost and research time:** `300CU 85RU 30s => 220CU 60RU 15s`
