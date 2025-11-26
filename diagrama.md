graph TD
A[Planta_OT] --> B[IoT_y_Sensores]
A --> C[RFID_Codigos]
B --> H[Plataforma_Datos]
C --> H

D[Negocio_IT] --> E[ERP]
D --> F[CRM_IA]
D --> G[Chatbot_IA]
E --> H
F --> H
G --> H

H --> I[Motor_IA]
I --> J[Decisiones_y_Optimizacion]
