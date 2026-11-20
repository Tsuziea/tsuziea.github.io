---
title: FAQ
parent: Dungeon
nav_order: 5
---

## 为什么 M7 需要 S+

除了能更快地填充 RNG Meter（S+ 为 100% Score，S 为 75% Score），S+ 还会提高 Boss 奖励箱的 Quality。

---
- Loot Table 中的每个物品都有自己的 Quality 和 Weight 
- 每个 Chest 则有一个 Chest Quality，受 Score, Boss Luck 等影响 
- 开启奖励箱时：
  1. 移除 Loot Table 中 Quality 高于 Chest Quality 的物品
  2. 在剩余物品中抽取，每个物品抽中的概率是 Weight / Total Weight
  3. 抽中的物品会从 Loot Table 中移除，同时扣除相应的 Quality
  4. 重复上述步骤直到 Chest Quality 用完
---
在 M7，Bedrock Chest 的 Quality 是 420；Handle 和 Scroll 的 Quality 都是 380。

如果想在第 2 个槽位出货，需要满足：第 1 个槽位的 Quality < Chest Quality - 380。

假设你有 Treasure Artifact（1.03x）、Boss Luck IV（+10）和满级 Catacomb Box（+13）。

**S+ 以下：**

Chest Quality 为 `[(420 * 1.03) + 10 + 13] * 1.03 + 10 + 13 = 492`

第 1 个槽位允许的最大 Quality 为 `492 - 380 = 112`。

**S+ 会在计算 Initial Quality 时乘以 1.05：**

Chest Quality 为 `[(420 * 1.05 * 1.03) + 10 + 13] * 1.03 + 10 + 13 = 512`

第 1 个槽位允许的最大 Quality 为 `512 - 380 = 132`。

综上，S+ 时即使第 1 个槽位是 Combo 2、No Pain No Gain 2，仍有机会在第 2 个槽位出货（S 则不能）。

Learn more at [Loot Calculator](https://calc.pigicial.com/).

### 为什么 Debuff 比 DPS 更重要
以 P5 的龙为例，龙有 1b HP、2.5k DEF，Boss 减伤机制视为 10x。假设玩家 A 在 Clear 时使用 Duplex，最高打出 1b 伤害。

根据 Wiki 上的公式：
- 无 Debuff 时，EHP = `1b * (1 + 2.5k / 100) * 10 = 260b`
  > A 需要命中足足 260 箭才能将龙打死
- 仅使用 Death Bow：DEF = `2.5k * 50% = 1.25k`，EHP = `1b * (1 + 1.25k / 100) * 10 = 135b`
  > A 需要 135 箭就能打死。将 Last Breath 换算成伤害，相当于 25b / Hit
- 叠加 Lethality 后：DEF = `1.25k * 0.91 ^ 4 = 857`，EHP = `1b * (1 + 857 / 100) * 10 = 85.7b`
  > A 需要 86 箭就能将龙杀死。将 Lethality 换算成伤害，相当于 12.35b / Hit
- 再使用 Armorshred Arrow：DEF = `857 * 0.95 = 814`，EHP = `1b * (1 + 814 / 100) * 10 = 81.4b`
  > A 需要 82 箭就能将龙射死

注意：

1. A 不一定每根箭都触发 Mega Crit；Duplex 的额外箭也只有前一根箭 20% 的伤害，所以实际需要更多箭。
2. 如果 Debuff 施加得太慢，A 的叠箭会被吞掉，导致龙死得更慢。
3. Lethality 降低的是当前防御，因此施加顺序会影响结果。
