flowchart LR

%% Clientes y ventas
A[Clientes] --> B[E-commerce]
B --> C[CRM con IA]

%% Negocio (IT)
subgraph IT["Negocio (IT)"]
    C --> D[ERP Conectado]
    D --> E[Base de Datos]
    D --> F[Dashboard]
end

%% Planta / Operaciones (OT)
subgraph OT["Planta (OT)"]
    G[Sensores IoT] --> H[RFID y Códigos de Barras]
    H --> I[SCADA / Plataforma de Datos]
    I --> D
    I --> L[Almacén / Control de Inventario]
    L --> M[Transportistas]
end

%% Inteligencia Artificial
E --> J[IA: Predicción de Demanda]
I --> K[IA: Optimización Operativa]

J --> D
K --> I
