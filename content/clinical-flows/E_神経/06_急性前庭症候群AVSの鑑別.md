---
title: 急性前庭症候群 (AVS) の鑑別
date: 2026-11-03
---

# 急性前庭症候群 (AVS) の鑑別
親カテゴリ: [[clinical-flows/E_神経/index|E章 神経]]

## 疾患概念とピットフォール
持続性の回転性めまい、自発眼振、嘔気・嘔吐、歩行障害を呈する急性症候群[cite: 352]。
- **末梢性**: 前庭神経炎（最多）、迷路炎[cite: 352, 353]。
- **中枢性**: 小脳・脳幹梗塞（**PICA梗塞、AICA梗塞**）[cite: 352, 353]。

> [!WARNING]- 早期MRIの偽陰性
> 発症48時間以内の後頭蓋窩・脳幹部ラクナ梗塞において、**拡散強調MRI (DWI) の偽陰性率は最大で約50%** に達する[cite: 352, 355, 356]。画像のみで小脳・脳幹梗塞を除外してはならず、ベッドサイドの**HINTS plus 診察**が最も鋭敏である[cite: 352, 354]。

---

## HINTS Plus アルゴリズム

以下の3検査のうち、**1つでも中枢パターン（または急性難聴）を認めれば「中枢性（脳卒中）」** と判定する（感度99%、特異度97%）[cite: 354, 355]。
```mermaid
flowchart TD
    Start([持続性自発眼振を伴う急性めまい]) --> Step1["1. Head Impulse Test (HIT)"]
    Start --> Step2["2. Nystagmus（注視方向性眼振）"]
    Start --> Step3["3. Test of Skew（垂直偏位）"]
    Start --> StepPlus["Plus: 新規発症の急性難聴"]

    %% 1. HIT
    Step1 --> HIT_Norm["正常（Catch-up saccade なし）"]
    HIT_Norm --> Central_HIT["【中枢性（PICA梗塞示唆）】"]
    Step1 --> HIT_Abn["異常（健側への回旋で眼球が外れ、補正サッケードあり）"]
    HIT_Abn --> Peri_HIT["末梢性示唆"]

    %% 2. Nystagmus
    Step2 --> Nyst_Dir["方向交代性（右注視で右向き、左注視で左向き）<br>または垂直眼振"]
    Nyst_Dir --> Central_Nyst["【中枢性】"]
    Step2 --> Nyst_Uni["単方向性水平回旋混合眼振<br>（どの方向を見ても一方向）"]
    Nyst_Uni --> Peri_Nyst["末梢性示唆"]

    %% 3. Test of Skew
    Step3 --> Skew_Dev["交互遮蔽試験で上下方向の再固視眼球運動あり"]
    Skew_Dev --> Central_Skew["【中枢性（脳幹病変）】"]
    Step3 --> Skew_No["上下偏位なし"]
    Skew_No --> Peri_Skew["末梢性示唆"]

    %% Plus: 急性難聴
    StepPlus --> Hearing_Loss["難聴合併あり"]
    Hearing_Loss --> Central_AICA["【中枢性（内耳梗塞 / AICA梗塞）】"]
```
> [!NOTE]- AICA（前下小脳動脈）梗塞の注意点
> AICAから内耳動脈が分岐するため、AICA梗塞では内耳壊死を伴い、**HITが末梢パターン（偽末梢所見）** を呈する[cite: 352, 353, 355]。これを拾い上げるために「指こすり試験等による急性難聴の有無」を必ず評価する（HINTS Plus）[cite: 354, 355]。
