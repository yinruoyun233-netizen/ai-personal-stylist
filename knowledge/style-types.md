# 1. Introduction（知识库简介）

在个人形象管理中，“风格（Style）”并不是单一标签，而是服装在以下多个维度上的综合表达：

- Silhouette（廓形）
- Color Palette（配色）
- Fabric Texture（材质）
- Styling Details（设计细节）
- Cultural References（文化语境）
- Visual Mood（整体氛围）

例如：

- 韩系极简 = 宽松廓形 + 低饱和配色 + 干净利落氛围
- 法式风 = 收腰线条 + 柔软材质 + 自然优雅氛围
- Old Money = 经典剪裁 + 高品质面料 + 克制精致氛围

因此，AI 在识别风格时，不应只判断“这是什么风格”，而应先识别构成风格的底层属性，再根据属性组合推断最可能的风格类型。

---

# 2. Style Analysis Framework（风格分析框架）

```text
用户上传参考图片 / 描述
→ 提取视觉特征
→ 识别通用风格属性
→ 计算风格相似度
→ 输出 Primary Style + Secondary Influences
→ 结合 Body Type 做适配推荐

3. Universal Style Attributes（通用风格属性）

本章节定义 AI 在识别和推荐穿搭风格时使用的“底层视觉语言（Style Vocabulary）”。

3.1 Silhouette（廓形）
定义

服装整体形成的外轮廓，是决定比例与气场的核心因素。

常见类型
Fitted（修身）

贴合身体曲线，强调腰线与曲线感。常见于法式风。

Straight（直线）

线条简洁，视觉利落。常见于通勤极简和静奢风。

Oversized（宽松）

明显大于身体轮廓，形成松弛感。常见于韩系与美式休闲。

Structured（结构感）

肩线与剪裁清晰，呈现权威与精致感。常见于 Old Money。

Flowing（垂坠）

面料自然下垂，强调流动感与女性化。常见于法式与日系。

3.2 Color Palette（配色体系）
关键维度
Hue（色相）
Saturation（饱和度）
Brightness（明度）
Contrast（对比度）
常见特征
Neutral（中性色）

黑、白、灰、米色、驼色。高级且易搭配。

Low Saturation（低饱和）

柔和克制，韩系和静奢风常见。

Monochrome（同色系）

统一且显高。

High Contrast（高对比）

视觉鲜明，例如黑白配。

3.3 Fabric Texture（材质）

材质决定“高级感”和服装结构。

Crisp（挺括）

干练、专业，如衬衫棉和西装面料。

Soft（柔软）

亲和、温柔，如针织。

Drapey（垂坠）

优雅、流动，如真丝与雪纺。

Textured（纹理感）

层次丰富，如亚麻和粗花呢。

3.4 Styling Details（设计细节）

关键观察点：

Neckline（领型）
Sleeve Shape（袖型）
Waist Definition（腰线）
Buttons（纽扣）
Pleats（褶皱）
Hardware（金属件）
3.5 Cultural References（文化语境）
风格	来源
Korean Minimal	韩国都市审美
French Chic	巴黎女性文化
Old Money	常春藤与欧洲上流社会
Y2K	千禧年代流行文化
Japanese Natural	日本生活方式美学
3.6 Visual Mood（整体氛围）

常见标签：

Elegant（优雅）
Relaxed（松弛）
Professional（专业）
Feminine（女性化）
Youthful（年轻）
Sophisticated（成熟高级）
Playful（活泼）
Edgy（前卫）
4. Core Style Categories（核心风格体系）
4.1 Korean Minimal（韩系极简）
定义

以韩国都市日常穿搭为代表，强调低饱和配色、基础款和精准比例。

Signature Items
宽松衬衫
西装裤
短款针织
白色运动鞋
Best Body Matches
Rectangle
Pear
Petite
Prompt Tags

korean-minimal, clean-fit, soft-neutral

4.2 French Chic（法式风）
定义

自然、随性、女性化，强调 effortless elegance（不费力的精致）。

Signature Items
裹身裙
高腰牛仔裤
风衣
芭蕾鞋
Best Body Matches
Hourglass
Pear
Curvy
Prompt Tags

french-chic, effortless-elegance, feminine

4.3 Old Money（老钱风）
定义

经典、克制、强调面料与剪裁品质。

Signature Items
西装外套
羊绒针织
白衬衫
乐福鞋
Prompt Tags

old-money, heritage-classic, refined

4.4 Quiet Luxury（静奢风）
定义

低调奢华，视觉简洁但质感极强。

Signature Items
羊绒大衣
真丝衬衫
高级针织
Prompt Tags

quiet-luxury, premium-minimal, sophisticated

4.5 Office Minimal（通勤极简）
定义

专业、现代、兼顾实用性。

Signature Items
西装外套
衬衫
直筒裤
乐福鞋
Prompt Tags

office-minimal, professional-clean

4.6 American Casual（美式休闲）
Signature Items
牛仔裤
卫衣
T-shirt
Sneakers
Prompt Tags

american-casual, relaxed-denim

4.7 Japanese Natural（日系自然风）
Signature Items
亚麻衬衫
长裙
针织开衫
Prompt Tags

japanese-natural, linen-layered

4.8 Clean Girl（Clean Girl Aesthetic）
Signature Items
白背心
高腰裤
金色饰品
Prompt Tags

clean-girl, polished-minimal

4.9 Athflow（运动休闲风）
Signature Items
Leggings
Hoodie
Sneakers
Prompt Tags

athflow, sporty-comfort

4.10 Y2K（千禧复古）
Signature Items
低腰裤
短上衣
金属配饰
Prompt Tags

y2k, retro-playful

5. Occasion Mapping（场景映射）
场景	推荐风格
面试	Office Minimal, Old Money
日常通勤	Korean Minimal, Office Minimal
约会	French Chic, Clean Girl
旅行	American Casual, Japanese Natural
健身通勤	Athflow
潮流表达	Y2K
6. Style Recognition Logic（风格识别逻辑）

AI 在分析用户参考图片时，应执行以下步骤：

提取颜色特征
分析服装廓形
识别关键单品
判断材质质感
推断整体氛围
计算风格相似度
输出 Top 3 风格及置信度
7. Example Output（示例输出）

Primary Style:

Korean Minimal (78%)

Secondary Styles:

Clean Girl (15%)
Office Minimal (7%)

Key Attributes:

低饱和
高腰线
基础款
干净利落
8. Prompt Template（Prompt 模板）

Analyze the user's reference images and determine:

Primary style category
Secondary style influences
Key visual attributes
Preferred color palette
Signature items
Suitable body adaptations

Always explain the recommendation using visual proportion and styling principles.

9. Future Extensions（未来扩展）
Seasonal Color Analysis（四季色彩）
Kibbe Body Types
Kitchener Essence
Male Style Taxonomy
小红书趋势监测
Pinterest Trend Mapping
Personal Brand Styling
