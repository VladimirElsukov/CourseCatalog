# Схема 2: «Процесс создания метапромпта» (flowchart, линейная, сверху вниз)

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

    P --> S1["АНАЛИЗ ЗАДАЧИ"]
    S1 --> S2["ФОРМУЛИРОВКА ПРАВИЛ"]
    S2 --> S3["ДОБАВЛЕНИЕ ПРИМЕРОВ"]
    S3 --> S4["ТЕСТИРОВАНИЕ"]

    S4 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S1,S2,S3,S4 step
    class R result
```

**Рисунок 2.** «Процесс создания метапромпта» (flowchart). **Линейная зависимость** (сверху вниз): ПРОМПТ → АНАЛИЗ ЗАДАЧИ → ФОРМУЛИРОВКА ПРАВИЛ → ДОБАВЛЕНИЕ ПРИМЕРОВ → ТЕСТИРОВАНИЕ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки.