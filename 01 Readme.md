Integrantes:
Jhon Edward Ospina
Sebastián García
Diego Naranjo

# Helpdesk TI Socobuses – Entregables Taller:

Este repositorio contiene los diagramas solicitados (puntos 2 a 5).  
El punto 1 (Excel) se omite por acuerdo.

## Cómo visualizar
- En draw.io/diagrams.net: Insert > Advanced > Mermaid y pega el contenido de cada archivo .mmd.
- Alternativamente, abre los .mmd en cualquier visor Mermaid.

## Contenido
- 02_proceso_general.mmd – Proceso end-to-end.
- 02_1_as_is.mmd – Situación actual.
- 02_2_to_be.mmd – Proceso objetivo.
- 03_contexto.mmd – C4 Nivel Contexto.
- 04_contenedores.mmd – C4 Nivel Contenedores.
- 05_1_componentes_ticketing.mmd – Componentes: Ticketing.
- 05_2_componentes_auth.mmd – Componentes: Auth y seguridad.
- 05_3_componentes_cron_opcional.mmd – Componentes: CRON (opcional).

## Notas de arquitectura
- Backend: PHP MVC (Controllers: Auth, Ticket, KPI, Cron).
- Servicios: OpenAIService (prioridad), MailService (SMTP), SLAService (SLA y semáforos).
- Seguridad: Sesiones seguras, CSRF, XSS, caducidad de clave 30 días, bitácora de login.
- DB: MySQL con repositorios PDO y placeholders.
- Frontend: Bootstrap 5 + JS (AJAX). Dashboards con métricas SLA y satisfacción.


