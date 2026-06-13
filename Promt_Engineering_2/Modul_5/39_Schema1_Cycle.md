# Схема 1: «Цикл управления памятью» (flowchart, линейная, сверху вниз)

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
    P --> S1["ЗАПРОС"]
    S1 --> S2["СОХРАНЕНИЕ КОНТЕКСТА"]
    S2 --> S3["ИСПОЛЬЗОВАНИЕ"]
    S3 --> S4["ОБНОВЛЕНИЕ/УДАЛЕНИЕ"]
    S4 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S1,S2,S3,S4 step
    class R result
```

**Рисунок 1.** «Цикл управления памятью» (flowchart). **Ровно 6 элементов** (сверху вниз): ПРОМПТ → ЗАПРОС → СОХРАНЕНИЕ КОНТЕКСТА → ИСПОЛЬЗОВАНИЕ → ОБНОВЛЕНИЕ/УДАЛЕНИЕ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки.