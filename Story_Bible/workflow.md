# 三位一体创作工作流 (3-Agent Pipeline)

为了规避AI写作的逻辑硬伤和机械感，我们采用以下闭环流程：

## Step 1: 逻辑审稿 (Planner/Logic Agent)
*   **输入**：上文剧情 + `Story_Bible/` + 创作意图。
*   **产出**：详细的章节大纲。
*   **核心任务**：检查是否违背人设、是否回收伏笔、冲突是否合理。
*   **防降智规则**：反派的行为必须有其自身逻辑，不能为了让主角装逼而强行降智。

## Step 2: 沉浸式初稿 (Draft/Writer Agent)
*   **指令参考**：`prompts/fanqie_style.md`。
*   **产出**：约1000-2000字的初稿。
*   **核心任务**：堆叠爽点，控制节奏。

## Step 3: 人文化精修 (Polisher/Humanizer Agent)
*   **指令参考**：`prompts/humanizer_polish.md`。
*   **产出**：最终成品。
*   **核心任务**：去AI味、打碎段落、增加生理描写和口语感。
