flowchart LR

A[Clientes] -->|Compras| B[E-commerce]
B --> C[CRM con IA]

subgraph IT["Negocio (IT)"]
    C --> D[ERP Conectado]
    D --> E[Base de Datos]
    D --> F[Dashboard]
end

subgraph OT["Planta (OT)"]
    G[IoT y Sensores] --> H[RFID y Códigos de Barras]
    H --> I[SCADA / Plataforma de Datos]
    I --> D
end

E --> J[IA: Predicción de Demanda y Optimización]
I --> K[IA: Optimización Operativa]

J --> D
K --> I
