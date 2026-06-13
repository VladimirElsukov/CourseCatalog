# Схема 2: «Цикл ReAct» (loop diagram, вертикальная компоновка)

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

    P --> A["АНАЛИЗ"]
    A --> P2["ПЛАН"]
    P2 --> D["ДЕЙСТВИЕ"]
    D --> C["ПРОВЕРКА"]
    C --> P3["ПОВТОРЕНИЕ"]

    P3 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px,color:#fff

    class P,P2,P3 prompt
    class A,D,C step
    class R result
```

**Рисунок 2.** «Цикл ReAct» (loop diagram). **Вертикальная компоновка** (сверху вниз): Промпт сверху, 4 этапа цикла в столбик (АНАЛИЗ → ПЛАН → ДЕЙСТВИЕ → ПРОВЕРКА → ПОВТОРЕНИЕ), Результат снизу. Компактная 1:1, текст полный, цвета и рамки 4px.