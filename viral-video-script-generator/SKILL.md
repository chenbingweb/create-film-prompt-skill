---
name: "viral-video-script-generator"
description: "Generates 6s viral video scripts for product marketing, featuring classic characters interacting with the user's product. Invoke when user provides a product image and wants creative ad scripts."
---

# 爆款短视频脚本生成器 (Viral Video Script Generator) - 商品版

此技能专为**商品营销**设计，用于生成结合热门话题、网络热梗的短视频脚本。它能够深度解析用户提供的**商品图片**，将商品自然植入经典角色的对话和互动中，并生成**可直接用于 AI 绘画和视频生成的提示词**。

## 核心功能

1.  **商品核心 (Product-Centric)**: 一切围绕用户提供的**商品图**展开。脚本内容需突出商品的外观、功能或使用场景（如：孙悟空喝这瓶饮料、林黛玉用这个美妆产品）。
2.  **角色带货/互动**: 使用经典且形象固定的虚拟人物（如孙悟空、唐僧、林黛玉、伏地魔等），让他们与商品发生有趣的互动（吐槽、种草、争抢、展示）。
3.  **专业分镜构图 (Cinematic Composition)**: 提供影视级的分镜描述，包括人物站位（主视/背视）、景别（中近景/特写）、镜头角度（俯拍/仰拍）及微表情指导，确保画面张力。
4.  **视觉一致性**: 深度解析商品图的视觉特征（颜色、包装、材质、Logo），确保生成的 **画面提示词 (Image Prompt)** 中包含准确的商品描述，保持视觉统一。
5.  **AI 生成优化 (双模式)**:
    *   **经典模式 (Classic)**: 适合 *Midjourney/Stable Diffusion + Runway/Pika* 工作流。提供静态画面提示词 + 简短动态指令。
    *   **高动态模式 (High-Dynamic)**: 适合 *Sora/Kling/Luma* 等新一代视频模型。提供包含**动作链、音效、特效**的全流程长文本提示词。
6.  **短小精悍**: 严格控制每个分镜时长（通常 3-6 秒），总时长适合短视频传播。

## 使用场景

*   用户提供：**风格 + 商品图片（需读取） + 文本脚本/营销卖点**。
*   用户希望制作一段创意广告或趣味短视频，让经典角色为自己的产品“代言”或进行剧情植入。

## 工作流程

1.  **解析输入**:
    *   **读取商品图**: 提取商品的**核心视觉特征**（如：红色易拉罐、发光的机械键盘、透明精华液瓶）。
    *   **分析卖点/脚本**: 理解用户想表达的商品卖点或剧情梗概。
    *   **确定风格**: 确认目标美术风格。
2.  **融合与植入**:
    *   **场景设计**: 将商品自然放置在场景中（桌上、手中、背景里）。
    *   **脚本创作**: 让角色的台词围绕商品展开，结合热梗进行趣味解读。
3.  **生成剧本**: 创作 10 个不同的对话场景。
    *   **格式要求**:
        *   **话题**: [一句话概括]
        *   **角色**: [角色 A] & [角色 B]
        *   **分镜 N (时长: X秒)**:
            *   **剧情**: [角色动作（与商品互动）与台词]
            *   **构图说明**:
                *   **人物**: [角色A (主视/背视/侧视)], [角色B (局部入镜/背景/无)]
                *   **站位**: [详细描述位置关系，如：角色A位于画面左侧三分之一处，角色B虚化在右后方]
                *   **景别**: [如：中近景 (Medium Close-up)、特写 (Close-up)、全身 (Full Shot)]
                *   **镜头角度**: [如：平视 (Eye-level)、低角度仰拍 (Low Angle)、轻微俯拍 (High Angle)]
                *   **表情要求**: [微表情描述，如：嘴角上扬带着戏谑，眼神坚定]
            *   **画面生成提示词 (Image Prompt)**: `[风格关键词], [商品视觉描述(核心)], [角色外观], [构图/站位描述], [表情/动作], [场景描述], [光影/画质词]`
            *   **视频生成提示词 (Video Prompt)**: `[运镜指令 (如: Slow zoom in, Pan left)], [构图/角度指令], [人物动作/表情变化], [商品展示动态], [环境动态]`
            *   **高动态视频脚本 (High-Dynamic Script)**: `镜头 [X-X秒] | 场景: [环境与光影细节] | 动作链: [起始动作] -> [中间动作] -> [结束动作] | 表情: [微表情变化] | 音效: [拟音/环境音] | 特效: [光效/粒子/物理碰撞]`

## 示例 (Examples)

**输入:**
*   **风格**: 赛博朋克 (Cyberpunk)
*   **商品图**: 一瓶绿色的能量饮料（用户上传图片）
*   **卖点**: 提神醒脑，熬夜必备

**输出:**

**话题 1: 修仙党的救赎**
*   **角色**: 哪吒 & 熬丙
*   **植入思路**: 哪吒熬夜打游戏，喝能量饮料回血。
*   **分镜 1 (时长: 3秒)**
    *   **剧情**: 哪吒顶着黑眼圈，手里紧紧握着**那瓶绿色的能量饮料**，背景是堆满屏幕的电竞房。
    *   **台词**: 哪吒: 我命由我不由天，但这局排位，全靠这瓶“续命水”了！
    *   **构图说明**:
        *   **人物**: 哪吒 (主视，正侧面)
        *   **站位**: 哪吒位于画面中央，身体前倾靠近屏幕，手持饮料挡在胸前。
        *   **景别**: 中近景 (Medium Close-up)
        *   **镜头角度**: 轻微仰拍 (Low Angle)，强调压迫感和专注。
        *   **表情要求**: 咬牙切齿，眼神死死盯着前方屏幕，黑眼圈明显。
    *   **画面生成提示词 (Image Prompt)**: `Cyberpunk style, Medium Close-up, Low Angle, Ne Zha with dark circles under eyes, holding a [green energy drink bottle, glowing liquid, metallic texture] (product) in front of chest, sitting in high-tech gaming room, multiple screens, neon lights, messy desk, intense expression, detailed, 8k`
    *   **Video Prompt**: `Low angle shot, handheld camera shake, Ne Zha raises the drink to his mouth aggressively, glowing eyes, dynamic lighting from screens`
    *   **高动态视频脚本 (High-Dynamic Script)**: `镜头 [0-3秒] | 场景: 赛博朋克电竞房，霓虹光影闪烁，屏幕蓝光映照在哪吒脸上 | 动作链: 哪吒紧握绿色能量饮料 -> 猛地举起饮料至嘴边 -> 仰头灌下 -> 眼神瞬间点亮 | 表情: 疲惫困倦 -> 咬牙切齿 -> 瞬间兴奋狂热 | 音效: 键盘敲击声(噼里啪啦) -> 饮料开罐声(咔嚓) -> 吞咽声(咕嘟) | 特效: 饮料瓶身流光闪动，哪吒眼中爆出红光，背景屏幕数据流加速`

*   **分镜 2 (时长: 3秒)**
    *   **剧情**: 熬丙在旁边优雅地拿着另一瓶同款饮料，轻轻摇晃。
    *   **台词**: 熬丙: 别硬撑了，喝完这口，随我去龙宫... 接着练级。
    *   **构图说明**:
        *   **人物**: 熬丙 (主视)，哪吒 (背影，边缘虚化)
        *   **站位**: 熬丙靠在电竞椅背上，位于画面右侧黄金分割点，哪吒背影在左下角。
        *   **景别**: 中景 (Medium Shot)
        *   **镜头角度**: 平视 (Eye-level)
        *   **表情要求**: 嘴角微微上扬，带着一丝优雅的嘲讽，眼神轻松。
    *   **画面生成提示词 (Image Prompt)**: `Cyberpunk style, Medium Shot, Eye-level, Ao Bing leaning on gaming chair, elegant pose, holding [green energy drink bottle] (product), blurred back of Ne Zha in foreground, cool blue holographic background, dragon elements, futuristic fashion, cinematic lighting`
    *   **Video Prompt**: `Static camera, shallow depth of field, Ao Bing smiles slightly and shakes the bottle gently, liquid movement inside, soft blue light pulsing`
    *   **高动态视频脚本 (High-Dynamic Script)**: `镜头 [3-6秒] | 场景: 同样的电竞房，侧面视角，背景是全息龙影装饰 | 动作链: 熬丙优雅靠在椅背 -> 轻轻摇晃手中的绿色饮料 -> 递向镜头方向(给哪吒) | 表情: 嘴角含笑 -> 眼神戏谑 -> 微微点头 | 音效: 液体摇晃声 -> 轻微的龙吟背景音 -> 椅子转动摩擦声 | 特效: 饮料瓶周围有淡淡的冰霜凝结，背景全息龙影缓缓游动`

**(此处省略后续 9 个话题...)**
