# Схема 2: «Алгоритм адаптации мастерпромпта» (flowchart, линейная, сверху вниз)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "13px",
    "fontFamily": "sans-serif"
  }
}}%%
graph TD
    P["ПРОМППТ"]

    P --> S1["ВЫБОР ЗАДАЧИ"]
    S1 --> S2["ИДЕНТИФИКАЦИЯ ПЕРЕМЕННЫХ"]
    S2 --> S3["ЗАПОЛНЕНИЕ ПАРАМЕТРОВ"]
    S3 --> S4["ТЕСТИРОВАНИЕ"]

    S4 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S1,S2,S3,S4 step
    class R result
```

**Рисунок 2.** «Алгоритм адаптации мастерпромпта» (flowchart). **Линейная зависимость** (сверху вниз): ПРОМПТ → ВЫБОР ЗАДАЧИ → ИДЕНТИФИКАЦИЯ ПЕРЕМЕННЫХ → ЗАПОЛНЕНИЕ ПАРАМЕТРОВ → ТЕСТИРОВАНИЕ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки.