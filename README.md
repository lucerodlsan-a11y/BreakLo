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

| Componente | Requerimiento |
|------------|---------------|
| Lenguaje | Java 17 |
| Framework | Spring Boot 4.1.0 |
| Servidor web | Servidor embebido de Spring Boot |
| Gestor de dependencias | Maven |
| Base de datos | No implementada en la versión actual |

## Paquetes principales

- spring-boot-starter-webmvc
- spring-boot-starter-thymeleaf
- spring-boot-starter-webmvc-test
- spring-boot-starter-thymeleaf-test

  ---

# Instalación

## Configuración del ambiente de desarrollo

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/lucerodlsan-a11y/BreakLo.git
   ```

2. Abrir el proyecto en IntelliJ IDEA o Eclipse.

3. Verificar que esté instalado Java 17.

4. Ejecutar el proyecto utilizando Maven o directamente desde el IDE.

## Pruebas manuales

1. Iniciar la aplicación.
2. Abrir el navegador.
3. Acceder a `http://localhost:8080`.
4. Verificar el funcionamiento de las pantallas y funcionalidades implementadas.

## Despliegue

Actualmente Breaklo está diseñado para ejecutarse en un ambiente local mediante Spring Boot. En versiones futuras podrá desplegarse en servicios en la nube compatibles con aplicaciones Java.

---

# Configuración

La configuración principal del proyecto se encuentra en los siguientes archivos:

- `pom.xml`: administración de dependencias y configuración de Maven.
- `application.properties`: configuración general de la aplicación (cuando aplique).

No se requiere configuración adicional para ejecutar la versión actual del proyecto.

---

# Uso

## Usuario

El usuario puede:

- Acceder a la aplicación.
- Solicitar un turno para break.
- Consultar su posición en la fila.
- Marcar su regreso al finalizar el descanso.

## Administrador

El administrador puede:

- Visualizar la fila completa.
- Supervisar las solicitudes activas.
- Gestionar el estado de los usuarios.
- Administrar el flujo de turnos.

---

# Contribución

Para contribuir al proyecto:

1. Clonar el repositorio.
2. Crear una nueva rama.
   ```bash
   git checkout -b nombre-rama
   ```
3. Realizar los cambios necesarios.
4. Guardar los cambios mediante un commit.
   ```bash
   git commit -m "Descripción de los cambios"
   ```
5. Subir la rama al repositorio.
   ```bash
   git push origin nombre-rama
   ```
6. Crear un Pull Request.
7. Esperar la revisión y aprobación para realizar el merge.

---

# Roadmap

Las siguientes funcionalidades están contempladas para futuras versiones de Breaklo:

- Integración con una base de datos.
- Autenticación de usuarios mediante roles.
- Notificaciones automáticas para inicio y fin de break.
- Historial de solicitudes y reportes.
- Panel administrativo con estadísticas.
- Despliegue en un servicio en la nube.
