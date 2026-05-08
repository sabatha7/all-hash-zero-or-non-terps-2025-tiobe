graph TD
    %% Style definitions
    classDef founder fill:#f9f,stroke:#333,stroke-width:4px;
    classDef hub fill:#bbf,stroke:#333,stroke-width:2px;
    classDef target fill:#fff,stroke:#333,stroke-width:3px;
    classDef elite fill:#ddd,stroke:#333,stroke-dasharray: 5 5;

    %% Founder Vertices
    ChemD["Chemdog D"]:::founder
    GSC["GSC (Forum Cut)"]:::founder
    SD["Sour Diesel"]:::founder
    SFV["SFV OG Kush"]:::founder
    TKush["Tuna Kush (BC Elite)"]:::elite
    MLoaf["Meatloaf (Elite Cut)"]:::elite

    %% The Mendo/OGKB Hub
    GSC --> OGKB["OGKB"]:::hub
    OGKB --> MendoB["Mendo Breath F2"]:::hub

    %% The GMO Hub
    ChemD --> GMO["GMO (Garlic Cookies)"]:::hub
    GSC --> GMO

    %% Terminal Strains (Your Collection)
    
    %% 1. ROTTEN
    GMO --> Rotten["ROTTEN"]:::target
    HC15["Hellcat #15"] --> Rotten
    %% Hellcat Context
    CPiss["Cheetah Piss"] --> HC15
    SD --> Sourdough
    GSC -.->|Re-entrant d=3| Sourdough
    Sourdough --> HC15

    %% 2. MEAT BREATH
    MendoB --> MeatB["Meat Breath"]:::target
    MLoaf --> MeatB

    %% 3. TUNA BREATH
    MendoB --> TunaB["Tuna Breath"]:::target
    TKush --> TunaB

    %% 4. DEAD UNICORN (Corrected)
    SD --> DValley["Death Valley"]
    SFV --> DValley
    GMO --> UPoop["Unicorn Poop"]
    SLady["Sophisticated Lady"] --> UPoop
    MendoB -.->|Via SLady| UPoop
    
    DValley --> DUni["Dead Unicorn"]:::target
    UPoop --> DUni

    %% 5. FROZEN PURPLE GAS
    BPunch["Banana Punch (Loki Cut)"] --> BBCups["Banana Butter Cups"]
    PBJ["PB & Jealous"] --> BBCups
    MendoB -.->|Hidden PB&J Link| PBJ
    
    GPie["Grape Pie"] --> GGas["Grape Gas (Compound)"]:::hub
    JFG["Jet Fuel Gelato"] --> GGas
    
    BBCups --> FPG["Frozen Purple Gas"]:::target
    GGas --> FPG

    %% Legend
    subgraph Legend
        direction LR
        L1[Solid = Primary Parent]
        L2[Dashed = Re-entrant / Remote Connection]
    end
