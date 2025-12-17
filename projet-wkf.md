graph TD

%% Main Component

AdDetails[📄 Page: AdDetails.tsx]

%% Styles

style AdDetails fill:#f9f,stroke:#333,stroke-width:4px

%% Data Source

Data[(🗄️ Data: ads.ts)]

%% Sub-Components

StickyHeader[🧩 AdStickyHeader]

Gallery[🧩 AdGallerySection]

MainInfo[🧩 AdMainInfo]

Desc[🧩 AdDescription]

Contact[🧩 AdContactGrid]

Video[🧩 AdVideoSection]

Report[🧩 ReportModal]

BottomNav[🧭 BottomNav]

%% Connections

AdDetails -->|Récupère les données| Data

AdDetails -->|Affiche| StickyHeader

AdDetails -->|Affiche| Gallery

AdDetails -->|Affiche| MainInfo

AdDetails -->|Affiche| Desc

AdDetails -->|Affiche| Contact

AdDetails -->|Affiche| Video

AdDetails -->|Affiche| Report

AdDetails -->|Affiche| BottomNav

%% Flow of data

Data -.->|Données envoyées| Gallery

Data -.->|Données envoyées| MainInfo

Data -.->|Données envoyées| Contact