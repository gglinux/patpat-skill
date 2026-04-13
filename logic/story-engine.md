# Story Engine Protocol | 故事引擎协议 (2.0)

## 1. JSON Schema (Bilingual | 双语)
All responses must strictly adhere to this format to ensure cross-platform compatibility.
所有回复必须严格遵守此格式，以确保跨平台兼容性。

```json
{
  "node_id": "unique_id",
  "text": "Narrative for the child. Warm, simple, vivid. (CN, <150 chars). | 针对孩子的叙述（温暖、简单、生动，中文，<150字）",
  "body_sensation": {
    "location": "Body part (e.g., chest, tummy) | 识别到的身体部位（如：胸口、肚子）",
    "feeling": "Interoception sensation (e.g., tight, hot, jumpy) | 躯体感官描述（如：紧紧的、热热的、乱跳的）"
  },
  "emotion_creature": {
    "name": "Sparky/Drippy etc. | 小火苗/小雨滴等",
    "emoji": "🔥/💧/☁️/🪨/🌿/🐌",
    "status": "Current movement (e.g., growing big, shivering) | 当前动作（如：正在变大、正在发抖）"
  },
  "choices": [
    {
      "id": "A",
      "text": "Natural impulse (Describe the 'relief' and 'regret') | 本能冲动（描述其释放感与遗憾感）",
      "icon": "😤",
      "type": "natural_impulse"
    },
    {
      "id": "B",
      "text": "Co-regulation skill (Parent-led sync action) | 共同调节技巧（由家长发起的动作）",
      "icon": "🌊",
      "type": "co_regulation"
    }
  ],
  "co_regulation_action": "10-second sync action for parent and child to perform together. | 亲子需共同完成的10秒同步动作指令",
  "parent_coach": {
    "pre_check": "Parent self-check (Calm your own thought first) | 家长压力自检话术",
    "empathy": "Validation script (e.g., 'I see you feel... because...') | 共情话术脚本",
    "boundary": "Gentle limit (e.g., 'You can be angry, but we can't...') | 温和边界脚本",
    "action": "How to lead the co_regulation_action | 家长如何引导同步动作",
    "repair_after": "Whisper script for connection repair | 情绪平静后的连接修复悄悄话"
  }
}
```

## 2. Narrative Standards | 叙事质量标准

*   **Sensation First | 躯体感官优先**: Start with body signals (interoception) before naming the emotion. | 在命名情绪之前，先从身体信号（躯体觉察）开始描述。
*   **De-stigmatize | 去道德化**: Choice A should acknowledge the urge's power (e.g., "Yelling would feel so powerful right now"). | 选项 A 应承认冲动的诱惑力（如：“现在大声喊叫一定很有力量吧”）。
*   **Sync Logic | 同步逻辑**: Choice B must be a cooperative action between parent and child. | 选项 B 必须是家长与孩子之间的合作动作。
