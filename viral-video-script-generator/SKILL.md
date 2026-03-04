---
name: "viral-video-script-generator"
description: "Generates 6s viral video scripts for product marketing, featuring classic characters interacting with the user's product. Invoke when user provides a product image and wants creative ad scripts."
---

# 爆款短视频脚本生成器 (Viral Video Script Generator) - 商品版

此技能专为**商品营销**设计，用于生成结合热门话题、网络热梗的短视频脚本。它能够深度解析用户提供的**商品图片**，将商品自然植入经典角色的对话和互动中，并生成**可直接用于 AI 绘画和视频生成的提示词**。

## 核心功能

1.  **商品核心 (Product-Centric)**: 一切围绕用户提供的**商品图**展开。脚本内容需突出商品的外观、功能或使用场景（如：孙悟空喝这瓶饮料、林黛玉用这个美妆产品）。
2.  **角色带货/互动**: 使用经典且形象固定的虚拟人物（如孙悟空、唐僧、林黛玉、伏地魔等），让他们与商品发生有趣的互动（吐槽、种草、争抢、展示）。
3.  **视觉一致性**: 深度解析商品图的视觉特征（颜色、包装、材质、Logo），确保生成的 **画面提示词 (Image Prompt)** 中包含准确的商品描述，保持视觉统一。
4.  **AI 生成优化**:
    *   **画面风格**: 根据用户指定的风格（如赛博朋克、皮克斯、国风等）生成画面提示词。
    *   **视频指令**: 生成用于控制视频动态的提示词（如：特写商品、手持商品展示）。
5.  **短小精悍**: 严格控制每个分镜时长（通常 3-6 秒），总时长适合短视频传播。

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
            *   **画面生成提示词 (Image Prompt)**: `[风格关键词], [商品视觉描述(核心)], [角色外观], [场景描述], [光影/构图], [画质词]`
            *   **视频生成提示词 (Video Prompt)**: `[运镜指令], [人物动作/商品展示指令], [环境动态]`

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
    *   **画面生成提示词 (Image Prompt)**: `Cyberpunk style, Ne Zha with dark circles under eyes, holding a [green energy drink bottle, glowing liquid, metallic texture] (product), sitting in high-tech gaming room, multiple screens, neon lights, messy desk, detailed, 8k`
    *   **Video Prompt**: `Handheld camera, Ne Zha raises the drink to his mouth, glowing eyes, dynamic lighting`

*   **分镜 2 (时长: 3秒)**
    *   **剧情**: 熬丙在旁边优雅地拿着另一瓶同款饮料，轻轻摇晃。
    *   **台词**: 熬丙: 别硬撑了，喝完这口，随我去龙宫... 接着练级。
    *   **画面生成提示词 (Image Prompt)**: `Cyberpunk style, Ao Bing, elegant pose, holding [green energy drink bottle] (product), cool blue holographic background, dragon elements, futuristic fashion, cinematic lighting`
    *   **Video Prompt**: `Slow pan, Ao Bing smiles slightly, shakes the bottle gently, liquid movement inside`

**(此处省略后续 9 个话题...)**
