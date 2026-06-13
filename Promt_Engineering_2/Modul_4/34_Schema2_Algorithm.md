# Схема 2: «Алгоритм синтеза мнений экспертов» (flowchart, линейная, сверху вниз)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "14px",
    "fontFamily": "sans-serif"
  }
}}%%
graph TD
    P["ПРОМПТ"]
    P --> S1["СБОР МНЕНИЙ"]
    S1 --> S2["ВЫЯВЛЕНИЕ СОВПАДЕНИЙ/ПРОТИВОРЕЧИЙ"]
    S2 --> S3["ОБЪЕДИНЕНИЕ/ВЫБОР"]
    S3 --> S4["ФИНАЛЬНЫЙ ОТВЕТ"]
    S4 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S1,S2,S3,S4 step
    class R result
```

**Рисунок 2.** «Алгоритм синтеза мнений экспертов» (flowchart). **Ровно 6 элементов** (сверху вниз): ПРОМПТ → СБОР МНЕНИЙ → ВЫЯВЛЕНИЕ СОВПАДЕНИЙ/ПРОТИВОРЕЧИЙ → ОБЪЕДИНЕНИЕ/ВЫБОР → ФИНАЛЬНЫЙ ОТВЕТ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки.