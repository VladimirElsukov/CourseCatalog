# Схема 1: «Цикл итеративного улучшения» (вертикальная компоновка)

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

    P --> G["ГЕНЕРАЦИЯ"]
    G --> A["АНАЛИЗ"]
    A --> D["ДОРАБОТКА"]
    D --> P2["НОВЫЙ ПРОМПТ"]

    P2 --> G2["ГЕНЕРАЦИЯ"]
    G2 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px,color:#fff

    class P,P2 prompt
    class G,G2,A,D step
    class R result
```

**Рисунок 1.** «Цикл итеративного улучшения» (flowchart). 3 ряда: Промпт сверху, 4 этапа цикла в столбик (ГЕНЕРАЦИЯ, АНАЛИЗ, ДОРАБОТКА, НОВЫЙ ПРОМПТ), Результат снизу. Компактная 1:1, текст полный, цвета и рамки 4px. Вертикальная компоновка.