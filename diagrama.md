# Diagrama Mermaid
mermaid
flowchart LR

A[Clientes] --> B[Pedidos Online]
B --> C[CRM]

subgraph IT
    C --> D[ERP]
    D --> E[Base de Datos]
    D --> F[Dashboard]
end

subgraph OT
    G[Sensores IoT] --> H[RFID]
    H --> I[SCADA]
    I --> D
end

E --> J[IA Predicción Demanda]
I --> K[IA Optimización Operativa]

J --> D
K --> I
