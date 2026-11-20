---
title: 基础
parent: Dungeon
nav_order: 1
---

## Gameplay
1. 击杀房间内所有 Nametag 上有 ✯ 的怪，会将房间标记为 Cleared
   - 怪所在的房间与 Wither Door 相连会掉落 Wither Key
   - 怪所在的房间与 Blood Door 相连会掉落 Blood Key
2. Wither Door 由煤方块组成；Blood Door 由红陶瓦组成；开门需要对应的 Key
3. 玩家需要打开 Blood Room 的门，击败 Watcher
4. Floor 1 开始，击败 Watcher 会在 Blood Room 开启一个通往 Boss 传送门，打败 Boss 即可获得奖励

## Rules
1. Potion Effects, 如 God Potion, Mixin 等会暂停
2. 除 Stamina, Healing, Mana, God Potions 外，地牢里只能使用一种药水
3. Speed 超过 100 的部分会被 0.67x
4. 每次攻击会回复 *5 + 5% 最大 Mana* 的 Mana
5. 箭矢造成的击退减弱，并且不再受无敌帧规则约束
6. <details> <summary> 附魔 </summary>
   
     - Rend, Cleave, Dragon Tracer 被禁用
     - 来自 Vampirism 的 治疗 被 0.1x
     - Venomous 的减速效果大幅降低
   </details>
7. 对 Boss 的伤害超过一定阈值时会被降低，具体取决于 Boss
   > 地牢里阈值应该是 1m，超过 1m 的部分会被 0.1x *(Not confirmed)*

## Map
1. 地牢开始后，玩家物品栏最后一格会变成 Magical Map
2. 不同类型的房间在地图上的颜色不同
3. Map 上有不同的的标记表示房间的状态

<details> <summary> 所有标记 </summary>

   - "?": 未进入的房间
   - 白"✓": 房间已经Cleared，但还有未发现的Secret
   - 绿"✓":房间已经Complete
   - "✗": Failed Puzzle，可使用 Architect's First Draft 重置
   </details>

## Rooms
1. 地牢会生成不重复，相互连接的房间
2. 通往 Blood Room 的路由Wither Doors保护，Fairy Room必然出现在这条路上

<details> <summary> 所有房间类型 </summary>

- Entrance: 地牢开始时玩家所在的房间
- Normal（普通房）: 会在固定位置生成怪物，通常还有一些 Secret。击杀所有 Nametag 上有 ✯ 的怪会标记为 Cleared
- MINIBOSS: 房间里有一个 Mini Boss
- Puzzle: 每把有2至5个，Puzzle 房的秘密通常包含 Blessing
- Trap（陷阱房），玩家需要完成最后一个秘密就算完成，
- Fairy: 仙女房: 出现在通往 Blood Room 的路上
- Blood（血房）: Watcher 会在这个房间生成小怪和上一层的 Boss，这些怪都拥有 Boss 的减伤机制，击杀所有怪就可以击败 Watcher
</details>


## [Score](https://hypixelskyblock.minecraft.wiki/w/Dungeon_Score)
<details> <summary> 来源 </summary>

   - Secret +1
   - Mimic +2 
   - Crypt +1 (Max 5)
   - Prince +1
   - Bat +1 (Max 1 per player, up to 5 players)
</details>

## [Blessing](https://hypixelskyblock.minecraft.wiki/w/Dungeon_Blessing)

Power 和 Time 可以提供大量的 Strength 和 Critical Damage 加成

## Party Finder Notes

chill: 不在乎打的快慢的人，只要不是打的特别糟糕就不会被踢

数字表示对 Personal Best 有要求，比如 5 指 5分钟内，430 指 4分30秒 内。当然也有一些是玩梗比如 67

adg: 全写是 Advanced Dungeon Guides。这是一个 Discord 服务器，队伍遵守这个服务器教程里的分工
___

[Go back to Content](/README.md)
