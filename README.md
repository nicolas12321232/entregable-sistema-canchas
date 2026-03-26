# Sistema de Reservas de Canchas 🏟️

Este repositorio es un **Monorepo** que contiene los microservicios y el frontend para el sistema de gestión y reserva de canchas.

## 🏗️ Diagrama de Arquitectura

A continuación se muestra la arquitectura planificada de los microservicios:

```mermaid
graph TD
    Usuario((Usuario)) --> Frontend["ms-frontend (React/Vite)"]
    Frontend --> Auth["ms-usuarios-backend (Spring Boot)"]
    Frontend --> Reservas["ms-reservas-backend (Spring Boot)"]
    Auth --> DB1[(DB Usuarios)]
    Reservas --> DB2[(DB Canchas)]



