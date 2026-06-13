# Схема: «Шкала тонов и стилей» (вертикальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "14px",
    "fontFamily": "sans-serif"
  }
}}%%
graph TD
    ОФИЦИАЛЬНЫЙ["ОФИЦИАЛЬНЫЙ\n(формальный, без эмоций)"]
    РАЗГОВОРНЫЙ["РАЗГОВОРНЫЙ\n(простой, с обращениями)"]
    ЮМОРИСТИЧЕСКИЙ["ЮМОРИСТИЧЕСКИЙ\n(шутки, ирония, преувеличения)"]
    МОТИВИРУЮЩИЙ["МОТИВИРУЮЩИЙ\n(позитивный, с призывами)"]
    НЕЙТРАЛЬНЫЙ["НЕЙТРАЛЬНЫЙ\n(объективный, фактологический)"]

    ОФИЦИАЛЬНЫЙ --> РАЗГОВОРНЫЙ
    РАЗГОВОРНЫЙ --> ЮМОРИСТИЧЕСКИЙ
    ЮМОРИСТИЧЕСКИЙ --> МОТИВИРУЮЩИЙ
    МОТИВИРУЮЩИЙ --> НЕЙТРАЛЬНЫЙ

    classDef tone1 fill:#1565c0,stroke:#0d47a1,stroke-width:4px,color:#fff
    classDef tone2 fill:#42a5f5,stroke:#1565c0,stroke-width:4px,color:#fff
    classDef tone3 fill:#66bb6a,stroke:#2e7d32,stroke-width:4px,color:#fff
    classDef tone4 fill:#ffa726,stroke:#ef6c00,stroke-width:4px,color:#fff
    classDef tone5 fill:#ab47bc,stroke:#6a1b9a,stroke-width:4px,color:#fff

    class ОФИЦИАЛЬНЫЙ tone1
    class РАЗГОВОРНЫЙ tone2
    class ЮМОРИСТИЧЕСКИЙ tone3
    class МОТИВИРУЮЩИЙ tone4
    class НЕЙТРАЛЬНЫЙ tone5
```

**Рисунок.** «Шкала тонов и стилей» (вертикальная компоновка). Пять тонов в один столбец сверху вниз с равными расстояниями. Компактная 1:1, текст полный, цвета и рамки 4px. Каждый тон имеет свой цвет для визуального разделения.