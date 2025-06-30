# CEIA_IIA_TP1_HanoiTower

Repositorio del Trabajo Práctico N°1 de la materia "Introducción a la Inteligencia Artificial (IIA)", correspondiente a la Carrera de Especialización en Inteligencia Artificial (CEIA) de la Facultad de Ingeniería de la Universidad de Buenos Aires (FIUBA).



Disclaimer: Readme generado por IA (gpt-4o) y ajustado. 



## 🧠 Tema del TP

Implementación y análisis de algoritmos de búsqueda aplicados al clásico problema de la Torre de Hanoi. Se exploran distintas estrategias de búsqueda no informadas como:

- Búsqueda en anchura (Breadth-First Search - BFS)
- Búsqueda en profundidad (Depth-First Search - DFS)
- Búsqueda en profundidad limitada (Depth-Limited Search - DLS)



## 🧩 Estructura del repositorio

CEIA_IIA_TP1_HanoiTower/
├── aima_libs/                # Adaptaciones de las clases base de AIMA para modelado de problemas y nodos
├── hanoi_states.py          # Lógica de representación de estados y acciones del problema
├── hanoi_solver.py          # Implementaciones de los algoritmos de búsqueda aplicados al problema
├── utils/                   # Scripts auxiliares (simulador, visualización, etc.)
├── results/                 # Resultados obtenidos (métricas, secuencias de acciones, etc.)
├── initial_state.json       # Estado inicial exportado para simulador externo
├── sequence.json            # Secuencia de movimientos solucionadores
└── README.md                # Este archivo



## ⚙️ Requisitos

- Python 3.10+
- Librerías estándar (copy, json, etc.)
- Opcional: Jupyter Notebook para exploración interactiva



## 🚀 Ejecución

Desde consola:

    python hanoi_solver.py

También puede usarse desde un entorno interactivo para correr variantes parametrizadas:

    from hanoi_solver import hanoi_busqueda_profundidad_limitada_v2

    sol, metrics, _ = hanoi_busqueda_profundidad_limitada_v2(disks=5, limite=31)
    print(metrics)



## 📈 Métricas

Los algoritmos devuelven un diccionario de métricas al encontrar (o no) una solución, por ejemplo:

    {
        "solution_found": True,
        "states_visited": 1592,
        "nodes_in_frontier": 23,
        "solution_depth": 31,
        "cost_total": 31.0,
        "max_depth": 31
    }



## 👨‍🏫 Docente

- Cátedra: CEIA - Especialización en Inteligencia Artificial
- Materia: Introducción a la Inteligencia Artificial (IIA)
- Facultad de Ingeniería – Universidad de Buenos Aires (FIUBA)



## 📚 Créditos

Trabajo realizado por estudiantes del CEIA para el TP1 del curso IIA.
