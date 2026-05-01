```mermaid
flowchart TD
    A[Start] --> B[Input Password]
    B --> C[Check Length]
    C --> D[Check Character Types (lower, upper, digit, symbol)]
    D --> E[Calculate Character Set Size]
    E --> F[Compute Combinations (n^r)]
    F --> G[Calculate Entropy (length × log2(n))]
    G --> H[Check Weak Patterns]
    H --> I[Adjust Score]
    I --> J[Classify Strength]
    J --> K[Give Suggestions]
    K --> L[End]
```
