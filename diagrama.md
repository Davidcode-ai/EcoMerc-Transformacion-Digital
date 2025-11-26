flowchart LR

A[Clientes] --> B[E-commerce]
B --> C[CRM]

subgraph IT
    C --> D[ERP]
    D --> E[Base de Datos]
    D --> F[Dashboard]
end

subgraph OT
    G[Sensores IoT] --> H[RFID y Códigos de Barras]
    H --> I[SCADA]
    I --> D
end

E --> J[IA: Predicción de Demanda]
I --> K[IA: Optimización Operativa]

J --> D
K --> I
