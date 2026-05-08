graph TD
    %% Style definitions
    classDef founder fill:#f9f,stroke:#333,stroke-width:4px;
    classDef hub fill:#bbf,stroke:#333,stroke-width:2px;
    classDef flavor fill:#fce4ec,stroke:#d81b60,stroke-width:3px;
    classDef savory fill:#fff9c4,stroke:#fbc02d,stroke-width:3px;

    %% Key Hubs & Founders
    Zkit["Zkittlez"]:::founder
    GSC["GSC (Forum Cut)"]:::founder
    Dosi["Dosidos"]:::hub

    %% 1. STRAWMELON (Fruit & Candy Path)
    Zkit -->|via Watermelon Z| FMelon["Fresca Melon"]:::flavor
    SBC24["Strawberries & Cream #24"] -->|Mother| SMelon["STRAWMELON"]:::flavor
    FMelon -->|Father| SMelon

    %% 2. DELICIOSA (The Z-Candy Path)
    Zkit -->|Crossed with Dosidos| RB20["Rainbow Belts #20"]:::flavor
    Dosi -->|Via Moonbow| RB20
    ABananas["Apples & Bananas"] -->|Via Pink Lady| Deliciosa["DELICIOSA"]:::flavor
    RB20 -->|Archive's Cut| Deliciosa

    %% 3. ANIMAL BUTTER (The Gas & Nutty Path)
    GSC -->|Via Dosidos| Dosi
    Dosi --> PBB["Peanut Butter Breath"]:::savory
    MendoB["Mendo Breath"] --> PBB
    AFace["Animal Face"] -->|Mother| AButter["ANIMAL BUTTER"]:::savory
    PBB -->|Father| AButter

    %% 4. MIRKA (The Heavy Hitter Path)
    PBB -->|F2 Selection| Mirka["MIRKA"]:::savory
    Fatso["Fatso (GMO x Legend OG)"] -->|Via Fat Yeti| Mirka
    YetiOG["Yeti OG"] -->|Via Fat Yeti| Mirka

    %% Grouping for Clarity
    subgraph Candy_Unicorns
        SMelon
        Deliciosa
    end

    subgraph Savory_Butter_Funk
        AButter
        Mirka
    end

    %% Legend
    subgraph Legend
        direction LR
        L1[Pink = Candy/Z-Ancestry]
        L2[Yellow = Nutty/Buttery Ancestry]
    end
