graph TD
    %% Style definitions
    classDef founder fill:#f9f,stroke:#333,stroke-width:4px;
    classDef hub fill:#bbf,stroke:#333,stroke-width:2px;
    classDef target fill:#fff,stroke:#333,stroke-width:3px;
    classDef hash fill:#fff9c4,stroke:#fbc02d,stroke-width:3px;
    classDef shwale fill:#e0f2f1,stroke:#00796b,stroke-width:2px;

    %% Global Founders
    ChemD["Chemdog D"]:::founder
    GSC["GSC (Forum Cut)"]:::founder
    Trop["Tropicanna Cookies"]:::hub
    Papaya["Papaya"]:::hub
    GPie["Grape Pie"]:::hub
    Melon["Melon"]:::hub

    %% THE MAMIKO/GMO HUB
    ChemD --> ChemC["CHEM COOKIES / GMO"]:::target
    GSC --> ChemC

    %% 1. TROPICAL RAIN
    Trop --> PTPie["Poon Tang Pie"]:::hub
    GPie --> PTPie
    Papaya --> PTPie
    PTPie --> TRain["TROPICAL RAIN"]:::hash
    FJoy["Fruitjoy #20"] --> TRain

    %% 2. JAMON & MELON
    %% Corrected: GMO/ChemC is an ancestor of Hash Burger via Donny Burger
    HBurger["Hash Burger"]:::hub --> JMelon["JAMON & MELON"]:::hash
    MGranita["Melon Granita"] --> JMelon
    Melon --> MGranita
    ChemC -.->|Ancestor via Donny Burger| HBurger

    %% 3. GAS MINT
    GMint["Gushmint"] --> GasM["GAS MINT"]:::hash
    MM26["26MM"] --> GasM

    %% 4. THE FUNK FROM MARS (Deep lineage from 1000062959.webp)
    PPunch["Purple Punch"] --> GDonut["Glazed Donut"]:::shwale
    CFuel["Cake Fuel"] --> GDonut
    Truth["The Truth"] --> SCoat["Sugar Coat"]:::shwale
    GDonut --> SCoat
    GDonut --> BDozen["Bakers Dozen"]:::shwale
    SCoat --> SShack["Sugar Shack"]:::shwale
    BDozen --> SShack
    
    %% JOMO uses the ChemC/GMO genetics directly in the cross
    SShack --> JOMO["JOMO"]:::shwale
    ChemC --> JOMO
    
    JOMO --> DGlands["Diamond Glands"]:::shwale
    FPie["Frozay Pie"] --> FMars["THE FUNK FROM MARS"]:::hash
    DGlands --> FMars

    %% Legend
    subgraph Legend
        direction LR
        L1[Solid = Direct Parent]
        L2[Dashed = Distant Ancestor/Influence]
    end

