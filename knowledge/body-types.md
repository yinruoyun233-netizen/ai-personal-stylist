# 1. Research Foundation（研究基础）

## 1.1 Female Figure Identification Technique (FFIT)

本知识库主要基于 Female Figure Identification Technique（FFIT）构建。

FFIT 是由 North Carolina State University 研究团队提出的女性体型识别框架，
通过人体测量数据对女性身材进行系统分类。

核心测量变量包括：

- Shoulder Width（肩宽）
- Bust Circumference（胸围）
- Waist Circumference（腰围）
- Hip Circumference（臀围）

FFIT 研究广泛应用于：

- 服装设计
- 人体工程学
- 电商尺码推荐
- 个性化造型系统

---

## 1.2 Styling Philosophy（造型理念）

本系统的目标不是改变身材，而是通过服装设计优化视觉效果：

- 平衡比例
- 强化优势
- 调整视觉重心
- 提升整体风格表达

---

# 2. Anthropometric Metrics（人体测量指标）

## 2.1 Waist-to-Hip Ratio (WHR)

WHR = Waist / Hip

| 范围 | 解释 |
|------|------|
| ≤ 0.75 | 腰线非常明显 |
| 0.75–0.85 | 中等腰线 |
| > 0.85 | 腰线不明显 |

---

## 2.2 Shoulder-to-Hip Ratio (SHR)

SHR = Shoulder Width / Hip Width

| 范围 | 解释 |
|------|------|
| < 0.95 | 肩窄于臀 |
| 0.95–1.05 | 肩臀平衡 |
| > 1.05 | 肩宽于臀 |

---

## 2.3 Leg-to-Height Ratio (LHR)

LHR = Leg Length / Height

| 范围 | 解释 |
|------|------|
| < 0.45 | 腿部相对较短 |
| 0.45–0.48 | 平均比例 |
| > 0.48 | 腿部相对较长 |

---

## 2.4 Frame Size（骨架大小）

可通过手腕围度、肩宽和锁骨宽度综合判断：

- Small Frame（小骨架）
- Medium Frame（中骨架）
- Large Frame（大骨架）

---

# 3. Classification Threshold Rules（分类规则）

## Hourglass（沙漏型）

判定条件：

- |Shoulder − Hip| ≤ 5%
- WHR ≤ 0.75

---

## Pear（梨形）

判定条件：

- SHR < 0.95
- WHR ≤ 0.80

---

## Inverted Triangle（倒三角）

判定条件：

- SHR > 1.05

---

## Rectangle（矩形）

判定条件：

- 0.95 ≤ SHR ≤ 1.05
- WHR > 0.75
- 腰线不明显

---

## Apple（苹果形）

判定条件：

- WHR > 0.85
- 腹部量感明显

---

# 4. Primary Body Type Profiles（主要身材类型）

## 4.1 Pear Shape（梨形）

### Visual Characteristics
- 肩窄
- 腰细
- 胯宽
- 臀腿量感明显

### Common Challenges
- 下半身显重
- 腿粗困扰
- 比例失衡

### Styling Objectives
- 提升视觉重心
- 平衡肩胯
- 拉长腿部

### Recommended
- 方领 / V领
- 结构感肩部
- 高腰裤
- A字裙
- 深色下装

### Avoid
- 低腰裤
- 包臀紧身裙
- 臀部装饰过多

### Prompt Tags
pear-shape, narrow-shoulders, wide-hips

---

## 4.2 Apple Shape（苹果形）

### Visual Characteristics
- 腰线弱
- 腹部突出
- 上半身厚
- 腿部通常较细

### Styling Objectives
- 创造纵向线条
- 弱化中段

### Recommended
- V领
- H型外套
- 垂坠面料
- 高腰直筒裤

### Avoid
- 紧身针织
- 高领
- 腰腹褶皱

### Prompt Tags
apple-shape, undefined-waist

---

## 4.3 Hourglass（沙漏型）

### Visual Characteristics
- 肩臀平衡
- 腰线明显
- 曲线突出

### Styling Objectives
- 展现曲线
- 保持高级感

### Recommended
- 收腰设计
- 裹身裙
- 方领 / V领

### Avoid
- 过度宽松
- 完全遮腰

### Prompt Tags
hourglass, defined-waist, curvy

---

## 4.4 Rectangle（矩形）

### Visual Characteristics
- 肩腰臀差异小
- 曲线感弱

### Styling Objectives
- 创造层次与曲线

### Recommended
- 腰带
- 层次叠穿
- A字裙
- 泡泡袖

### Avoid
- 完全直筒
- 单薄贴身设计

### Prompt Tags
rectangle, straight-body

---

## 4.5 Inverted Triangle（倒三角）

### Visual Characteristics
- 肩宽
- 胯窄
- 上半身量感大

### Styling Objectives
- 弱化肩宽
- 增加下半身量感

### Recommended
- V领
- 落肩
- 阔腿裤
- A字裙

### Avoid
- 垫肩
- 泡泡袖
- 一字肩

### Prompt Tags
inverted-triangle, broad-shoulders

---

# 5. Secondary Modifiers（次级标签）

## Petite
- 身高较低
- 需强调高腰和纵向比例

## Tall
- 可驾驭长线条和叠穿

## Plus Size
- 强调结构与比例，而非遮挡

## Curvy
- 曲线明显，应强化腰线

## Long Torso
- 上半身较长，应提高腰线

## Short Legs
- 优先拉长下半身比例

---

# 6. AI Decision Logic（AI 决策逻辑）

Step 1. 获取输入：
- 身高体重
- 三围（可选）
- 照片分析结果

Step 2. 计算：
- WHR
- SHR
- LHR

Step 3. 判断主身材类型

Step 4. 识别次级标签

Step 5. 结合：
- 风格偏好
- 场景需求
- 气候条件

Step 6. 输出：
- 身材分析报告
- 核心穿搭目标
- 推荐单品
- 避免元素

---

# 7. Example Classification（示例）

Input:
- Shoulder Width = 38 cm
- Waist = 67 cm
- Hip = 96 cm

Calculated:
- WHR = 0.70
- SHR = 0.92

Result:
- Primary Type = Pear
- Secondary Modifier = Defined Waist
- Styling Objective = Balance upper and lower body

---

# 8. Prompt Template（Prompt 模板）

You are a professional fashion stylist.

Use the following metrics:
- WHR
- SHR
- LHR

Determine:
1. Primary body type
2. Secondary modifiers
3. Styling objectives
4. Recommended silhouettes
5. Items to avoid

Always explain recommendations based on visual proportion principles.

---

# 9. Ethical Guidelines（伦理准则）

AI 应：
- 使用中性和尊重的语言
- 强调比例优化而非“缺陷”
- 提供多样化风格建议

AI 不应：
- 强化身材羞辱
- 使用“胖”“缺陷”等贬义表达
- 制造外貌焦虑

---

# 10. Future Extensions（未来扩展）

- Kibbe Body Types
- Kitchener Essence
- Seasonal Color Analysis
- Male Body Type System
- Face Shape Analysis
- 3D Avatar Mapping
- Virtual Try-On Integration

---
