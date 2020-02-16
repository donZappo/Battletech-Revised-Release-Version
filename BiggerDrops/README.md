# BiggerDrops
<pre>
Settings 
{
  "debugLog": true, - debug log, log is small most time at contract init, no performance impact, assumed to be true by default
  "additionalLanceName": "EXTRA LANCE", - name of additional lance at drop UI, for localization compatibility in future 
  "additinalMechSlots": 4, - number of additional mech slots, if grater than 4 assumed to be 4
  "additinalPlayerMechSlots": 4, - number of additional slots for direct player control, can't be grater than additinalMechSlots.
                              Example: additinalMechSlots = 3, additinalPlayerMechSlots = 1. You will get 3 available slots at drop UI. 
                              At battle start you will be able to control 5 meches (4+1) directly (5 portraits) and additional employer's lance friendly AI controlled with 2 meches.
  "defaultMaxTonnage": 800, - max tonnage by default, if contract not overriding it.
  "allowUpgrades" : true, - when true, turns additinalMechSlots, additinalPlayerMechSlots & defaultMaxTonnage into default values and allows argo upgrades or events to modify these values by accessing 
							BiggerDrops_AdditionalMechSlots, BiggerDrops_AdditionalPlayerMechSlots or BiggerDrops_MaxTonnage stats in the simGame's statcollection
  "showAdditionalArgoUpgrades" : true, - when true modify the argo upgrade screen to show an additional row of upgrades.
										 Note: because the upgrade category is currently controlled by an enum, existing values of POWER_SYSTEM, STRUCTURE & DRIVE_SYSTEM are reused for the 1st, second and 3rd categories within the new row.
										 to add items to these categories, the upgrade location must be set to UNKNOWN.
  "argoUpgradeName" : "Command & Control", sets the name of the new row of upgrades on the argo upgrade screen if enabled
  "argoUpgradeCategory1Name" : "Drop Size", sets the name of the first new upgrade category on upgrades on the argo upgrade screen if enabled
  "argoUpgradeCategory2Name" : "Mech Control", sets the name of the second new upgrade category on upgrades on the argo upgrade screen if enabled
  "argoUpgradeCategory3Name" : "Drop Tonnage" sets the name of the third new upgrade category on upgrades on the argo upgrade screen if enabled
}
</pre>