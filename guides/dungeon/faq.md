---
title: FAQ
parent: Dungeon
nav_order: 6
---

### 为什么 M7 需要 S+
除了能更快的 fill RNG Meter（S+ 100% Score，S 75% Score），S+ 还提高了 Boss 奖励箱的 Quality

---
- Loot Table 中的每个物品都有自己的 Quality 和 Weight 
- 每个 Chest 则有一个 Chest Quality，受 Score, Boss Luck 等影响 
- <details> <summary> 开启奖励箱时 </summary>

    1. 移除 Loot Table 中 Quality 高于 Chest Quality 的物品
    2. 在剩余物品中抽取，每个物品抽中的概率是 Weight / Total Weight 
    3. 抽中的物品会从 Loot Table 中移除，同时扣除相应的 Quality
    4. 重复上述步骤直到 Chest Quality 用完
  </details>
---
在M7，Bedrock Chest 的 Quality 是420；Handle 和 Scroll 的 Quality 都是380

如果你想在 2nd slot 出货，要求 1st Slot Quality < Chest Quality - 380

假设你有 Treasure Artifact (1.03x), Boss Luck IV (+10), 满级 Catacomb Box (+13)

<details> <summary> S+ 以下 </summary>
  
Chest Quality 为 `[(420 * 1.03) + 10 + 13] * 1.03 + 10 + 13 = 492`

1st slot 允许的最大 Quality 为 `492 - 380 = 112`
</details>

<details> <summary> S+ 会在计算 Initial Quality 时 1.05x</summary>

Chest Quality 为 `[(420 * 1.05 * 1.03) + 10 + 13] * 1.03 + 10 + 13 = 512`

1st slot 允许的最大 Quality 为 `512 - 380 = 132`
</details>

综上，S+ 可以在 1st slot 是 Combo 2，No pain no gain 2 的情况下让你仍有机会在 2nd slot 出货 （S 则不能）

Learn more at [Loot Calculator](https://calc.pigicial.com/).

### 为什么 Debuff 比 DPS 更重要
以 P5 的龙为例，龙有 1b HP，2.5k DEF, Boss 减伤机制视为 10x，假设 A 在 Clear 时用 Duplex 最高打出 1b 伤害

根据 Wiki 上的公式，
- 无 Debuff 时，EHP = `1b * (1 + 2.5k / 100) * 10= 260b`
  > A 需要命中足足 260 箭才能将龙打死
- 仅 Death Bow，DEF = `2.5k * 50% = 1.25k`, EHP  = `1b * (1 + 1.25k/100) * 10 = 135b`
  > A 需要 135 箭就能打死。将 Last Breath 换算成伤害，相当于 25b / Hit
- Post Lethality, DEF = `1.25k * 0.91 ^ 4 = 857`, EHP = `1b * (1 + 857/100) * 10 = 85.7`
  > A 需要 86 箭就能将龙杀死。将 Lethality 换算成伤害，相当于 12.35b / Hit
- A 再用上 Armorshred Arrow, DEF = 857 * 0.95 = 814， EHP = `1b * (1 + 814/100) * 10 = 81.4`
  > A 需要 82 箭就能将龙射死

注意:
1. A 不一定每根箭都触发 Mega Crit，Duplex 也只有20%前一根箭的伤害，所以实际需要更多
2. 如果 Debuff 慢了，A 的叠箭会被吞掉，导致龙死得更慢
3. Lethality 减的是当前防御，因此先后顺序会导致不同的结果
___

[Go back to Content](/README.md)
