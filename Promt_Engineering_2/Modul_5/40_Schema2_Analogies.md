# Схема 2: «Алгоритм генерации идей через аналогии» (flowchart, вертикальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "13px",
    "fontFamily": "sans-serif"
  }
}}%%
graph TD
    P["ПРОМПТ"]

    P --> S1["ПРОБЛЕМА"]
    S1 --> S2["ПОИСК АНАЛОГИЙ"]
    S2 --> S3["АДАПТАЦИЯ РЕШЕНИЙ"]

    S3 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S1,S2,S3 step
    class R result
```

**Рисунок 2.** «Алгоритм генерации идей через аналогии» (flowchart). **Вертикальная компоновка** (сверху вниз): ПРОМПТ → ПРОБЛЕМА → ПОИСК АНАЛОГИЙ → АДАПТАЦИЯ РЕШЕНИЙ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки.