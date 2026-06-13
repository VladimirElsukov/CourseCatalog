# Схема 2: «Правила организации дебатов» (flowchart, линейная, сверху вниз)

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

    P --> S1["ВЫБОР ТЕМЫ"]
    S1 --> S2["РАСПРЕДЕЛЕНИЕ РОЛЕЙ"]
    S2 --> S3["ФОРМУЛИРОВКА ПРАВИЛ"]
    S3 --> S4["ПРОВЕДЕНИЕ"]
    S4 --> S5["ВЫВОДЫ"]

    S5 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S1,S2,S3,S4,S5 step
    class R result
```

**Рисунок 2.** «Правила организации дебатов» (flowchart). **Линейная зависимость** (сверху вниз): ПРОМПТ → ВЫБОР ТЕМЫ → РАСПРЕДЕЛЕНИЕ РОЛЕЙ → ФОРМУЛИРОВКА ПРАВИЛ → ПРОВЕДЕНИЕ → ВЫВОДЫ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки.