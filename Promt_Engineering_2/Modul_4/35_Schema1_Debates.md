# Схема 1: «Структура дебатов» (вертикальная линейная компоновка)

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
    P --> T["ТЕЗИС"]
    T --> A["СТОРОНА А\n(аргументы)"]
    A --> B["СТОРОНА Б\n(контраргументы)"]
    B --> S["СИНТЕЗ"]
    S --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef thesis fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef side fill:#FFF59D,stroke:#F9A825,stroke-width:4px
    classDef synthesis fill:#FF8A65,stroke:#BF360C,stroke-width:4px
    classDef result fill:#CE93D8,stroke:#7B1FA2,stroke-width:4px

    class P prompt
    class T thesis
    class A,B side
    class S synthesis
    class R result
```

**Рисунок 1.** «Структура дебатов» (flowchart). **Вертикальная линейная компоновка** (сверху вниз): ПРОМПТ → ТЕЗИС → СТОРОНА А (аргументы) → СТОРОНА Б (контраргументы) → СИНТЕЗ → РЕЗУЛЬТАТ. Компактная 1:1, текст полный, цвета и рамки 4px. Прямые стрелки. Видны сами дебаты (аргументы и контраргументы).