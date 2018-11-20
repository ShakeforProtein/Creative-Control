# Creative Control
Take Control of Creative mode.


Allows players with the required permissions to add blocks to, remove blocks from, or ignore, a banned block list. This was written because of an issue with Tridents being able to crash spigot servers that had not at the time of writing been dealt with.

This plugin works on a per world basis and items need to be added or removed on each world. In the future there will be an option to ban on all worlds.

Items are destroyed in four circumstances. When an inventory is closed, when the hotbar slot changes, when the item is dropped and when a player animation event triggers, eg moving or using.

#Commands
ccBlock
ccUnblock
ccShowBlocked

#Permissions
creativecancel.cancel   -   Players with this permission can add and remove items from the blocked item list.
creativecancel.bypass   -   Players with this permission will not be effected by creative cancel.
creativecancel.show     -   Players with this permission can see what items have been blocked.



#Default config (this will be installed automatically when the plugin is first loaded)

BlockedItems:
  Example_World:
    TRIDENT: TRIDENT

ConsoleNotify: true

messages:
  prefix: '[CreativeCancel] - '
  showBlocked: 'The following items have are currently blocked on this world.'
  itemBlocked: 'You have blocked XXXITEMXXX on this world.'
  itemUnblocked: 'You have unblocked XXXITEMXXX  on this world.'
  noCommandPerm: 'Im sorry XXXPLAYERXXX, but you lack sufficient privileges to use Creative Cancel.'
  animate: 'Im sorry XXXPLAYERXXX, but we have elected to disallow the use of XXXITEMXXX on this world'
  changedHotbar: 'Im sorry XXXPLAYERXXX, but we have elected to disallow the use of XXXITEMXXX on this world'
  itemDropped: 'Im sorry XXXPLAYERXXX, but we have elected to disallow the use of XXXITEMXXX on this world'
  closeInventory: 'Im sorry XXXPLAYERXXX, but we have elected to disallow the use of XXXITEMXXX on this world'
