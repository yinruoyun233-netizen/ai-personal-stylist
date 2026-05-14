# 1. Introduction（知识库简介）

在现代个人形象管理中，“风格（Style）”并不是单一标签，而是服装在多个视觉维度上的综合表达。

用户通常会说：

- “我喜欢这种高级感”
- “我想穿得更有气质”
- “我不知道是什么风格，但觉得很好看”

这些表达本质上是在描述一种“视觉感受”，而不是标准化风格名称。

因此，AI 不应该直接猜测：

> “这是法式风”  
> “这是韩系风”

而应该先识别：

- 服装轮廓（Silhouette）
- 配色逻辑（Color Palette）
- 材质特征（Fabric Texture）
- 设计细节（Styling Details）
- 整体氛围（Visual Mood）
- 文化语境（Cultural References）

再通过这些底层属性组合，推断最终风格类型。

---

# 2. Style Analysis Framework（风格分析框架）

```text
用户上传参考图片 / 穿搭描述
↓
提取视觉特征
↓
识别通用风格属性
↓
建立风格向量（Style Vector）
↓
计算风格相似度
↓
输出：
- Primary Style
- Secondary Influences
- Body Adaptation
- Styling Suggestions
```

---

# 3. Universal Style Attributes（通用风格属性）

本章节定义 AI 在分析风格时使用的“底层视觉语言（Style Vocabulary）”。

这些属性是所有风格的基础组成元素。

---

## 3.1 Silhouette（廓形）

### Definition（定义）

廓形（Silhouette）是服装整体形成的外轮廓。

它决定：

- 视觉比例
- 气场
- 身高感
- 曲线感
- 松弛感
- 权威感

廓形是风格识别中最核心的变量之一。

---

### Fitted（修身）

服装贴合身体轮廓，强调曲线与腰线。

#### Visual Effects（视觉效果）

- 展现身材
- 强化女性化
- 更成熟精致

#### Common In（常见风格）

- French Chic
- Romantic
- 性感风格

#### Suitable Body Types（适配身材）

- Hourglass
- Curvy

---

### Straight（直线）

线条垂直简洁，不刻意强调身体曲线。

#### Visual Effects

- 利落
- 现代
- 职场感

#### Common In

- Office Minimal
- Quiet Luxury

---

### Oversized（宽松）

服装轮廓明显大于身体。

#### Visual Effects

- 松弛感
- 年轻化
- 潮流感

#### Risks（潜在问题）

- 压身高
- 掩盖腰线

#### Common In

- Korean Minimal
- Streetwear
- American Casual

---

### Structured（结构感）

通过肩线与剪裁形成明确轮廓。

#### Visual Effects

- 权威
- 高级
- 强气场

#### Common In

- Old Money
- Tailoring
- Formalwear

---

### Flowing（垂坠）

面料自然下垂并形成流动感。

#### Visual Effects

- 优雅
- 女性化
- 柔和

#### Common In

- French Chic
- Japanese Natural

---

## 3.2 Color Palette（配色体系）

### Definition（定义）

颜色是用户最容易感知风格的维度。

同样的服装，在不同配色下会呈现完全不同的视觉气质。

---

### Hue（色相）

颜色类别。

例如：

- 蓝色
- 驼色
- 酒红色

---

### Saturation（饱和度）

颜色鲜艳程度。

#### High Saturation（高饱和）

视觉更年轻、更张扬。

#### Low Saturation（低饱和）

视觉更高级、更柔和。

韩系、静奢风中大量使用低饱和颜色。

---

### Brightness（明度）

颜色明暗程度。

#### High Brightness

更轻盈、年轻。

#### Low Brightness

更稳重、成熟。

---

### Contrast（对比度）

颜色之间的差异程度。

#### High Contrast

例如黑白配色。

视觉效果：

- 强烈
- 利落
- 强存在感

#### Low Contrast

视觉效果：

- 温柔
- 统一
- 松弛

---

### Neutral Colors（中性色）

包括：

- 黑
- 白
- 灰
- 米色
- 驼色

#### Visual Effects

- 百搭
- 稳定
- 高级

---

### Monochrome（同色系）

同一色系不同深浅搭配。

#### Visual Effects

- 显高
- 统一
- 极简感

---

## 3.3 Fabric Texture（材质）

### Definition（定义）

材质决定服装的：

- 挺括度
- 光泽
- 厚重感
- 垂坠感
- 高级感

---

### Crisp（挺括）

例如：

- 西装面料
- 衬衫棉

#### Visual Effects

- 干练
- 专业
- 清晰结构

---

### Soft（柔软）

例如：

- 针织
- 莫代尔

#### Visual Effects

- 温柔
- 亲和
- 日常感

---

### Drapey（垂坠）

例如：

- 真丝
- 雪纺

#### Visual Effects

- 优雅
- 流动感
- 女性化

---

### Textured（纹理感）

例如：

- 亚麻
- 粗花呢

#### Visual Effects

- 层次丰富
- 更具生活方式感
- 文艺感

---

## 3.4 Styling Details（设计细节）

### Definition（定义）

细节是决定风格识别度的重要因素。

很多时候：

> 风格差异不来自单品本身，而来自细节。

---

### Key Elements（关键元素）

- Neckline（领型）
- Sleeve Shape（袖型）
- Waist Definition（腰线）
- Buttons（纽扣）
- Pleats（褶皱）
- Hardware（金属件）
- Hemline（裙摆）
- Pattern（图案）

---

## 3.5 Cultural References（文化语境）

### Definition（定义）

许多风格本身具有明确文化来源。

AI 不仅需要识别视觉特征，还需要理解其文化背景。

---

| Style | Cultural Origin |
|---|---|
| Korean Minimal | 韩国都市日常审美 |
| French Chic | 巴黎女性穿衣文化 |
| Old Money | 欧洲上流社会与常春藤文化 |
| Quiet Luxury | 当代高端极简主义 |
| Y2K | 千禧年代流行文化 |
| Japanese Natural | 日本生活方式美学 |

---

## 3.6 Visual Mood（整体氛围）

### Definition（定义）

Mood 是用户最常感知但最难准确描述的部分。

用户常说：

- “我想看起来更高级”
- “我想有松弛感”
- “我想更有气质”

这些本质上都属于氛围描述。

---

### Common Mood Labels（常见氛围标签）

- Elegant（优雅）
- Relaxed（松弛）
- Professional（专业）
- Feminine（女性化）
- Youthful（年轻）
- Sophisticated（成熟高级）
- Romantic（浪漫）
- Playful（活泼）
- Edgy（前卫）
- Powerful（强气场）

---

## 3.7 Style DNA（风格 DNA）

每一种风格，本质上都是上述属性的固定组合。

---

### Korean Minimal

```text
Oversized + High Waist
Low Saturation
Neutral Colors
Clean Mood
```

---

### French Chic

```text
Fitted + Flowing
Defined Waist
Soft Fabrics
Feminine Mood
```

---

### Old Money

```text
Structured Tailoring
Premium Fabrics
Heritage Colors
Refined Mood
```

---

### Quiet Luxury

```text
Straight Silhouette
Monochrome Palette
Luxury Materials
Sophisticated Mood
```

---

## 3.8 AI Usage Guidelines（AI 调用规则）

在分析用户上传的参考图片时，AI 应依次执行：

1. 提取颜色特征
2. 判断廓形类型
3. 识别材质属性
4. 分析关键设计细节
5. 判断文化语境
6. 总结整体氛围
7. 输出属性标签
8. 计算风格概率分布
9. 生成 Primary Style 与 Secondary Influences

---

# 4. Core Style Categories（核心风格体系）

---

## 4.1 Korean Minimal（韩系极简）

### Definition（定义）

强调：

- 低饱和
- 基础款
- 宽松轮廓
- 干净比例

核心理念：

> “不费力但很精致”

---

### Signature Items（代表单品）

- 宽松衬衫
- 西装裤
- 短款针织
- 白色运动鞋

---

### Common Colors（常见配色）

- 米白
- 灰色
- 雾蓝
- 黑色
- 卡其色

---

### Suitable Body Types（适配身材）

- Rectangle
- Pear
- Petite

---

### Prompt Tags

```text
korean-minimal, clean-fit, soft-neutral
```

---

## 4.2 French Chic（法式风）

### Definition（定义）

强调：

- 女性化
- 自然感
- 收腰
- effortless elegance

核心理念：

> “看起来像没有刻意打扮，但非常迷人”

---

### Signature Items

- 裹身裙
- 风衣
- 高腰牛仔裤
- 芭蕾鞋

---

### Common Colors

- 黑白
- 酒红
- 海军蓝
- 驼色

---

### Suitable Body Types

- Hourglass
- Curvy

---

### Prompt Tags

```text
french-chic, feminine, effortless-elegance
```

---

## 4.3 Old Money（老钱风）

### Definition（定义）

强调：

- 克制
- 高品质
- 经典剪裁
- 非 Logo 化

核心不是“贵”，而是：

> “长期稳定的上层阶级审美”

---

### Signature Items

- 西装外套
- 羊绒针织
- 白衬衫
- 乐福鞋

---

### Common Colors

- 驼色
- 奶油白
- 海军蓝
- 深棕

---

### Prompt Tags

```text
old-money, heritage-classic, refined
```

---

## 4.4 Quiet Luxury（静奢风）

### Definition（定义）

视觉上极简，但强调：

- 面料
- 剪裁
- 质感
- 做工

---

### Signature Items

- 羊绒大衣
- 真丝衬衫
- 高级针织

---

### Prompt Tags

```text
quiet-luxury, premium-minimal, sophisticated
```

---

## 4.5 Office Minimal（通勤极简）

### Definition（定义）

强调：

- 专业感
- 实用性
- 现代职场审美

---

### Signature Items

- 西装外套
- 直筒裤
- 衬衫
- 乐福鞋

---

### Prompt Tags

```text
office-minimal, professional-clean
```

---

## 4.6 American Casual（美式休闲）

### Definition（定义）

强调：

- 舒适
- 功能性
- 青春感

---

### Signature Items

- 牛仔裤
- 卫衣
- T-shirt
- Sneakers

---

### Prompt Tags

```text
american-casual, relaxed-denim
```

---

## 4.7 Japanese Natural（日系自然风）

### Definition（定义）

强调：

- 天然材质
- 松弛层次
- 生活感

---

### Signature Items

- 亚麻衬衫
- 长裙
- 针织开衫

---

### Prompt Tags

```text
japanese-natural, linen-layered
```

---

## 4.8 Clean Girl（Clean Girl Aesthetic）

### Definition（定义）

强调：

- 干净
- 健康
- 自律感

---

### Signature Items

- 白背心
- 高腰裤
- 金色饰品

---

### Prompt Tags

```text
clean-girl, polished-minimal
```

---

## 4.9 Athflow（运动休闲风）

### Definition（定义）

将运动服与日常穿搭结合。

---

### Signature Items

- Leggings
- Hoodie
- Sneakers

---

### Prompt Tags

```text
athflow, sporty-comfort
```

---

## 4.10 Y2K（千禧复古）

### Definition（定义）

受 1990s–2000s 流行文化影响。

强调：

- 青春感
- 个性
- 高存在感

---

### Signature Items

- 低腰裤
- 短上衣
- 金属配饰

---

### Prompt Tags

```text
y2k, retro-playful
```

---

# 5. Occasion Mapping（场景映射）

| Occasion | Recommended Styles |
|---|---|
| 面试 | Office Minimal / Old Money |
| 日常通勤 | Korean Minimal / Office Minimal |
| 约会 | French Chic / Clean Girl |
| 旅行 | American Casual / Japanese Natural |
| 健身通勤 | Athflow |
| 潮流表达 | Y2K |

---

# 6. Style Recognition Logic（风格识别逻辑）

AI 在分析用户参考图片时，应执行以下步骤：

1. 提取颜色特征
2. 判断廓形类型
3. 识别关键单品
4. 分析材质属性
5. 推断文化语境
6. 总结整体氛围
7. 计算风格相似度
8. 输出 Top 3 风格及置信度

---

# 7. Example Output（示例输出）

## Primary Style

```text
Korean Minimal (78%)
```

---

## Secondary Influences

```text
Clean Girl (15%)
Office Minimal (7%)
```

---

## Key Attributes

```text
- 低饱和
- 高腰线
- 基础款
- 干净利落
```

---

# 8. Prompt Template（Prompt 模板）

```text
Analyze the user's reference images and determine:

1. Primary style category
2. Secondary style influences
3. Key visual attributes
4. Preferred color palette
5. Signature items
6. Suitable body adaptations

Always explain the recommendation using visual proportion and styling principles.
```

---

# 9. Future Extensions（未来扩展）

- Seasonal Color Analysis（四季色彩）
- Kibbe Body Types
- Kitchener Essence
- Male Style Taxonomy
- 小红书趋势监测
- Pinterest Trend Mapping
- Fashion Trend Forecasting
- AI Outfit Scoring System
- Personal Brand Styling

---
