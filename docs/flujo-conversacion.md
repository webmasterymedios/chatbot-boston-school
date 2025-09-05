graph TD
    A[Inicio: Saludo de Bienvenida] --> B{Menú Principal};

    B --> C[1. Conócenos];
    B --> D[2. Admisiones];
    B --> E[3. Procesos Administrativos];
    B --> F[4. Sedes y Contacto];
    B --> G[5. Vida Estudiantil];
    B --> H[6. Hablar con un Asesor];

    subgraph "1. Conócenos"
        C --> C1[Nuestra Historia];
        C --> C2[Nuestro Fundador];
        C --> C3[Nuestros Programas];
    end

    subgraph "2. Admisiones"
        D --> D1[Requisitos de Inscripción];
        D --> D2[Proceso Paso a Paso];
        D --> D3[Costos y Tarifas];
    end

    subgraph "3. Procesos Administrativos"
        E --> E1[Métodos de Pago];
        E --> E2[Contacto Tienda Escolar];
        E --> E3[Solicitud de Certificados];
    end

    subgraph "4. Sedes y Contacto"
        F --> F1[Información de Sedes];
        F --> F2[Contacto Secretarías];
    end

    subgraph "5. Vida Estudiantil"
        G --> G1[Eventos Relevantes];
        G --> G2[Alianzas Estratégicas];
        G --> G3[Éxito de Egresados (Becas)];
    end

    subgraph "Fin de Interacción"
        Z1[¿Puedo ayudarte con algo más?];
        Z2{Sí / No};
        Z3[Mensaje de Despedida];

        Z1 --> Z2;
        Z2 -- No --> Z3;
        Z2 -- Sí --> B;
    end

    C1 --> Z1;
    C2 --> Z1;
    C3 --> Z1;
    D1 --> Z1;
    D2 --> Z1;
    D3 --> Z1;
    E1 --> Z1;
    E2 --> Z1;
    E3 --> Z1;
    F1 --> Z1;
    F2 --> Z1;
    G1 --> Z1;
    G2 --> Z1;
    G3 --> Z1;
    H --> Z1;
