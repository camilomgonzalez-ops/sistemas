flowchart TD

A[Inicio del día] --> B[Consulta 1: Revisar inventario de sabores]
B --> C{¿Hay stock mínimo?}

C -->|No| D[Generar pedido urgente al proveedor]
D --> B

C -->|Sí| E[Colocar baldes en la vitrina]

E --> F[Consulta 2: Verificar envases en depósito]
F --> G{¿Hay envases suficientes?}

G -->|No| H[Reponer envases o realizar pedido]
H --> F

G -->|Sí| I[Comienza atención al público]

I --> J[*Boom del sabor Pistacho*]

J --> K[Consulta 3: Verificar stock real de Pistacho]
K --> L{¿Alcanza el Pistacho para la demanda?}

L -->|Sí| M[Reponer Pistacho en vitrina y continuar]

L -->|No| N[Iniciar protocolo por escasez]

N --> O[Consulta 4: Revisar baldes reservados]
O --> P{¿Hay baldes extra?}

P -->|Sí| Q[Reponer sabor con balde extra]
Q --> R[Continuar atención]

P -->|No| S[Consulta 5: Ver lista de sustitutos]

S --> T{¿Ofrecer sabor sustituto?}

T -->|Sí| U[Sugerir sabores alternativos]
U --> R

T -->|No| V[Suspender venta de Pistacho]
V --> R

R --> W[Consulta final: Actualizar inventario del día]
W --> X{¿Pedir Pistacho urgente?}

X -->|Sí| Y[Pedido especial al proveedor]
X -->|No| Z[Reposición normal]

Z --> F1[Fin]
Y --> F1
