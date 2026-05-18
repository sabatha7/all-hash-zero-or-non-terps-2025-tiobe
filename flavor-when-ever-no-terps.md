graph TD
    %% Style definitions
    classDef founder fill:#f9f,stroke:#333,stroke-width:4px;
    classDef hub fill:#bbf,stroke:#333,stroke-width:2px;
    classDef flavor fill:#fce4ec,stroke:#d81b60,stroke-width:3px;
    classDef savory fill:#fff9c4,stroke:#fbc02d,stroke-width:3px;
    classDef citrus fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px;

    %% Key Hubs & Founders
    Zkit["Zkittlez"]:::founder
    GSC["GSC (Forum Cut)"]:::founder
    Dosi["Dosidos"]:::hub
    GG["Grape Gas"]:::hub

    %% 1. STRAWMELON (Fruit & Candy Path)
    Zkit -->|via Watermelon Z| FMelon["Fresca Melon"]:::flavor
    SBC24["Strawberries & Cream #24"] -->|Mother| SMelon["STRAWMELON"]:::flavor
    FMelon -->|Father| SMelon

    %% 2. ANIMAL BUTTER (The Gas & Nutty Path)
    GSC -->|Via Dosidos| Dosi
    Dosi --> PBB["Peanut Butter Breath"]:::savory
    MendoB["Mendo Breath"] --> PBB
    AFace["Animal Face"] -->|Mother| AButter["ANIMAL BUTTER"]:::savory
    PBB -->|Father| AButter

    %% 3. CITRUS LINES (Blood Lime & Clementine Gold)
    LSkunk["Lemon Skunk"] --> BLime["BLOOD LIME"]:::citrus
    BOTangie["Blood Orange Tangie"] --> BLime
    K24["24K"] --> CGold["CLEMENTINE GOLD"]:::citrus
    CTangie["Clementine Tangie"] --> CGold

    %% 4. EL KREM PEACHES LINE (Fez & Cheri Granada)
    RB20["Rainbow Belts"]:::flavor --> Fez["FEZ"]:::flavor
    Zkit -->|Via Rainbow Belts| RB20
    MPeaches["Moroccan Peaches"] --> Fez
    MPeaches --> CGranada["CHERI GRANADA"]:::flavor
    
    %% Cheri Breakdown
    CPie["Cherry Pie"] --> Cheri["Cheri"]
    FFruit["Forbidden Fruit"] --> Cheri
    Zkit --> Cheri
    Cheri --> CGranada

    %% 5. DIRTY GRAPE
    BMaple["Black Maple"] --> DGrape["DIRTY GRAPE"]:::flavor
    GG --> DGrape

    %% 6. JOKER RUNTZ
    %% Joker Juice Breakdown
    JCandy["Jokerz Candy"] --> JJuice["Joker Juice"]
    Temp["Temptation"] --> JJuice
    JJuice --> JRuntz["JOKER RUNTZ"]:::flavor
    
    %% Black Runtz Breakdown
    Zkit --> BRuntz["Black Runtz"]
    G33["Gelato #33"] --> BRuntz
    BRuntz --> JRuntz

    %% Grouping for Clarity
    subgraph Candy_Fruit_Terps
        SMelon
        Fez
        CGranada
        DGrape
        JRuntz
    end

    subgraph Citrus_Zest
        BLime
        CGold
    end

    subgraph Savory_Butter_Funk
        AButter
    end

    %% Legend
    subgraph Legend
        direction LR
        L1[Pink = Candy/Z/Fruit Ancestry]
        L2[Green = Citrus Profiles]
        L3[Yellow = Nutty/Buttery Ancestry]
    end
