flowchart TD
    A[Start] --> B[Input Password]

    B --> C[Check Length]
    C --> D[Check Character Types\n(lower, upper, digit, symbol)]

    D --> E[Calculate Character Set Size]

    E --> F[Compute Combinations\n(n^r with repetition)]
    F --> G[Calculate Entropy\n(length × log2(n))]

    G --> H[Check Weak Patterns]
    H --> H1[Common Password?]
    H --> H2[Sequence? (abc, 123)]
    H --> H3[Repetition? (aaa, 111)]

    H1 --> I[Adjust Score]
    H2 --> I
    H3 --> I

    C --> I
    D --> I

    I --> J[Classify Strength\n(Very Weak → Very Strong)]

    J --> K[Give Suggestions]
    K --> L[End]
