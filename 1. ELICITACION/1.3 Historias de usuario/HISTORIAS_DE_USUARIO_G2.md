# Historias de usuario — AgendaMed Renacer (Grupo 2, ADSW NRC 36839)

**Estado: BORRADOR para validar por el equipo.** Fecha: 09/11/2026 · Tarea Jira: G2-55 (Sprint 3, 16/11 a 20/11) · Carpeta destino del repo: `1. ELICITACION/1.3 Historias de usuario/`

## Para qué sirve este archivo

Es el entregable "Historias de usuario" de la Unidad de elicitación. Reúne las 39 Historias que ya existen en Jira (`G2-13` a `G2-51`), una por requisito funcional del SRS v4.0, con su texto "Como… quiero… para…" y los criterios de aceptación.

## Qué viene del SRS y qué es redacción nuestra

| Parte | Origen |
|---|---|
| ID, nombre, actor, prioridad MoSCoW | SRS v4.0 (§12.1), sin cambios |
| Criterios de aceptación (Gherkin) | Copiados del SRS v4.0, sin cambios |
| "Como… quiero…" | Redactado a partir del texto del requisito y su actor |
| **"para…"** | **Borrador nuestro**: el SRS describe qué hace el sistema pero casi nunca dice para qué. Se derivó de los problemas P-001 a P-010 del SRS §1.4 o, si no hay problema asociado, de un RNF. Cada historia indica en qué se apoya |

**Lo que hay que validar:** (1) que cada "para…" refleje la intención real del requisito; (2) las historias cuyo actor en el SRS es "Sistema" (RF-SIS-05, RF-PAG-03) o un proceso automático (RF-CIT-08), que aquí se redactaron desde el usuario beneficiado; (3) los cuatro hallazgos abiertos señalados abajo, que dependen de la errata del SRS (tarea G2-53).

**Pendiente de la docente:** si la rúbrica pide un formato concreto (por ejemplo INVEST) o criterios de estimación. No lo tengo.

## Problemas del SRS usados en los "para…" (§1.4)

| ID | Problema |
|---|---|
| P-001 | Cancelaciones tardías |
| P-002 | Ausentismo elevado |
| P-003 | Sobrecarga de la recepcionista |
| P-004 | Disponibilidad dinámica de médicos |
| P-005 | Atención sin cita previa (Sangolquí) |
| P-006 | Canal de WhatsApp bloqueado |
| P-007 | Sin reportes de gestión |
| P-009 | Pérdida de datos de pacientes |
| P-010 | Procesos manuales propensos a error |

P-008 (sin integración con historias clínicas) está fuera de alcance del SRS y no se usa.

## Índice

| Jira | RF | Nombre | Prioridad | Actor(es) según el SRS |
|---|---|---|---|---|
| G2-13 | RF-SIS-01 | Iniciar Sesión | Imprescindible | Usuario del Sistema |
| G2-14 | RF-SIS-02 | Cerrar Sesión | Debería tener | Usuario del Sistema |
| G2-15 | RF-SIS-03 | Restablecer Contraseña | Debería tener | Usuario del Sistema |
| G2-16 | RF-SIS-04 | Gestionar Usuarios | Imprescindible | Administrador |
| G2-17 | RF-SIS-05 | Validar Rol | Imprescindible | Sistema (incluido en Iniciar Sesión) |
| G2-18 | RF-SIS-06 | Consultar Auditoría | Debería tener | Administrador |
| G2-19 | RF-CFG-01 | Gestionar Sucursales | Imprescindible | Administrador |
| G2-20 | RF-CFG-02 | Gestionar Consultorios | Imprescindible | Administrador |
| G2-21 | RF-CFG-03 | Gestionar Especialidades | Imprescindible | Administrador |
| G2-22 | RF-CFG-04 | Gestionar Médicos | Imprescindible | Administrador |
| G2-23 | RF-CFG-05 | Configurar Horario Global | Debería tener | Administrador |
| G2-24 | RF-PAC-01 | Registrar Paciente | Imprescindible | Paciente, Recepcionista |
| G2-25 | RF-PAC-02 | Registrar Consentimiento de Datos | Imprescindible | Paciente (incluido en Registrar Paciente) |
| G2-26 | RF-PAC-03 | Modificar Datos de Paciente | Debería tener | Paciente, Recepcionista |
| G2-27 | RF-PAC-04 | Buscar Paciente | Imprescindible | Recepcionista, Médico |
| G2-28 | RF-PAC-05 | Consultar Historial de Citas | Debería tener | Paciente, Médico |
| G2-29 | RF-CIT-01 | Buscar Disponibilidad | Imprescindible | Paciente y Recepcionista (a través de los casos de uso que lo incluyen) |
| G2-30 | RF-CIT-02 | Pre-reservar Cita | Imprescindible | Paciente |
| G2-31 | RF-CIT-03 | Agendar Cita por Recepción | Imprescindible | Recepcionista |
| G2-32 | RF-CIT-04 | Agendar Walk-in | Debería tener | Recepcionista |
| G2-33 | RF-CIT-05 | Cancelar Cita | Imprescindible | Paciente, Recepcionista |
| G2-34 | RF-CIT-06 | Reprogramar Cita | Debería tener | Paciente, Recepcionista |
| G2-35 | RF-CIT-07 | Cancelar Cita por el Centro | Debería tener | Recepcionista |
| G2-36 | RF-CIT-08 | Recibir Recordatorio y Confirmar Asistencia | Imprescindible | Paciente |
| G2-37 | RF-PAG-01 | Pagar Cita en Línea | Imprescindible | Paciente |
| G2-38 | RF-PAG-02 | Procesar Pago en Caja | Imprescindible | Recepcionista |
| G2-39 | RF-PAG-03 | Generar Recibo | Imprescindible | Sistema (incluido en RF-PAG-01 y RF-PAG-02) |
| G2-40 | RF-PAG-04 | Registrar Reembolso | Debería tener | Administrador |
| G2-41 | RF-DIS-01 | Registrar Disponibilidad | Imprescindible | Médico |
| G2-42 | RF-DIS-02 | Modificar Disponibilidad | Imprescindible | Médico |
| G2-43 | RF-DIS-03 | Consultar Agenda del Día | Debería tener | Médico |
| G2-44 | RF-DIS-04 | Registrar Atención o Ausencia | Imprescindible | Médico (desde Consultar Agenda del Día) |
| G2-45 | RF-DIS-05 | Recibir Notificación de Cita | Debería tener | Médico |
| G2-46 | RF-REP-01 | Aplicar Filtros de Reporte | Debería tener | Administrador, Director General (desde los reportes que extiende) |
| G2-47 | RF-REP-02 | Reporte de Citas Confirmadas | Debería tener | Administrador, Director General |
| G2-48 | RF-REP-03 | Reporte de Ausentismo | Debería tener | Administrador, Director General |
| G2-49 | RF-REP-04 | Reporte de Cancelaciones | Debería tener | Administrador, Director General |
| G2-50 | RF-REP-05 | Reporte de Ingresos | Debería tener | Administrador, Director General |
| G2-51 | RF-REP-06 | Exportar Reporte | Debería tener | Administrador, Director General |

---

## Módulo SIS · Administrar Sistema (Epic G2-1)

### RF-SIS-01 — Iniciar Sesión (G2-13)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Usuario del Sistema  
- **Historia (borrador):** Como usuario registrado (Paciente, Recepcionista, Médico, Administrador o Director General), quiero iniciar sesión con mi correo y mi contraseña, para entrar solo al panel que corresponde a mi rol.  
- **En qué se apoya el "para…":** RNF-10 y RNF-11 (control de acceso y seguridad de credenciales); no hay un problema P-xxx directo.  
- **Relación en el SRS:** Incluye (<<include>>) RF-SIS-05 Validar Rol. Es extendido por RF-SIS-03 Restablecer Contraseña.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado que el usuario ingresa un correo y una contraseña correctos, cuando envía el formulario, entonces el sistema lo redirige al panel de su rol en un máximo de 2 segundos.
  - CA-02 Dado que el usuario ingresa credenciales incorrectas, cuando envía el formulario, entonces el sistema muestra 'Correo o contraseña incorrectos' sin indicar cuál de los dos campos falló.
  - CA-03 Dado que el usuario acumula 3 intentos fallidos consecutivos, cuando confirma el tercer intento, entonces el sistema bloquea la cuenta durante 15 minutos, envía un correo de aviso e impide el inicio de sesión aunque las credenciales posteriores sean correctas.
  - CA-04 Dado una cuenta bloqueada temporalmente, cuando transcurren los 15 minutos, entonces el sistema permite nuevamente el intento de inicio de sesión.
  - CA-05 Dado una cuenta que registra su cuarto bloqueo dentro de 24 horas, cuando se produce el bloqueo, entonces el sistema la mantiene bloqueada y muestra 'Cuenta bloqueada. Contacte al administrador' hasta su desbloqueo manual.
  - CA-06 Dado una cuenta inactiva, cuando su titular intenta iniciar sesión con credenciales correctas, entonces el sistema rechaza el acceso.

### RF-SIS-02 — Cerrar Sesión (G2-14)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Usuario del Sistema  
- **Historia (borrador):** Como usuario autenticado, quiero cerrar mi sesión, o que se cierre sola por inactividad sin perder lo que estaba escribiendo, para que nadie use mi cuenta desde un equipo compartido.  
- **En qué se apoya el "para…":** RNF-11 (seguridad de sesión); no hay un problema P-xxx directo.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un usuario autenticado, cuando selecciona 'Cerrar Sesión', entonces el sistema invalida el token, elimina la cookie y lo redirige a la pantalla de inicio de sesión.
  - CA-02 Dado un usuario sin actividad durante 13 minutos, cuando se cumple ese lapso, entonces el sistema muestra la advertencia de cierre con la opción 'Continuar'.
  - CA-03 Dado que el usuario selecciona 'Continuar' en la advertencia, cuando confirma, entonces el sistema reinicia el contador de inactividad.
  - CA-04 Dado un usuario sin actividad durante 15 minutos, cuando se cumple ese lapso, entonces el sistema cierra la sesión automáticamente.
  - CA-05 Dado un formulario en curso al momento del cierre automático, cuando el mismo usuario vuelve a iniciar sesión, entonces el sistema le ofrece recuperar el borrador guardado.

### RF-SIS-03 — Restablecer Contraseña (G2-15)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Usuario del Sistema  
- **Historia (borrador):** Como usuario que olvidó su contraseña, quiero recibir en mi correo un enlace para definir una contraseña nueva, para recuperar mi acceso sin depender de otra persona.  
- **En qué se apoya el "para…":** RNF-11; no hay un problema P-xxx directo.  
- **Relación en el SRS:** Extiende (<<extend>>) RF-SIS-01 Iniciar Sesión.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado que un usuario solicita el restablecimiento con un correo registrado, cuando confirma la solicitud, entonces el sistema envía el enlace en un máximo de 1 minuto.
  - CA-02 Dado que se solicita el restablecimiento con un correo no registrado, cuando se confirma la solicitud, entonces el sistema muestra el mismo mensaje genérico y no envía ningún correo.
  - CA-03 Dado un enlace generado hace más de 1 hora o ya utilizado, cuando el usuario lo abre, entonces el sistema muestra 'El enlace ha expirado, solicite uno nuevo' y no permite el cambio.
  - CA-04 Dado un enlace vigente, cuando el usuario define una contraseña que cumple la política de RF-SIS-01, entonces el sistema la actualiza, cierra las sesiones activas y envía un correo de confirmación.

### RF-SIS-04 — Gestionar Usuarios (G2-16)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero registrar, modificar, inactivar y desbloquear las cuentas del personal asignando un único rol a cada una, para controlar quién entra al sistema y con qué permisos.  
- **En qué se apoya el "para…":** RNF-10 y RNF-12; no hay un problema P-xxx directo.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado el formulario de registro de usuario, cuando falta algún campo obligatorio, entonces el sistema rechaza el registro señalando el campo faltante.
  - CA-02 Dado un correo electrónico ya registrado por otra cuenta, cuando se intenta guardar, entonces el sistema rechaza el registro mostrando 'Correo ya registrado'.
  - CA-03 Dado un registro con datos válidos y un rol asignado, cuando se guarda, entonces el sistema crea la cuenta y envía la contraseña temporal al correo del usuario.
  - CA-04 Dado un usuario con contraseña temporal, cuando inicia sesión por primera vez, entonces el sistema le exige definir una nueva contraseña antes de continuar.
  - CA-05 Dado un usuario activo, cuando el Administrador lo inactiva, entonces el sistema impide su inicio de sesión sin eliminar su historial.
  - CA-06 Dado una cuenta bloqueada, cuando el Administrador la desbloquea sin registrar la observación de verificación, entonces el sistema rechaza la acción.
  - CA-07 Dado que solo existe un Administrador activo, cuando se intenta inactivar su cuenta, entonces el sistema rechaza la acción.

### RF-SIS-05 — Validar Rol (G2-17)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Sistema (incluido en Iniciar Sesión)  
- **Historia (borrador):** Como usuario autenticado, quiero que el sistema habilite solo los módulos y operaciones de mi rol, para que no se expongan datos ni acciones que no me corresponden (por ejemplo, datos de pago al Médico).  
- **En qué se apoya el "para…":** RNF-10. El SRS define como actor al "Sistema (incluido en Iniciar Sesión)"; aquí se redacta desde el usuario que se beneficia.  
- **Relación en el SRS:** Caso de uso incluido por RF-SIS-01. Detalla a nivel funcional el mismo mecanismo especificado como atributo de calidad en RNF-10; ambos deben mantenerse consistentes.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un usuario con rol Paciente, cuando inicia sesión, entonces el sistema habilita únicamente su portal con sus propios datos y citas.
  - CA-02 Dado un usuario con rol Recepcionista, cuando inicia sesión, entonces el sistema habilita Gestionar Pacientes, Gestionar Citas y Procesar Pago en Caja.
  - CA-03 Dado un usuario con rol Médico, cuando inicia sesión, entonces el sistema habilita su disponibilidad, su agenda y la búsqueda e historial de sus pacientes, sin datos de pago.
  - CA-04 Dado un usuario con rol Administrador, cuando inicia sesión, entonces el sistema habilita Administrar Sistema, Configurar Clínica, Registrar Reembolso y Generar Reportes.
  - CA-05 Dado un usuario con rol Director General, cuando inicia sesión, entonces el sistema habilita únicamente Generar Reportes.
  - CA-06 Dado cualquier usuario autenticado, cuando intenta acceder a un módulo no autorizado para su rol, entonces el sistema rechaza el acceso mostrando 'No tiene permisos para acceder a este módulo' y registra el intento en la auditoría.

### RF-SIS-06 — Consultar Auditoría (G2-18)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero consultar la bitácora de inicios de sesión, intentos fallidos y operaciones críticas, para saber quién hizo qué y cuándo.  
- **En qué se apoya el "para…":** RNF-13 (trazabilidad y auditoría).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado el Administrador en la bitácora, cuando aplica filtros combinados de usuario, acción, resultado y rango de fechas, entonces el sistema muestra solo los registros que cumplen todos los criterios en un máximo de 3 segundos.
  - CA-02 Dado un rango de fechas con fecha inicio posterior a la fecha fin, cuando se aplica el filtro, entonces el sistema rechaza la búsqueda indicando rango inválido.
  - CA-03 Dado un registro de auditoría, cuando cualquier usuario intenta modificarlo o eliminarlo, entonces el sistema no ofrece ni permite esa operación.

---

## Módulo CFG · Configurar Clínica (Epic G2-2)

### RF-CFG-01 — Gestionar Sucursales (G2-19)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero registrar, modificar e inactivar las sucursales de la clínica, para que Matriz Sur, La Arcadia y Sangolquí queden disponibles para consultorios, médicos y búsqueda de citas.  
- **En qué se apoya el "para…":** P-003 (hoy la gestión depende de una sola recepción en Matriz Sur).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado el formulario de sucursal, cuando el nombre ya existe o está fuera del rango de 3 a 50 caracteres, entonces el sistema rechaza el registro.
  - CA-02 Dado un teléfono que no tiene 9 o 10 dígitos o no inicia en 0, cuando se intenta guardar, entonces el sistema rechaza el registro indicando formato inválido.
  - CA-03 Dado una sucursal con citas futuras, cuando se intenta inactivar, entonces el sistema bloquea la acción mostrando el mensaje de reasignación.
  - CA-04 Dado una sucursal con datos válidos, cuando se guarda, entonces el sistema la registra y queda disponible para consultorios, médicos y búsqueda de disponibilidad.

### RF-CFG-02 — Gestionar Consultorios (G2-20)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero registrar y mantener los consultorios de cada sucursal, para evitar que dos médicos ocupen el mismo consultorio al mismo tiempo.  
- **En qué se apoya el "para…":** P-004 (gestión de horarios de médicos); lo usa RF-DIS-01.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un código que no cumple la máscara CON-NN o que ya existe en la misma sucursal, cuando se intenta guardar, entonces el sistema rechaza el registro.
  - CA-02 Dado un consultorio con bloques de disponibilidad futuros, cuando se intenta inactivar, entonces el sistema bloquea la acción mostrando 'El consultorio tiene disponibilidad asignada'.
  - CA-03 Dado un código válido y único para una sucursal activa, cuando se guarda, entonces el sistema registra el consultorio.

### RF-CFG-03 — Gestionar Especialidades (G2-21)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero registrar las especialidades con su duración de cita y su tarifa base, para que la agenda y el cobro usen datos consistentes.  
- **En qué se apoya el "para…":** P-010 (procesos manuales propensos a error); lo usan RF-PAG-01 y RF-PAG-02.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un nombre de especialidad duplicado o fuera del rango de 3 a 50 caracteres, cuando se intenta guardar, entonces el sistema rechaza el registro.
  - CA-02 Dado una tarifa menor o igual a 0 o con más de 2 decimales, cuando se intenta guardar, entonces el sistema rechaza el registro.
  - CA-03 Dado una especialidad con citas existentes, cuando el Administrador modifica su tarifa, entonces las citas existentes conservan el monto original y las nuevas usan la tarifa actualizada.
  - CA-04 Dado una especialidad con citas futuras, cuando se intenta inactivar, entonces el sistema bloquea la acción.

### RF-CFG-04 — Gestionar Médicos (G2-22)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero registrar a los médicos con las especialidades que atienden y las sucursales donde trabajan, para que cada médico pueda publicar su disponibilidad y recibir citas.  
- **En qué se apoya el "para…":** P-004 (disponibilidad dinámica de médicos).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado el formulario de médico, cuando falta algún campo obligatorio o no se asigna al menos una especialidad y una sucursal, entonces el sistema rechaza el registro.
  - CA-02 Dado una cédula que no supera la validación módulo 10 o ya pertenece a otro médico, cuando se intenta guardar, entonces el sistema rechaza el registro.
  - CA-03 Dado un médico con datos válidos, cuando se guarda, entonces el sistema lo registra y crea su cuenta con rol Médico.
  - CA-04 Dado un médico con citas futuras en una especialidad, cuando se intenta retirar esa especialidad, entonces el sistema bloquea el cambio mostrando el mensaje de reasignación.

### RF-CFG-05 — Configurar Horario Global (G2-23)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero definir el horario global de atención y registrar excepciones como feriados o cierres, para que ningún bloque de disponibilidad ni cita quede fuera del horario de la clínica.  
- **En qué se apoya el "para…":** P-004 y P-010.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un día marcado como abierto, cuando la hora de inicio es mayor o igual a la hora de fin, entonces el sistema rechaza el cambio.
  - CA-02 Dado una excepción en una fecha con citas reservadas, cuando se intenta guardar, entonces el sistema muestra las citas afectadas y no guarda la excepción.
  - CA-03 Dado un horario válido sin citas afectadas, cuando se guarda, entonces el sistema lo aplica a la búsqueda de disponibilidad y a la validación de bloques de RF-DIS-01.

---

## Módulo PAC · Gestionar Pacientes (Epic G2-3)

### RF-PAC-01 — Registrar Paciente (G2-24)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Paciente, Recepcionista  
- **Historia (borrador):** Como paciente (o Recepcionista a solicitud del paciente), quiero registrar mis datos una sola vez, para poder agendar citas y que mis datos no se pierdan.  
- **En qué se apoya el "para…":** P-009 (pérdida de datos de pacientes).  
- **Relación en el SRS:** Incluye (<<include>>) RF-PAC-02 Registrar Consentimiento de Datos.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cédula que no tiene 10 dígitos o no supera la validación módulo 10, cuando se intenta guardar, entonces el sistema rechaza el registro mostrando 'Cédula inválida'.
  - CA-02 Dado una cédula ya registrada, cuando se intenta guardar, entonces el sistema rechaza el registro mostrando 'Paciente ya registrado'.
  - CA-03 Dado un correo con formato inválido o ya registrado, o un celular que no cumple la máscara 09XXXXXXXX, cuando se intenta guardar, entonces el sistema rechaza el registro indicando el campo inválido.
  - CA-04 Dado un autorregistro de una persona menor de 18 años, cuando se intenta guardar, entonces el sistema rechaza el registro e indica que debe acercarse a Recepción.
  - CA-05 Dado un formulario válido sin el consentimiento aceptado, cuando se intenta guardar, entonces el sistema no completa el registro.
  - CA-06 Dado un registro válido realizado por la Recepcionista, cuando se guarda, entonces el sistema crea al paciente y envía el enlace de activación a su correo.

### RF-PAC-02 — Registrar Consentimiento de Datos (G2-25)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Paciente (incluido en Registrar Paciente)  
- **Historia (borrador):** Como paciente, quiero aceptar o revocar de forma explícita el tratamiento de mis datos personales, para que mi información se use conforme a la LOPDP.  
- **En qué se apoya el "para…":** RNF-12 (protección de datos personales); no hay un problema P-xxx directo.  
- **Relación en el SRS:** Caso de uso incluido por RF-PAC-01.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado el formulario de registro, cuando se muestra la casilla de consentimiento, entonces esta aparece sin marcar.
  - CA-02 Dado que el paciente acepta el consentimiento, cuando se completa el registro, entonces el sistema guarda fecha, hora, versión del texto y canal.
  - CA-03 Dado una nueva versión del texto de tratamiento, cuando el paciente inicia sesión, entonces el sistema le solicita aceptarla antes de continuar.
  - CA-04 Dado un paciente con citas futuras, cuando intenta revocar el consentimiento, entonces el sistema le indica que debe cancelarlas antes de continuar.
  - CA-05 Dado un paciente sin citas futuras, cuando revoca el consentimiento, entonces el sistema inactiva su cuenta e inicia la supresión de sus datos personales.

### RF-PAC-03 — Modificar Datos de Paciente (G2-26)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Paciente, Recepcionista  
- **Historia (borrador):** Como paciente o Recepcionista, quiero actualizar los datos del paciente (el paciente su contacto; la Recepcionista también su identificación), para que los recordatorios y avisos lleguen al contacto correcto.  
- **En qué se apoya el "para…":** P-002 (ausentismo) y P-009.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un paciente existente, cuando se intenta editar el campo cédula, entonces el sistema no permite su modificación.
  - CA-02 Dado un paciente que cambia su correo, cuando guarda, entonces el sistema envía un enlace de confirmación al nuevo correo y mantiene el correo anterior hasta que se confirme.
  - CA-03 Dado un usuario con rol Paciente, cuando intenta modificar sus nombres o su fecha de nacimiento, entonces el sistema no habilita esos campos.
  - CA-04 Dado datos válidos, cuando se guardan, entonces el sistema actualiza al paciente y registra el cambio en la auditoría.

### RF-PAC-04 — Buscar Paciente (G2-27)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Recepcionista, Médico  
- **Historia (borrador):** Como Recepcionista o Médico, quiero buscar pacientes registrados por cédula o por nombre, para agendar, cobrar o consultar sin duplicar registros ni depender de papel.  
- **En qué se apoya el "para…":** P-003 y P-010. Es precondición de RF-CIT-03, RF-CIT-04 y RF-PAG-02.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cédula registrada, cuando la Recepcionista busca por cédula, entonces el sistema muestra exactamente ese paciente en un máximo de 3 segundos.
  - CA-02 Dado un texto de al menos 3 caracteres, cuando se busca por nombre, entonces el sistema muestra los pacientes cuyo nombre o apellido lo contiene.
  - CA-03 Dado un usuario con rol Médico, cuando busca un paciente que nunca tuvo cita con él, entonces el sistema no lo muestra en los resultados.
  - CA-04 Dado una búsqueda sin resultados realizada por la Recepcionista, cuando se ejecuta, entonces el sistema muestra 'No se encontraron pacientes' y ofrece registrar uno nuevo.
- **Observación:** Hallazgo abierto (ver tarea G2-53): el texto del RF menciona búsqueda por correo o celular, pero ningún CA define si es exacta o parcial; "100 resultados por página" no tiene CA.

### RF-PAC-05 — Consultar Historial de Citas (G2-28)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Paciente, Médico  
- **Historia (borrador):** Como paciente (o Médico tratante), quiero ver el historial administrativo de mis citas, para saber qué cité, cancelé o atendí sin llamar a recepción.  
- **En qué se apoya el "para…":** P-003 (sobrecarga de la recepcionista).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un paciente autenticado, cuando abre 'Mis Citas', entonces el sistema muestra únicamente sus citas ordenadas por fecha descendente.
  - CA-02 Dado una cita próxima que inicia en menos de 4 horas, cuando el paciente la visualiza, entonces el sistema no habilita las opciones Cancelar ni Reprogramar.
  - CA-03 Dado un médico que consulta el historial de un paciente suyo, cuando se muestra, entonces no se incluye ningún dato de pago ni información clínica.
- **Observación:** Hallazgo abierto (ver tarea G2-53): el CA-02 dice "menos de 4 horas" y el texto del RF "más de 4 horas"; no hay CA para exactamente 4 horas, ni CA de filtros ni de descarga de recibos.

---

## Módulo CIT · Gestionar Citas (Epic G2-4)

### RF-CIT-01 — Buscar Disponibilidad (G2-29)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Paciente y Recepcionista (a través de los casos de uso que lo incluyen)  
- **Historia (borrador):** Como paciente o Recepcionista, quiero buscar horarios libres por sucursal, especialidad, tipo de visita, médico, fecha y hora, para elegir una cita sin pasar por llamadas ni listas manuales.  
- **En qué se apoya el "para…":** P-003 y P-004.  
- **Relación en el SRS:** Caso de uso incluido por RF-CIT-02, RF-CIT-03 y RF-CIT- 06.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un paciente en la búsqueda, cuando no ha seleccionado sucursal, entonces el sistema no habilita la selección de especialidad.
  - CA-02 Dado una sucursal, especialidad y tipo de visita seleccionados, cuando se ejecuta la búsqueda, entonces el sistema muestra en un máximo de 2 segundos solo slots libres dentro del horario global y de los bloques del médico.
  - CA-03 Dado un slot con una pre-reserva vigente de otro paciente, cuando se ejecuta la búsqueda, entonces ese slot no aparece como disponible.
  - CA-04 Dado la búsqueda en el portal del paciente, cuando se muestran los resultados, entonces no aparece ningún slot que inicie en menos de 2 horas.

### RF-CIT-02 — Pre-reservar Cita (G2-30)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Paciente  
- **Historia (borrador):** Como paciente, quiero reservar temporalmente un horario y elegir si pago en línea o en caja, para asegurar mi cupo mientras completo el pago, sin dobles reservas.  
- **En qué se apoya el "para…":** P-003 y RNF-04 (cero dobles reservas).  
- **Relación en el SRS:** Incluye (<<include>>) RF-CIT-01 Buscar Disponibilidad.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un paciente autenticado, cuando selecciona un slot disponible, entonces el sistema lo bloquea durante exactamente 10 minutos y muestra el tiempo restante.
  - CA-02 Dado dos pacientes que seleccionan el mismo slot simultáneamente, cuando se procesan las solicitudes, entonces solo uno obtiene la pre-reserva y el otro recibe 'El horario seleccionado ya no está disponible'.
  - CA-03 Dado una pre-reserva vigente, cuando el paciente elige 'Pagar en caja', entonces la cita pasa a PENDIENTE_PAGO y el sistema le notifica que debe confirmar asistencia y pagar antes de la atención.
  - CA-04 Dado una pre-reserva sin acción durante 10 minutos, cuando vence el plazo, entonces el sistema libera el slot y la pre-reserva pasa a EXPIRADA.
  - CA-05 Dado un paciente con 2 citas futuras en PENDIENTE_PAGO, cuando intenta pre-reservar otra con pago en caja, entonces el sistema solo le permite la opción 'Pagar en línea'.

### RF-CIT-03 — Agendar Cita por Recepción (G2-31)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Recepcionista  
- **Historia (borrador):** Como Recepcionista, quiero agendar citas para cualquier paciente registrado, en cualquier sucursal, por teléfono o en persona, para atender a quien no usa el portal sin ser el cuello de botella.  
- **En qué se apoya el "para…":** P-003 (sobrecarga de la recepcionista, crítico).  
- **Relación en el SRS:** Incluye (<<include>>) RF-CIT-01 Buscar Disponibilidad.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un paciente registrado y un slot disponible, cuando la Recepcionista agenda la cita, entonces el sistema la crea en PENDIENTE_PAGO con la anotación 'Agendada por: Recepcionista [nombre]'.
  - CA-02 Dado una cita agendada por Recepción, cuando se guarda, entonces el sistema envía al paciente un correo y un SMS con los datos de la cita.
  - CA-03 Dado una cita agendada que inicia en menos de 2 horas, cuando se guarda, entonces el sistema la registra con asistencia confirmada.
  - CA-04 Dado que el slot fue tomado por otro usuario segundos antes, cuando la Recepcionista intenta guardar, entonces el sistema rechaza la operación mostrando 'El horario seleccionado ya no está disponible'.

### RF-CIT-04 — Agendar Walk-in (G2-32)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Recepcionista  
- **Historia (borrador):** Como Recepcionista, quiero agendar de inmediato a quien llega sin cita en las sucursales habilitadas, para atender la demanda espontánea del sector.  
- **En qué se apoya el "para…":** P-005 (atención sin cita previa, Sangolquí).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una sucursal sin el indicador 'Atiende walk-in', cuando la Recepcionista intenta agendar un walk-in, entonces el sistema no habilita la opción.
  - CA-02 Dado una fecha distinta al día en curso, cuando se intenta agendar un walk-in, entonces el sistema rechaza la operación.
  - CA-03 Dado un paciente registrado y un slot libre hoy, cuando la Recepcionista registra el walk-in y el pago, entonces la cita queda CONFIRMADA y el médico recibe la notificación.

### RF-CIT-05 — Cancelar Cita (G2-33)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Paciente, Recepcionista  
- **Historia (borrador):** Como paciente (o Recepcionista a solicitud del paciente), quiero cancelar una cita con la anticipación mínima, para liberar el cupo de inmediato y reducir las cancelaciones de último minuto.  
- **En qué se apoya el "para…":** P-001 (cancelaciones tardías).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cita CONFIRMADA que inicia en más de 4 horas, cuando el paciente la cancela indicando un motivo, entonces la cita pasa a CANCELADA y el cupo aparece disponible de inmediato.
  - CA-02 Dado una cita que inicia en 4 horas o menos, cuando se intenta cancelar, entonces el sistema rechaza la acción mostrando 'La cita no puede cancelarse con menos de 4 horas de anticipación'.
  - CA-03 Dado una cancelación sin motivo seleccionado, cuando se intenta confirmar, entonces el sistema rechaza la acción.
  - CA-04 Dado una cita pagada que se cancela dentro del plazo, cuando se confirma la cancelación, entonces el sistema genera una solicitud de reembolso del 100% del pago.

### RF-CIT-06 — Reprogramar Cita (G2-34)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Paciente, Recepcionista  
- **Historia (borrador):** Como paciente o Recepcionista, quiero cambiar fecha, hora, médico o sucursal de una cita conservando su estado y su pago, para no perder la cita ni el dinero al reagendar.  
- **En qué se apoya el "para…":** P-001 (cancelaciones tardías).  
- **Relación en el SRS:** Incluye (<<include>>) RF-CIT-01 Buscar Disponibilidad.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cita que inicia en más de 4 horas y un nuevo slot libre de la misma especialidad, cuando se confirma la reprogramación, entonces el sistema asigna el nuevo slot, libera el anterior y conserva el estado y el pago.
  - CA-02 Dado que el nuevo slot fue tomado por otro usuario, cuando se confirma la reprogramación, entonces el sistema la rechaza y la cita original permanece sin cambios.
  - CA-03 Dado una cita reprogramada 2 veces por el paciente, cuando intenta una tercera reprogramación, entonces el sistema rechaza la acción.

### RF-CIT-07 — Cancelar Cita por el Centro (G2-35)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Recepcionista  
- **Historia (borrador):** Como Recepcionista, quiero cancelar citas por causas de la clínica, incluso todas las de un médico en una fecha en una sola operación, para avisar y devolver el pago sin hacerlo cita por cita.  
- **En qué se apoya el "para…":** P-004 y P-010.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cita que inicia en menos de 4 horas, cuando la Recepcionista la cancela por el centro indicando el motivo, entonces la cita pasa a CANCELADA_CENTRO.
  - CA-02 Dado un médico con varias citas en una fecha, cuando la Recepcionista las cancela en una sola operación, entonces todas pasan a CANCELADA_CENTRO.
  - CA-03 Dado una cita pagada cancelada por el centro, cuando se confirma la acción, entonces el sistema genera la solicitud de reembolso del 100% y notifica al paciente en un máximo de 5 minutos.

### RF-CIT-08 — Recibir Recordatorio y Confirmar Asistencia (G2-36)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Paciente  
- **Historia (borrador):** Como paciente, quiero recibir recordatorios 24 h y 4 h antes y confirmar mi asistencia con un enlace, para no olvidar la cita y que la clínica libere el cupo si no confirmo.  
- **En qué se apoya el "para…":** P-002 (ausentismo) y P-006 (WhatsApp bloqueado: se usan correo y SMS). El SRS lo define como proceso automático.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cita programada, cuando faltan 24 horas (±10 minutos) para su inicio, entonces el sistema envía el recordatorio por correo y SMS con el enlace de confirmación.
  - CA-02 Dado una cita programada, cuando faltan 4 horas (±10 minutos), entonces el sistema envía el segundo recordatorio.
  - CA-03 Dado que el paciente usa el enlace 'Confirmar asistencia', cuando lo abre antes del inicio de la cita, entonces el sistema registra la confirmación con fecha y hora.
  - CA-04 Dado una cita en PENDIENTE_PAGO sin confirmación, cuando faltan 2 horas para su inicio, entonces el sistema la cancela automáticamente, libera el cupo y notifica al paciente.
  - CA-05 Dado una cita CONFIRMADA sin confirmación, cuando faltan 2 horas para su inicio, entonces el sistema la mantiene y muestra la alerta a la Recepcionista y al médico.

---

## Módulo PAG · Gestionar Pagos (Epic G2-5)

### RF-PAG-01 — Pagar Cita en Línea (G2-37)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Paciente  
- **Historia (borrador):** Como paciente, quiero pagar mi cita con tarjeta mediante una pasarela certificada PCI DSS, para confirmar mi cupo sin ir a caja.  
- **En qué se apoya el "para…":** P-003; el pago hoy es solo presencial.  
- **Relación en el SRS:** Incluye (<<include>>) RF-PAG-03 Generar Recibo.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una pre-reserva vigente, cuando el paciente paga y la pasarela aprueba la transacción, entonces la cita pasa a CONFIRMADA y el sistema genera el recibo.
  - CA-02 Dado un pago rechazado con la pre-reserva aún vigente, cuando se recibe la respuesta, entonces el sistema muestra el motivo y permite reintentar con otra tarjeta.
  - CA-03 Dado un pago rechazado con la pre-reserva expirada, cuando el paciente intenta reintentar, entonces el sistema muestra 'La pre-reserva expiró; seleccione un nuevo horario'.
  - CA-04 Dado una cita con un pago aprobado, cuando se intenta un segundo pago para la misma cita, entonces el sistema lo rechaza.
  - CA-05 Dado un pago registrado, cuando se inspecciona la base de datos, entonces no existe ningún número completo de tarjeta almacenado.

### RF-PAG-02 — Procesar Pago en Caja (G2-38)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Recepcionista  
- **Historia (borrador):** Como Recepcionista, quiero registrar el pago presencial de una cita pendiente, para confirmar la cita y cerrar el cobro con comprobante.  
- **En qué se apoya el "para…":** P-010 (procesos manuales propensos a error).  
- **Relación en el SRS:** Incluye (<<include>>) RF-PAG-03 Generar Recibo.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un paciente con citas en PENDIENTE_PAGO, cuando la Recepcionista busca por su cédula, entonces el sistema muestra solo esas citas.
  - CA-02 Dado un pago en efectivo con monto recibido menor al monto de la cita, cuando se intenta registrar, entonces el sistema lo rechaza.
  - CA-03 Dado un pago con tarjeta sin número de voucher, o una transferencia sin número de comprobante, cuando se intenta registrar, entonces el sistema lo rechaza indicando el campo faltante.
  - CA-04 Dado un pago válido, cuando se registra, entonces la cita pasa a CONFIRMADA y deja de aparecer como pendiente de pago.

### RF-PAG-03 — Generar Recibo (G2-39)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Sistema (incluido en RF-PAG-01 y RF-PAG-02)  
- **Historia (borrador):** Como paciente, quiero recibir por correo un recibo con número único y código QR, para tener un comprobante de mi pago (no reemplaza la factura electrónica del SRI).  
- **En qué se apoya el "para…":** P-010. El SRS define como actor al "Sistema (incluido en RF-PAG-01 y RF-PAG-02)".  
- **Relación en el SRS:** Caso de uso incluido por RF-PAG-01 y RF-PAG-02.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un pago aprobado o registrado, cuando se confirma, entonces el sistema genera un recibo con un número REC-AAAA-NNNNNN que no se repite.
  - CA-02 Dado un recibo generado, cuando se envía, entonces llega al correo del paciente en un máximo de 5 segundos.
  - CA-03 Dado el código QR de un recibo, cuando se escanea, entonces abre la página de verificación con los datos del recibo.

### RF-PAG-04 — Registrar Reembolso (G2-40)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador  
- **Historia (borrador):** Como Administrador, quiero procesar las solicitudes de reembolso que generan las cancelaciones, para devolver el 100 % del pago sin duplicados ni errores manuales.  
- **En qué se apoya el "para…":** P-010 (procesos manuales propensos a error).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una solicitud de reembolso PENDIENTE, cuando el Administrador la procesa, entonces el sistema registra el reembolso por el 100% del pago original y la marca como REEMBOLSADO.
  - CA-02 Dado un pago ya reembolsado, cuando se intenta reembolsar de nuevo, entonces el sistema rechaza la acción.
  - CA-03 Dado una cita en estado AUSENTE o ATENDIDA, cuando se intenta generar un reembolso, entonces el sistema rechaza la acción.

---

## Módulo DIS · Gestionar Disponibilidad (Epic G2-6)

### RF-DIS-01 — Registrar Disponibilidad (G2-41)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Médico  
- **Historia (borrador):** Como Médico, quiero registrar mis bloques de disponibilidad, validados contra el horario global y los consultorios, para que los pacientes solo vean horarios reales.  
- **En qué se apoya el "para…":** P-004 (disponibilidad dinámica de médicos).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un bloque fuera del horario global o en una fecha de excepción, cuando se intenta guardar, entonces el sistema lo rechaza.
  - CA-02 Dado un consultorio ocupado por otro médico en el mismo horario, cuando se intenta guardar el bloque, entonces el sistema lo rechaza mostrando 'El consultorio ya está asignado en ese horario'.
  - CA-03 Dado un bloque que se cruza con otro bloque del mismo médico, cuando se intenta guardar, entonces el sistema lo rechaza.
  - CA-04 Dado un bloque válido, cuando se guarda, entonces sus slots aparecen en la búsqueda de disponibilidad en un máximo de 2 segundos.

### RF-DIS-02 — Modificar Disponibilidad (G2-42)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Médico  
- **Historia (borrador):** Como Médico, quiero modificar o eliminar mis bloques futuros sin afectar las citas ya reservadas, para ajustar mi agenda cuando cambian mis rotativas.  
- **En qué se apoya el "para…":** P-004 (disponibilidad dinámica de médicos).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un bloque sin citas, cuando el médico lo elimina, entonces sus slots desaparecen de la búsqueda en un máximo de 2 segundos.
  - CA-02 Dado un bloque con al menos una cita reservada, cuando el médico intenta eliminarlo o reducirlo, entonces el sistema bloquea la acción mostrando el mensaje de reasignación.
  - CA-03 Dado una modificación de disponibilidad, cuando se guarda, entonces se registra en la auditoría con los valores anterior y nuevo.

### RF-DIS-03 — Consultar Agenda del Día (G2-43)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Médico  
- **Historia (borrador):** Como Médico, quiero ver mis citas del día y las de los próximos 30 días, para preparar mi atención sin depender de la recepción.  
- **En qué se apoya el "para…":** P-003.  
- **Relación en el SRS:** Es extendido por (<<extend>>) RF-DIS-04 Registrar Atención o Ausencia.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un médico autenticado, cuando abre su agenda, entonces el sistema muestra solo sus citas del día ordenadas por hora.
  - CA-02 Dado una cita sin asistencia confirmada a 2 horas de su inicio, cuando se muestra la agenda, entonces la cita aparece con la alerta visual.
  - CA-03 Dado que se agenda una cita nueva para el médico, cuando tiene la agenda abierta, entonces la cita aparece sin recargar la página.

### RF-DIS-04 — Registrar Atención o Ausencia (G2-44)

- **Prioridad:** Imprescindible  
- **Actor(es) según el SRS:** Médico (desde Consultar Agenda del Día)  
- **Historia (borrador):** Como Médico, quiero registrar si el paciente fue atendido o no se presentó, para cerrar el ciclo de la cita y medir el ausentismo.  
- **En qué se apoya el "para…":** P-002 y P-007.  
- **Relación en el SRS:** Extiende (<<extend>>) RF-DIS-03 Consultar Agenda del Día. Alimenta RF-REP-03 Reporte de Ausentismo.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cita CONFIRMADA cuya hora de inicio ya llegó, cuando el médico registra la atención, entonces la cita pasa a ATENDIDA.
  - CA-02 Dado una cita CONFIRMADA con menos de 15 minutos desde su inicio, cuando el médico intenta marcar ausencia, entonces el sistema no lo permite.
  - CA-03 Dado una cita en PENDIENTE_PAGO, cuando el médico intenta marcarla como ATENDIDA, entonces el sistema lo rechaza indicando que el pago está pendiente.
  - CA-04 Dado una cita sin registro al cierre de la jornada, cuando se ejecuta el cierre, entonces el sistema la marca como AUSENTE.
- **Observación:** Hallazgo abierto (ver tarea G2-53): el SRS permite corregir un registro hasta 24 h después, pero RNF-06 define ATENDIDA y AUSENTE como estados finales. Además, esta historia Imprescindible extiende a RF-DIS-03 (Debería tener).

### RF-DIS-05 — Recibir Notificación de Cita (G2-45)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Médico  
- **Historia (borrador):** Como Médico, quiero recibir notificación de citas nuevas, canceladas o reprogramadas, para mantener mi agenda al día sin revisarla constantemente.  
- **En qué se apoya el "para…":** P-010.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado una cita nueva para el médico, cuando se registra, entonces el sistema genera la notificación interna y el correo en un máximo de 1 minuto.
  - CA-02 Dado que una cita del médico se cancela o reprograma, cuando ocurre el evento, entonces el sistema notifica al médico por ambos canales.
- **Observación:** Hallazgo abierto (ver tarea G2-53): el SRS §1.5 dice que RF-DIS-05 usa SMS, pero el RF solo define notificación interna y correo.

---

## Módulo REP · Generar Reportes (Epic G2-7)

### RF-REP-01 — Aplicar Filtros de Reporte (G2-46)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador, Director General (desde los reportes que extiende)  
- **Historia (borrador):** Como Administrador o Director General, quiero filtrar cualquier reporte por rango de fechas, sucursal, médico y especialidad, para analizar solo la parte del negocio que me interesa.  
- **En qué se apoya el "para…":** P-007 (sin reportes de gestión).  
- **Relación en el SRS:** Extiende (<<extend>>) RF-REP-02, RF-REP-03, RF-REP- 04 y RF-REP-05.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado filtros combinados de rango de fechas, sucursal, médico y especialidad, cuando se aplican, entonces el reporte incluye solo los registros que cumplen todos los criterios en un máximo de 3 segundos.
  - CA-02 Dado un rango con fecha inicio posterior a la fecha fin, o mayor a 12 meses, cuando se aplica, entonces el sistema rechaza el filtro indicando rango inválido.

### RF-REP-02 — Reporte de Citas Confirmadas (G2-47)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador, Director General  
- **Historia (borrador):** Como Administrador o Director General, quiero ver el reporte de citas confirmadas del periodo, para conocer la demanda real.  
- **En qué se apoya el "para…":** P-007 (sin reportes de gestión).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un periodo filtrado, cuando se genera el reporte, entonces incluye solo citas que alcanzaron CONFIRMADA, con los campos y totales definidos, en un máximo de 5 segundos.
  - CA-02 Dado el reporte generado, cuando se revisa, entonces las citas aparecen ordenadas por fecha descendente.

### RF-REP-03 — Reporte de Ausentismo (G2-48)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador, Director General  
- **Historia (borrador):** Como Administrador o Director General, quiero ver el porcentaje de ausentismo por médico, especialidad y sucursal con comparativa entre periodos, para decidir qué hacer contra el ausentismo.  
- **En qué se apoya el "para…":** P-002 y P-007.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un periodo con 8 citas ATENDIDA y 2 AUSENTE para un médico, cuando se genera el reporte, entonces muestra 20,00% de ausentismo para ese médico.
  - CA-02 Dado un periodo filtrado, cuando se genera el reporte, entonces muestra la variación respecto al periodo anterior de igual duración.

### RF-REP-04 — Reporte de Cancelaciones (G2-49)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador, Director General  
- **Historia (borrador):** Como Administrador o Director General, quiero ver las cancelaciones con sus motivos, tendencias y pacientes recurrentes, para atacar las causas de las cancelaciones tardías.  
- **En qué se apoya el "para…":** P-001 y P-007.  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un periodo filtrado, cuando se genera el reporte, entonces muestra las cancelaciones agrupadas por motivo y por origen.
  - CA-02 Dado un paciente con 3 cancelaciones en el periodo, cuando se genera el reporte, entonces aparece en la lista de pacientes recurrentes.

### RF-REP-05 — Reporte de Ingresos (G2-50)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador, Director General  
- **Historia (borrador):** Como Administrador o Director General, quiero ver los pagos, los reembolsos y el ingreso neto del periodo, para conocer el resultado financiero real.  
- **En qué se apoya el "para…":** P-007 (sin reportes de gestión).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un periodo con pagos y reembolsos, cuando se genera el reporte, entonces el ingreso neto es igual al total de pagos aprobados menos el total de reembolsos.
  - CA-02 Dado un usuario con rol Recepcionista, cuando intenta acceder al reporte, entonces el sistema rechaza el acceso.

### RF-REP-06 — Exportar Reporte (G2-51)

- **Prioridad:** Debería tener  
- **Actor(es) según el SRS:** Administrador, Director General  
- **Historia (borrador):** Como Administrador o Director General, quiero exportar los reportes a PDF o Excel, para compartirlos en reuniones de dirección.  
- **En qué se apoya el "para…":** P-007 (sin reportes de gestión).  
- **Criterios de aceptación (SRS v4.0):**
  - CA-01 Dado un reporte filtrado, cuando se exporta en PDF, entonces el archivo se descarga en un máximo de 5 segundos y no permite edición.
  - CA-02 Dado un reporte filtrado, cuando se exporta en Excel (.xlsx), entonces el archivo se descarga en un máximo de 5 segundos.
  - CA-03 Dado el archivo descargado, cuando se revisa, entonces su nombre incluye el tipo de reporte y la fecha de generación, y su contenido indica usuario, fecha y filtros.

---

## Siguiente paso

Cuando el equipo valide los "para…", se pega cada historia al inicio de la descripción de su issue en Jira (39 ediciones) y este archivo se sube a la carpeta `1.3 Historias de usuario/`. Las historias con hallazgo se cierran después de aprobar la errata del SRS (G2-53).
