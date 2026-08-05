# Breaklo

Sistema para la administración automatizada de filas de espera para breaks y lunches en equipos de soporte técnico.

---

# Tabla de Contenidos

- [Resumen Ejecutivo](#resumen-ejecutivo)
- [Requerimientos](#requerimientos)
- [Instalación](#instalación)
- [Configuración](#configuración)
- [Uso](#uso)
- [Contribución](#contribución)
- [Roadmap](#roadmap)

---

# Resumen Ejecutivo

## Descripción

Breaklo es una aplicación web desarrollada para automatizar la administración de los turnos de descanso dentro de equipos de soporte técnico. El sistema permite organizar las solicitudes de break de manera ordenada, reduciendo la coordinación manual entre los agentes y supervisores.

## Problema identificado

En el proceso actual, los agentes deben calcular cuándo dejarán de recibir nuevos chats, registrarse manualmente en una hoja de cálculo y coordinar el orden de salida con el resto del equipo. Este procedimiento consume tiempo, requiere comunicación constante y puede ocasionar errores en la administración de la fila.

## Solución

Breaklo centraliza la administración de las solicitudes de break mediante una plataforma web donde los agentes pueden solicitar su turno y consultar su posición en la fila. El sistema organiza automáticamente el orden de salida, permitiendo una gestión más eficiente y reduciendo la intervención manual.

## Arquitectura

El proyecto está desarrollado utilizando una arquitectura basada en el patrón Modelo-Vista-Controlador (MVC) mediante Spring Boot.

- **Modelo:** administra la información de usuarios, solicitudes y estados.
- **Vista:** interfaz web utilizada por agentes y administradores.
- **Controlador:** procesa las solicitudes del usuario y coordina la lógica del sistema.
- **Base de datos:** almacena la información de usuarios y solicitudes de break.

  ---

# Requerimientos

## Software requerido

Para ejecutar Breaklo es necesario contar con el siguiente software instalado:

| Componente | Versión recomendada |
|------------|---------------------|
| Java | JDK 21 |
| Maven | 3.9 o superior |
| Spring Boot | 4.1.0 |
| Git | Última versión |
| IntelliJ IDEA | Community o Ultimate |
| Navegador Web | Chrome, Edge o Firefox |

## Servidor de aplicación

Breaklo utiliza el servidor embebido Apache Tomcat proporcionado por Spring Boot, por lo que no es necesario instalar un servidor web adicional.

## Base de datos

Actualmente el proyecto utiliza una base de datos relacional para almacenar la información de usuarios y solicitudes de break. Durante el desarrollo puede utilizarse H2 Database y, para un ambiente de producción, PostgreSQL o MySQL.

## Dependencias principales

Las principales dependencias del proyecto son:

- Spring Boot Starter Web
- Spring Boot Starter Thymeleaf
- Spring Boot Starter Data JPA
- Spring Boot Starter Validation
- Base de datos H2
- Maven

## Hardware recomendado

- Procesador de dos núcleos o superior.
- 4 GB de memoria RAM como mínimo.
- 500 MB de espacio libre en disco.
- Conexión a Internet para descargar dependencias.
