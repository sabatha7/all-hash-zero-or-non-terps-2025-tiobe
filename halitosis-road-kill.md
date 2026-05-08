graph TD
    %% Style definitions
    classDef founder fill:#f9f,stroke:#333,stroke-width:4px;
    classDef hub fill:#bbf,stroke:#333,stroke-width:2px;
    classDef target fill:#fff,stroke:#333,stroke-width:3px;
    classDef elite fill:#ddd,stroke:#333,stroke-dasharray: 5 5;
    classDef skunk fill:#c8e6c9,stroke:#2e7d32,stroke-width:3px;

    %% Founder Vertices
    ChemD["Chemdog D"]:::founder
    GSC["GSC (Forum Cut)"]:::founder
    SD["Sour Diesel"]:::founder
    SFV["SFV OG Kush"]:::founder
    MLoaf["Meatloaf (Elite Cut)"]:::elite
    
    %% Skunk Founders
    Sk1["Skunk #1"]:::founder
    Afghani["Afghani"]:::founder

    %% Hubs
    GSC --> OGKB["OGKB"]:::hub
    OGKB --> MendoB["Mendo Breath F2"]:::hub
    ChemD --> GMO["GMO (Garlic Cookies)"]:::hub
    GSC --> GMO
    
    %% Skunk Hubs
    Sk1 --> SSkunk["90's Super Skunk"]:::hub
    Afghani --> SSkunk
    Sk1 --> UFester["Uncle Festers Skunk #18"]:::hub

    %% 1. CHEM COOKIES
    ChemD --> ChemC["Chem Cookies"]:::target
    GSC --> ChemC

    %% 2. MEAT BREATH
    MendoB --> MeatB["Meat Breath"]:::target
    MLoaf --> MeatB

    %% 3. DEAD UNICORN
    SD --> DValley["Death Valley"]
    SFV --> DValley
    GMO --> UPoop["Unicorn Poop"]
    SLady["Sophisticated Lady"] --> UPoop
    DValley --> DUni["Dead Unicorn"]:::target
    UPoop --> DUni

    %% 4. CORPSE FLOWER (Nature's Farm)
    SSkunk --> CFlower["Corpse Flower"]:::skunk
    UFester --> CFlower

    %% Legend
    subgraph Legend
        direction LR
        L1[Solid = Primary Parent]
        L3[Green = Skunk / Heirloom Line]
    end

