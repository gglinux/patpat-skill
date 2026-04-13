# 故事引擎逻辑规则 (Story Engine Logic)

## 1. 结构化输出协议
Agent 生成的所有故事节点必须严格遵守以下 JSON 格式：

```json
{
  "node_id": "unique_string",
  "text": "针对孩子的共情叙述（不超过150字）",
  "mood_color": "#HEX_COLOR",
  "emoji": "代表当前情绪的 Emoji",
  "emotion_creature": {
    "name": "小生物名字",
    "emoji": "🔥/💧/☁️/🪨",
    "status": "当前状态描述（如：正在喷火、正在发抖）"
  },
  "choices": [
    {
      "id": "A",
      "text": "冲动反应/自然后果",
      "icon": "😤",
      "type": "natural_consequence"
    },
    {
      "id": "B",
      "text": "调节技巧/替代行为",
      "icon": "🌊",
      "type": "emotional_regulation"
    }
  ],
  "parent_coach": {
    "empathy": "家长共情话术",
    "boundary": "家长边界话术",
    "action": "即时动作指导",
    "repair_after": "事后修复建议"
  }
}
```

## 2. 叙事质量要求
*   **视角**：使用第二人称“你”，增强代入感。
*   **语言**：简单、形象、充满感官描述（例如“肚子里像塞了一个大气球”）。
*   **节奏**：一次只处理一个情绪冲突点。

## 3. 结局处理
*   **结局 A (Learning through failure)**：温和地展示冲动带来的遗憾，并提问：“如果下次重来，我们可以找谁帮忙呢？”
*   **结局 B (Empowerment)**：热烈庆祝孩子掌握了“魔法”，并给予虚拟奖牌（Emoji）。
