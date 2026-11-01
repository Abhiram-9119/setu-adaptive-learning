# Setu – Architecture and Flow

The current MVP is a standalone browser application. Its decision logic runs in JavaScript and its demo progress is stored in browser local storage.

```mermaid
flowchart TD
    A[Student selects name, class and language] --> B[Diagnostic assessment]
    B --> C{Possible prerequisite gap?}
    C -- Yes --> D[Check earlier prerequisite concept]
    C -- No --> E[Recommend selected-class concept]
    D --> F[Concept dependency map and explanation]
    E --> G[Learn]
    F --> G
    G --> H[Solve practice questions]
    H --> I[Rule-based difficulty adjustment]
    I --> H
    H --> J[Five-question Test]
    J --> K{Score at least 80%?}
    K -- Yes --> L[Mark concept passed and unlock next concept]
    K -- No --> M[Recommend revision / alternative explanation]
    M --> G
    L --> N[Update browser local storage]
    N --> O[Teacher dashboard reads available demo progress]
```

## Components
- **Student interface:** collects the student's selected class and presents the learning flow.
- **Diagnostic logic:** checks the current topic and, when indicated, earlier prerequisite concepts.
- **Concept dependency map:** displays the relationship between Integers, Transposing Equations and Linear Equations.
- **Adaptive practice logic:** changes question difficulty using consecutive correct/incorrect answers.
- **Assessment logic:** calculates the five-question test score and applies the 80% pass threshold.
- **Teacher view:** displays the current browser's live student status alongside clearly labelled fictional demonstration records.
- **Persistence:** browser `localStorage`; there is no cloud database or multi-user sync in this version.
