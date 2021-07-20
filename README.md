# **MATH**

## Vector3

Properties:  

- ```number``` x
- ```number``` y
- ```number``` z
- ```number``` X
- ```number``` Y
- ```number``` Z
- ```boolean``` isWall
- ```boolean``` isBush
- ```boolean``` isInFOW
- ```boolean``` valid
- ```number``` perpendicular
- ```number``` perpendicular2
- ```number``` height
- ```Vector3``` normalized

> Vector3(number, number, number)

```lua
local vec = Vector3(0, 0, 0)
vec:print()
```

> v1:__tostring()

```lua
local a = player.position
print(a:__tostring())
```

> v1:distance(v2)

**Parameters**  
```Vector3``` v2  
**Return Value**  
```number```  

```lua
local distance = player.position:distance(Vector3(0,0,0))
print(distance)
```

> v1:shorten(v2, distance)

**Parameters**  
```Vector3``` v2  
```number```  distance  
**Return Value**  
```void```  

```
modifies vector
```

> v1:shortended(v2, distance)

**Parameters**  
```Vector3``` v2  
```number```  distance  
**Return Value**  
```Vector3```  shortened vector

```
returns new shortened vector
```

> v1:extend(v2, distance)

**Parameters**  
```Vector3``` v2  
```number```  distance  
**Return Value**  
```void```  

```
modifies vector
```

> v1:extended(v2, distance)

**Parameters**  
```Vector3``` v2  
```number```  distance  
**Return Value**  
```Vector3```  extended vector

```
returns new extended vector
```

> v1:lerp(v2, delta)

**Parameters**  
```Vector3``` v2  
```number```  delta  
**Return Value**  
```Vector3```  lerped vector

## Vector2

Properties:  

- ```number``` x
- ```number``` y
- ```number``` X
- ```number``` Y

> Vector2(number, number)

```lua
local a = Vector2(0, 0)
```

> v1:__tostring()

```lua
local a = Vector2(0, 0)
print(a:__tostring())
```

# **LIBRARIES**

## game

## camera

> camera.zoom

Return Value  
```number``` returns the current zoom value  

> camera.setPosition(position)

Parameters  
```Vector3``` position to set camera to

> camera.setZoom(value)

Parameters  
```number``` zoom value

## network

> network.latency

> network.ping

Return Value  
```number``` latency to the game server in milliseconds

## ts

## healthPrediction

## system

## chat

> chat.printChat(msg)

Parameter  
```string``` msg  
sends message locally  

> chat.sendChat(msg)

Parameter  
```string``` msg  
sends message in chat  

## keyboard

## damage

## orb

## evade

## renderer

## networking

> networking.downloadFile(url, path)

Return Value  
```boolean``` success

> networking.post(url, body, header)

Return Value
```Response.obj```

> networking.get(url)

Return Value
```Response.obj```

# **OBJECTS**

## gameObject.obj

Properties:  

- ```Vector3``` gameObject.position
- ```Vector3``` gameObject.pos
- ```number```  gameObject.id
- ```number```  gameObject.team
- ```number```  gameObject.networkId
- ```number```  gameObject.boundingRadius
- ```string```  gameObject.name
- ```number```  gameObject.resource
- ```number```  gameObject.maxResource
- ```number```  gameObject.mana
- ```number```  gameObject.maxMana
- ```number```  gameObject.secondaryResource
- ```number```  gameObject.maxSecondaryResource
- ```number```  gameObject.sar
- ```number```  gameObject.maxSar
- ```boolean``` gameObject.isTargetable
- ```number```  gameObject.health
- ```number```  gameObject.maxHealth
- ```number```  gameObject.healthPercent
- ```number```  gameObject.manaPercent
- ```number```  gameObject.allShield
- ```number```  gameObject.physicalShield
- ```number```  gameObject.magicalShield
- ```boolean``` gameObject.isEnemy
- ```boolean``` gameObject.isAlly
- ```boolean``` gameObject.isNeutral
- ```boolean``` gameObject.isHero
- ```boolean``` gameObject.isMonster
- ```boolean``` gameObject.isMinion
- ```boolean``` gameObject.isInhib
- ```boolean``` gameObject.isNexus
- ```boolean``` gameObject.isTurret
- ```boolean``` gameObject.isMissile
- ```boolean``` gameObject.isMelee
- ```boolean``` gameObject.isRanged
- ```boolean``` gameObject.isStructure
- ```boolean``` gameObject.isLaneMinion
- ```boolean``` gameObject.isSiegeMinion
- ```boolean``` gameObject.isPet
- ```boolean``` gameObject.isWard
- ```boolean``` gameObject.isPlant
- ```boolean``` gameObject.isLargeMonster
- ```boolean``` gameObject.isEpicMonster
- ```boolean``` gameObject.isBlueRed
- ```boolean``` gameObject.isDead
- ```boolean``` gameObject.isVisible
- ```number```  gameObject.attackRange
- ```number```  gameObject.totalBonusAttackDamage
- ```number```  gameObject.totalAbilityPower
- ```number```  gameObject.totalAttackDamage
- ```number```  gameObject.totalBonusAbilityPower
- ```number```  gameObject.flatMagicDamageMod
- ```number```  gameObject.hash
- ```boolean``` gameObject.isAsleep
- ```boolean``` gameObject.isInvulnerable
- ```number```  gameObject.magicResist
- ```number```  gameObject.attackSpeedMod
- ```number```  gameObject.armor
- ```number```  gameObject.flatMagicPenetration
- ```number```  gameObject.percentMagicPenetration
- ```number```  gameObject.physicalLethality
- ```number```  gameObject.flatArmorPenetration
- ```number```  gameObject.percentArmorPenetration
- ```number```  gameObject.healthRegen
- ```number```  gameObject.percentLifeStealMod
- ```number```  gameObject.gold
- ```number```  gameObject.totalGold
- ```number```  gameObject.shutdownValue
- ```number```  gameObject.percentCooldownMod
- ```boolean``` gameObject.isOnScreen
- ```Vector3``` gameObject.direction
- ```string```  gameObject.charName
- ```string```  gameObject.skinName
- ```number```  gameObject.level
- ```number```  gameObject.buffCount
- ```boolean``` gameObject.isMe
- ```number```  gameObject.attackCastDelay
- ```number```  gameObject.attackDelay
- ```boolean``` gameObject.isMoving
- ```boolean``` gameObject.isCastingSpell
- ```boolean``` gameObject.canAttack
- ```number```  gameObject.totalHealth
- ```number```  gameObject.totalMaxHealth
- ```number```  gameObject.moveSpeed
- ```Vector2``` gameObject.barPos
- ```table```   gameObject.getWayPoints
- ```table```   gameObject.path
- ```number```  gameObject.pathCount
- ```number```  gameObject.pathIndex
- ```number```  gameObject.distance
- ```boolean``` gameObject.isDashing
- ```number```  gameObject.dashSpeed
- ```number```  gameObject.crit
- ```boolean``` gameObject.isRecalling
- ```boolean``` gameObject.isTeleporting
- ```boolean``` gameObject.willReviveOnDeath
- ```gameObject.obj``` gameObject.owner
- ```boolean``` gameObject.canMove
- ```Vector3``` gameObject.pathEndposition
- ```Vector3``` gameObject.nextPathposition
- ```heroStats.obj``` gameObject.stats
- ```number``` gameObject.actionState
- ```spellCastInfo.obj``` gameobject.activeSpell
- ```spellCastInfo.obj``` gameobject.basicAttack

**localplayer only function**  

> player:castSpell(slot)

**Parameters**  
```number``` slot  
**Return Value**  
```bool``` success  

```lua
-- example: Garen Q
player:castSpell(SpellSlot.Q)
```

> player:castSpell(slot, pos)

**Parameters**  
```number``` slot  
```Vector3``` pos  
**Return Value**  
```bool``` success  

```lua
-- example: Ezreal Q
player:castSpell(SpellSlot.Q, game.mousePos)
```

> player:castSpell(slot, obj)

**Parameters**  
```number``` slot  
```gameObject.obj``` obj  
**Return Value**  
```bool``` success  

```lua
-- example: Vayne E
player:castSpell(SpellSlot.E, orb.selectedTarget)
```

> player:castSpell(slot, startPos, endPos)

**Parameters**  
```number``` slot  
```Vector3``` startPos  
```Vector3``` endPos  
**Return Value**  
```bool``` success  

```lua
-- example: Viktor E
player:castSpell(SpellSlot.E, player.position, game.mousePos)
```

> player:castSpellFast(slot)

**Parameters**  
```number``` slot  
**Return Value**  
```bool``` success  

```
castSpellFast variants are the same as castSpell but ignore rate limiting
```

> player:castSpellFast(slot, pos)

**Parameters**  
```number``` slot  
```Vector3``` pos  
**Return Value**  
```bool``` success  

> player:castSpellFast(slot, obj)

**Parameters**  
```number``` slot  
```gameObject.obj``` obj  
**Return Value**  
```bool``` success  

> player:castSpell(slot, startPos, endPos)

**Parameters**  
```number``` slot  
```Vector3``` startPos  
```Vector3``` endPos  
**Return Value**  
```bool``` success  

> player:levelSpell(slot)

**Parameters**  
```number``` slot  
**Return Value**  
```void```  

> player:move(pos)

**Parameters**  
```Vector3``` pos  
**Return Value**  
```void```  

> player:attack(obj)

**Parameters**  
```gameObject.obj``` obj  
**Return Value**  
```void``` 

> player:issueOrder(order, obj)

**Parameters**  
```number``` order  
```gameObject.obj``` obj  
**Return Value**  
```void``` 

> player:issueOrder(order, pos)

**Parameters**  
```number``` order  
```Vector3``` pos  
**Return Value**  
```void``` 

> player:issueOrder(order, pos, drawClick, triggerEvent)

**Parameters**  
```number``` order  
```gameObject.obj``` obj  
```boolean``` drawClick  
```boolean``` triggerEvent  
**Return Value**  
```void``` 

```lua
--if drawclick is true the indicator will be drawn
--if triggerEvent is false the order wont trigger the OnIssueOrder Event
player:issueOrder(gameObjectOrder.moveTo, game.mousePos, true, false) 
-- ^ draw indicator, dont trigger event
```

> player:issueOrderFast(obj)

```
same as issueOrder but ignores ratelimit and implicitly generates order
```

**Parameters**  
```gameObject.obj``` obj  
**Return Value**  
```void``` 

> player:issueOrderFast(pos)

**Parameters**  
```Vector3``` pos  
**Return Value**  
```void``` 

> player:issueOrderFast(order, pos, drawClick, triggerEvent)

**Parameters**  
```number``` order  
```gameObject.obj``` obj  
```boolean``` drawClick  
```boolean``` triggerEvent  
**Return Value**  
```void``` 

> player:updateChargeableSpell(slot, pos)

**Parameters**  
```number``` slot  
```Vector3``` pos  
**Return Value**  
```void```  

```lua
--example: Xerath Q
player:updateChargeableSpell(SpellSlot.Q, game.mousePos)
```

> player:updateChargeableSpellFast(slot, pos)

**Parameters**  
```number``` slot  
```Vector3``` pos  
**Return Value**  
```void```  

> player:setSkin(skinID)

**Parameters**  
```number``` skinID  
**Return Value**  
```void```  

```lua
-- example: Ezreal Q
player:castSpell(SpellSlot.Q, game.mousePos)
```

**all gameobject functions**  

> gameObject:hasBuffOfType(type)

**Parameters**  
```number``` type  
**Return Value**  
```bool```  hasBuff

```lua
if player:hasBuffOfType(5) then
    print("player is stunned")
end
```

> gameObject:getBuffByIndex(index)

**Parameters**  
```number``` index  
**Return Value**  
```buffInstance.obj```  

```lua
for i = 0,player.buffCount - 1 do
    local buff = player:getBuffByIndex(i)
    if buff and buff.valid then
        print(buff.name)
    end
end
```

> gameObject:findBuff(name)

**Parameters**  
```string``` name  
**Return Value**  
```buffInstance.obj```  

> gameObject:findBuff(hash)

**Parameters**  
```number``` hash  
**Return Value**  
```buffInstance.obj```  

> gameObject:spellState(slot)

**Parameters**  
```number``` slot  
**Return Value**  
```number``` SpellState  

> gameObject:isValidTarget(range, onlyEnemy, from)

**Parameters**  
```number``` range  
```boolean``` onlyEnemy  
```Vector3``` from  
**Return Value**  
```boolean```  

> gameObject:getSpell(slot)

**Parameters**  
```number``` slot  
**Return Value**  
```spellDataInst.obj``` spell  

> gameObject:getAutoAttackRange(target)  

**Parameters**  
```gameobject.obj``` target  
**Return Value**  
```float```  

```lua
--adjusts range according to target, eg. cait debuff
local a = player:getAutoAttackRange(orb.selectedTarget)

--player bounding + player range
local a = player:getAutoAttackRange(nil)
```

> gameObject:isInAutoAttackRange(target)  

**Parameters**  
```gameobject.obj``` target  
**Return Value**  
```bool```  

> gameObject:drawDamage(damage, color)  

**Parameters**  
```number``` damage  
```number``` color  
**Return Value**  
```void```  

```lua
--draw damage on healthbar
player:drawDamage(200, Color(255,255,255,255))
```

> gameObject:findItemSlot(itemID)

**Parameters**  
```number``` itemID  
**Return Value**  
```number```  spellSlot  

> gameObject:isFacing()

**Return Value**
```boolean```

```lua
if orb.selectedTarget:isFacing() then
    print("target faces player")
else
    print("target does not face player")
end
```

> gameObject:getAutoAttackDamage(target)  

**Parameters**  
```gameobject.obj``` target  
**Return Value**  
```float```  

> gameObject:willReviveOnDeathByTime(time)  

**Parameters**  
```number``` time    
**Return Value**  
```bool```  

```
time in seconds
```

> gameObject:getItemIdFromSlot(slot)

**Parameters**  
```number``` slot  
**Return Value**  
```number```  itemID  

> gameObject:createPath(position, smoothed)

**Parameters**  
```Vector3``` position  
```bool``` smoothed  
**Return Value**  
```table```  path  

## HeroStats.obj

Properties:  

- ```number```  HeroStats.minionsKilled
- ```number```  HeroStats.kills
- ```number```  HeroStats.deaths
- ```number```  HeroStats.assists

## missileClient.obj

Inherits gameObject.obj  
  
Properties:  

- ```number``` missileClient.sourceIndex
- ```Vector3``` missileClient.startPos
- ```Vector3``` missileClient.endPos
- ```number``` missileClient.targetIndex
- ```string``` missileClient.missileName
- ```SpellData.obj``` missileClient.sourceIndex
- ```number``` missileClient.missileSpeed

## buffScript.obj

Properties:  

- ```number``` buffScript.hash
- ```string``` buffScript.name

## buffInstance.obj

Properties:  

- ```number``` buffInstance.type
- ```buffScript.obj``` buffInstance.script
- ```number``` buffInstance.startTime
- ```number``` buffInstance.endTime
- ```number``` buffInstance.remainingTime
- ```number``` buffInstance.counter
- ```boolean``` buffInstance.valid
- ```gameObject.obj``` buffInstance.source
- ```number``` buffInstance.stacks
- ```string``` buffInstance.name

## objManager.obj

Properties:  

- ```table``` objManager.heroes
- ```table``` objManager.turrets
- ```table``` objManager.aibases
- ```table``` objManager.minions
- ```table``` objManager.objList

> objManager.getObjectFromID(id)

**PARAMETERS**  
```number``` id  
**RETURN VALUE**  
```gameObject.obj``` object  

> objManager.getHeroesInRange(range, position, enemy, ally)

**PARAMETERS**  
```number``` range
```Vector3``` position  
```boolean``` enemy    
```boolean``` ally    
**RETURN VALUE**  
```table``` heroes  

> objManager.getEnemyHeroes()

**RETURN VALUE**  
```table``` enemies  

> objManager.getAllyHeroes()

**RETURN VALUE**  
```table``` allies  

> objManager.getEnemiesInRange(range)

**PARAMETERS**
```number``` range  
**RETURN VALUE**  
```table``` enemies  

> objManager.getEnemiesInRange(range, from)

**PARAMETERS**
```number``` range  
```Vector3``` from  
**RETURN VALUE**  
```table``` enemies  

## SpellData.obj

Properties:  

- ```spellDataResource.obj``` SpellData.resource
- ```string``` SpellData.name

## SpellDataInst.obj

Properties:  

- ```number``` SpellDataInst.level
- ```number``` SpellDataInst.ammo
- ```number``` SpellDataInst.toggleState
- ```SpellData.obj``` SpellDataInst.spellData
- ```number``` SpellDataInst.cost
- ```number``` SpellDataInst.targetingType

## spellCastInfo.obj

Properties:  

- ```boolean``` spellCastInfo.isBasicAttack
- ```number``` spellCastInfo.targetId
- ```Vector3``` spellCastInfo.startPos
- ```Vector3``` spellCastInfo.endPos
- ```number``` spellCastInfo.slot
- ```SpellData.obj``` spellCastInfo.spellData
- ```number``` spellCastInfo.castDelay
- ```gameObject.obj``` spellCastInfo.target
- ```boolean``` spellCastInfo.hasTarget
- ```number``` spellCastInfo.delay

## spellDataResource.obj

Properties:  

- ```string``` spellDataResource.displayName
- ```number``` spellDataResource.missileSpeed

# **ENUMS**

- SpellSlot
  - Q
  - W
  - E
  - R
  - S1
  - S2
  - Item1
  - Item2
  - Item3
  - Item4
  - Item5
  - Item6
  - Trinket
  - Recall
  - Unknown

- SpellState
  - Ready
  - NotAvailable
  - NotLearned
  - Supressed
  - Disabled
  - Cooldown
  - NoMana

# **GLOBALS**

- ```gameObject.obj``` player
- ```gameObject.obj``` myHero
- ```gameObject.obj``` LocalPlayer

> Log(text)

> log(text)

> print(text)

> Color(R, G, B, A)

**PARAMETERS**
```number``` R  
```number``` G  
```number``` B  
```number``` A  
**RETURN VALUE**
```number```  hexColor  

> color(R, G, B, A)

**PARAMETERS**
```number``` R  
```number``` G  
```number``` B  
```number``` A  
**RETURN VALUE**
```number```  hexColor  

# **CALLBACKS**

> cb.add(number, function)

reigsters a callback

```lua
function OnDraw()
    -- do something
end

cb.add(cb.draw, OnDraw)
```

> cb.remove(number, function)

unregisters a callback, call this in the **unload** callback

```lua
cb.remove(cb.draw, OnDraw)
```

> cb.delay_action(function, number)

used to delay a function call by the specified number in milliseconds

```lua
function PrintTime()
    print(game.time)
end

cb.delay(PrintTime, 1000)
```

## draw

no args, used for rendering only

```lua
function OnDraw()
    renderer.draw_circle(player.position, 50, 2, Color(255, 0, 0, 255))
end

cb.add(cb.draw, OnDraw)
```

## update

no args, called per game frame

## tick

no args, called every 25 game frames

## wndproc

Has two args: message, wParam

```lua
function OnWndProc(msg, wParam)
    if msg == 0x100 then -- WM_KEYDOWN
        if wParam == 0x20 then -- VK_SPACE
            print("spacebar down")
        end
    end
end

cb.add(cb.wndproc, OnWndProc)
```

## process_spell

Has two args: gameObject.obj, spellCastInfo.obj

```lua
function OnProcessSpell(sender, spell)
    print(sender.skinName .. " cast " .. spell.spellData.name)
end

cb.add(cb.process_spell, OnProcessSpell)
```

## stop_cast

Has one arg, gameObject.obj

```lua
function OnStopCast(sender)
    print(sender.skinName .. " has cancelled a cast")
end

cb.add(cb.stop_cast, OnStopCast)
```

## delete

Has two args: gameObject.obj, number

```lua
function OnDelete(sender, netID)
    print(sender.name .. " is being deleted")
end

cb.add(cb.delete, OnDelete)
```

## create_object

Has two args: gameObject.obj, number

```lua
function OnCreateObject(sender, netID)
    print(sender.name .. " has been created")
end

cb.add(cb.create_object, OnCreateObject)
```

## create_missile

Has two args: missileClient.obj, number

```lua
function OnCreateMissile(sender, netID)
    print(sender.name .. " has been created")
end

cb.add(cb.create_missile, OnCreateMissile)
```

## new_path

Has four args: gameObject.obj, table, boolean, number

```lua
    function OnNewPath(sender, path, isDash, dashSpeed)
        if isDash then
            print(sender.skinName .. " is dashing")
        else
            print(sender.skinName .. " is moving")
        end
    end

    cb.add(cb.new_path, OnNewPath)
```

## pre_attack

Has one arg, gameobject.obj

```lua
function OnPreAttack(target)
    print("orb is going to attack " .. target.skinName)
    return true
end

cb.add(cb.pre_attack, function(target) return OnPreAttack(target) end)
```

## post_attack

Has one arg, gameobject.obj

```lua
function OnPostAttack(target)
    print("orb completed attack on " .. target.skinName)
end

cb.add(cb.post_attack, OnPostAttack)
```

## unload

Has no args, triggered on plugin unload, remove your callbacks and menu here

```lua
function OnUnload()
    mainMenu.remove("rootMenuKey")

    cb.remove(cb.draw, OnDraw)
end

cb.add(cb.unload, OnUnload)

```

## execute_cast_frame

Has two args: gameObject.obj, spellCastInfo.obj

```lua
function OnProcessSpell(sender, spell)
    print(sender.skinName .. " finished casting " .. spell.spellData.name)
end

cb.add(cb.process_spell, OnProcessSpell)
```

## issue_order

Has three args: number, Vector3, gameObject.obj

```lua
function OnIssueOrder(order, pos, obj)
    if order == gameObjectOrder.moveTo then
        game.blockOrder()
        print("blocking movement")
    end
end

cb.add(cb.issue_order, OnIssueOrder)
```

## delete_missile

Has two args: missileClient.obj, number

```lua
function OnDeleteMissile(sender, netID)
    print(sender.name .. " is being deleted")
end

cb.add(cb.delete_missile, OnDelete)
```

## teleport

Has two args: gameObject.obj, number

```lua
function OnTeleport(sender, type)
    if type == teleportType.Recall then
        print(sender.skinName .. " started recalling")
    end
end

cb.add(cb.teleport, OnTeleport)
```

## vision_change

Has two args: gameObject.obj, boolean

```lua
function OnVisionChange(sender, isVisible)
    if isVisible then
        print(sender.skinName .. " becaome visible")
    end
end

cb.add(cb.vision_change, OnVisionChange)
```

## gapcloser

Has one arg, gapcloserData.obj

```lua
function OnGapCloser(args)
    print(args.sender.skinName .. " used gapcloser with slot " .. args.slot)
end

cb.add(cb.gapcloser, OnGapCloser)
```

## play_animation

Has two args: gameObject.obj, string

```lua
function OnPlayAnimation(sender, animationName)
    print(sender.skinName .. " is playing animation " .. animationName)
end

cb.add(cb.play_animation, OnPlayAnimation)
```

## unkillable_minion

Has one arg, gameObject.obj

```lua
function OnUnkillableMinion(minion)
    print("Orb cant lasthit " .. minion.skinName)
end

cb.add(cb.unkillable_minion, OnUnkillableMinion)
```

## change_inventory

## game_end

Has no args

```lua
function OnGameEnd()
    print("the game has ended")
end

cb.add(cb.game_end, OnGameEnd)
```