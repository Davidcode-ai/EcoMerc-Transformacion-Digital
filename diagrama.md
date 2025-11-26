graph TD
    %% Planta (OT)
    A[Planta_OT] --> B[IoT_y_Sensores]
    A --> C[RFID_y_Codigos]
    B --> H[Plataforma_Datos]
    C --> H
    H --> I[Motor_IA]
    I --> J[Optimización_y_Decisiones_Planta]

    %% Negocio (IT)
    D[Negocio_IT] --> E[ERP]
    D --> F[CRM_IA]
    D --> G[Chatbot_IA]
    E --> H
    F --> H
    G --> H
    H --> K[Optimización_y_Decisiones_Negocio]

    %% Comentarios
    classDef planta fill:#f9f,stroke:#333,stroke-width:1px;
    classDef negocio fill:#9ff,stroke:#333,stroke-width:1px;
    class A,B,C,J planta;
    class D,E,F,G,K negocio;
