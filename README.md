flowchart TD

A([Inicio del día]) --> B[Consulta 1: Revisar inventario de sabores]
B --> C{¿Hay stock mínimo?}

C -->|No| D[Pedido urgente al proveedor]
D --> B

C -->|Sí| E[Colocar baldes en vitrina]

E --> F[Consulta 2: Verificar envases en depósito]
F --> G{¿Hay envases suficientes?}

G -->|No| H[Reponer envases o pedir más]
H --> F

G -->|Sí| I[Comienza atención al público]

I --> J[[Boom del Pistacho]]

J --> K[Consulta 3: Verificar stock real de Pistacho]
K --> L{¿Alcanza el Pistacho?}

L -->|Sí| M[Reponer Pistacho y seguir]

L -->|No| N[Protocolo por escasez]

N --> O[Consulta 4: Revisar baldes reservados]
O --> P{¿Hay baldes extra?}

P -->|Sí| Q[Reponer con balde extra]
Q --> R[Continuar atención]

P -->|No| S[Consulta 5: Ver sabores sustitutos]

S --> T{¿Ofrecer sustituto?}

T -->|Sí| U[Sugerir sabores alternativos]
U --> R

T -->|No| V[Suspender venta de Pistacho]
V --> R

R --> W[Actualizar inventario del día]
W --> X{¿Pedir Pistacho urgente?}

X -->|Sí| Y[Pedido especial al proveedor]
X -->|No| Z[Reposición normal]

Y --> F1([Fin])
Z --> F1
