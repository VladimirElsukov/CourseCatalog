# Схема 1: «Типы цепочек промптов» (горизонтальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "14px",
    "fontFamily": "sans-serif"
  }
}}%%
graph LR
    P["ПРОМПТ"]

    P --> T1["ЛИНЕЙНАЯ"]
    P --> T2["ВЕТВЯЩАЯСЯ"]
    P --> T3["ИТЕРАТИВНАЯ"]

    T1 --> T1a["Шаг 1 → Шаг 2 → Шаг 3"]
    T2 --> T2a["Шаг 1 → Шаг 2a → Шаг 3"]
    T2 --> T2b["Шаг 1 → Шаг 2b → Шаг 3"]
    T3 --> T3a["Шаг 1 → Шаг 2 → Шаг 3 → Шаг 2 (улучшение)"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef type fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef example fill:#FFF59D,stroke:#F9A825,stroke-width:4px,color:#e65100

    class P prompt
    class T1,T2,T3 type
    class T1a,T2a,T2b,T3a example
```

**Рисунок 1.** «Типы цепочек промптов» (classification diagram). 3 ряда: Промпт слева, 3 типа цепочек в столбик (ЛИНЕЙНАЯ, ВЕТВЯЩАЯСЯ, ИТЕРАТИВНАЯ), примеры справа. Компактная 1:1, текст полный, цвета и рамки 4px. Расширение слева направо, не длинная по горизонтали.