graph TD
    %% Style definitions
    classDef founder fill:#f9f,stroke:#333,stroke-width:4px;
    classDef hub fill:#bbf,stroke:#333,stroke-width:2px;
    classDef target fill:#fff,stroke:#333,stroke-width:3px;
    classDef flavor fill:#fce4ec,stroke:#d81b60,stroke-width:3px;

    %% Global Founders
    GSC["GSC"]:::founder
    Zkit["Zkittlez"]:::founder
    OG["OG Kush"]:::founder
    ChemD["Chemdog D"]:::founder

    %% 1. STRAWMELON (The Grateful Seeds)
    SBC24["Strawberry & Cream #24"] --> SMelon["STRAWMELON"]:::flavor
    FMelon["Fresca Melon (La Chanvrière)"] --> SMelon
    
    %% Fresca Melon Context
    Zkit --> FMelon
    WMelonZ["Watermelon Zkittlez"] --> FMelon

    %% 2. OFFENSIVE SELECTIONS - DELICIOSA
    RB20["Rainbow Belts #20 (Archive)"] --> Deliciosa["DELICIOSA"]:::flavor
    PLady["Pink Lady #27"] --> Deliciosa
    
    %% Pink Lady & Apples/Bananas Context
    ABananas["Apples & Bananas (Compound)"] --> PLady
    Sourdough["Sourdough #1"] --> PLady
    Zkit --> RB20
    Moonbow["Moonbow (Dosidos x Zkit)"] --> RB20

    %% 3. ANIMAL BUTTER (3rd Coast)
    AFace["Animal Face"] --> AButter["ANIMAL BUTTER"]:::target
    PBBreath["Peanut Butter Breath"] --> AButter
    
    %% PBB Context
    Dosidos["Dosidos"] --> PBBreath
    MendoB["Mendo Breath"] --> PBBreath

    %% 4. MIRKA (Hoku Seed Co)
    PBBF2["Peanut Butter Breath F2"] --> Mirka["MIRKA"]:::target
    FYeti["Fat Yeti"] --> Mirka
    
    %% Fat Yeti Context
    Fatso["Fatso (GMO x Legend OG)"] --> FYeti
    YetiOG["Yeti OG (Loompa's Headband Bx)"] --> FYeti
    ChemC["GMO (Chem Cookies)"] -.->|Ancestor| Fatso

    %% Linkages
    Dosidos -.->|Common Ancestor| RB20
    Dosidos -.->|Common Ancestor| PBBreath

