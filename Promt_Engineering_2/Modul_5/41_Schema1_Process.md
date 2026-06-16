# Схема 1: «Процесс анализа и синтеза» (flowchart, вертикальная компоновка)

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

    P --> S1["ВХОДНЫЕ ДАННЫЕ"]
    S1 --> S2["КРИТЕРИИ АНАЛИЗА"]
    S2 --> S3["ОБРАБОТКА"]
    S3 --> S4["СИНТЕЗ"]
    S4 --> S5["ВЫВОДЫ"]

    S5 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S1,S2,S3,S4,S5 step
    class R result
```

**Рисунок 1.** «Процесс анализа и синтеза» (flowchart). **Вертикальная компоновка** (сверху вниз): ПРОМПТ → ВХОДНЫЕ ДАННЫЕ → КРИТЕРИИ АНАЛИЗА → ОБРАБОТКА → СИНТЕЗ → ВЫВОДЫ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки.