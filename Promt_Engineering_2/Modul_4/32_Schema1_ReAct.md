# Схема 1: «Структура ReAct» (вертикальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "14px",
    "fontFamily": "sans-serif"
  }
}}%%
graph TD
    P["ПРОМПТ"] -->|Задача + роль| R1["РАССУЖДЕНИЕ 1"]
    R1 -->|Объясни, почему| A1["ДЕЙСТВИЕ 1"]
    A1 -->|Что сделать| R2["РАССУЖДЕНИЕ 2"]
    R2 -->|Объясни, почему| A2["ДЕЙСТВИЕ 2"]
    A2 -->|Что сделать| F["ФИНАЛЬНЫЙ ОТВЕТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef reasoning fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef action fill:#FFF59D,stroke:#F9A825,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class R1,R2 reasoning
    class A1,A2 action
    class F result
```

**Рисунок 1.** «Структура ReAct» (flowchart). **Вертикальная компоновка** (сверху вниз): ПРОМПТ → РАССУЖДЕНИЕ 1 → ДЕЙСТВИЕ 1 → РАССУЖДЕНИЕ 2 → ДЕЙСТВИЕ 2 → ФИНАЛЬНЫЙ ОТВЕТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки с текстом.