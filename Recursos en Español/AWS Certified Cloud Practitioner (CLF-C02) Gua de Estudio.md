
**Autor:** Tom Taulli | **Publicado:** 2026 (O'Reilly Media)

Este documento ofrece un resumen ampliado y muy detallado de la Guía de Estudio de AWS Certified Cloud Practitioner (CLF-C02). Sigue un enfoque estructurado con títulos y subtítulos para brindar un contexto más profundo de cada tema y servicio mencionado en el libro.

---

## Capítulo 1: Introducción al examen AWS Certified Cloud Practitioner (CLF-C02)

### 1.1 Propósito de la certificación
La certificación AWS Cloud Practitioner está diseñada para validar el entendimiento general de una persona sobre la plataforma AWS Cloud. Es muy beneficiosa no solo para profesionales técnicos (como desarrolladores y administradores de sistemas), sino también para roles no técnicos —incluidos ventas, marketing, finanzas y gerentes de proyecto— que necesitan comunicarse eficazmente sobre soluciones en la nube y comprender cómo AWS genera valor de negocio.

### 1.2 Estructura del examen (dominios y ponderación)
El examen evalúa a los candidatos en cuatro dominios principales, cada uno con una ponderación específica que refleja su importancia:
* **Dominio 1: Conceptos de la nube (24 %)**: Se centra en definir la nube de AWS y su propuesta de valor, destacando aspectos como la elasticidad, la escalabilidad, la agilidad y los distintos modelos de despliegue en la nube.
* **Dominio 2: Seguridad y cumplimiento (30 %)**: El segundo dominio con mayor ponderación, hace énfasis en el Modelo de Responsabilidad Compartida de AWS, la Gestión de Identidades y Accesos (IAM) y servicios de seguridad clave como WAF, Shield y Macie.
* **Dominio 3: Tecnología y servicios de la nube (34 %)**: Evalúa tu conocimiento de los servicios centrales de AWS en cómputo (EC2, Lambda), almacenamiento (S3), bases de datos (RDS) y la infraestructura global de AWS.
* **Dominio 4: Facturación, precios y soporte (12 %)**: Cubre cómo AWS cobra por sus servicios, los distintos modelos de precios y las herramientas de gestión de costos como AWS Budgets y Cost Explorer.

### 1.3 Logística y entorno del examen
El examen dura 90 minutos y consta de 65 preguntas, en formato de opción múltiple o de respuesta múltiple. Solo se califican 50 preguntas, mientras que las 15 restantes son experimentales y no se puntúan. Para aprobar se requiere una puntuación de 700 sobre 1000 posibles. Los candidatos pueden presentar el examen de manera presencial en un centro de pruebas Pearson VUE o de forma remota mediante el sistema de supervisión en línea OnVUE.

### 1.4 Certificaciones posteriores
Esta certificación fundamental actúa como un peldaño hacia rutas más avanzadas. Después de aprobar, los profesionales suelen buscar los exámenes de nivel Associate (Solutions Architect, Developer, SysOps Administrator) y más adelante aspiran a certificaciones Professional o Specialty (como Data Engineer o Security).

---

## Capítulo 2: Primeros pasos con AWS

### 2.1 Creación de cuenta y capa gratuita (Free Tier)
AWS Free Tier. La capa gratuita se divide en tres categorías:
- **Capa gratuita de seis meses**: obtienes una cuota mensual de servicios populares de forma gratuita.
- **Siempre gratis (Always Free):** servicios que no caducan, como la capacidad básica de DynamoDB, un millón de invocaciones de Lambda y CloudWatch básico.
- **12 meses gratis**: servicios disponibles durante el primer año, como 750 horas de una instancia EC2 t2.micro.
- **Pruebas de corta duración**: pruebas limitadas en el tiempo para software o servicios específicos.

### 2.2 AWS Management Console
La AWS Management Console es la interfaz web principal para administrar recursos. Verás:
- Servicios disponibles
- Visitados recientemente
- Aplicaciones
- Bienvenida a AWS
- AWS Health
- Costo y uso
- Seguridad

### 2.3 Gestión inicial de costos
Mientras usas AWS, puedes recibir cargos inesperados por cargas de trabajo que estés ejecutando. Para prevenir costos adicionales, necesitas saber dónde revisar los presupuestos.

#### 2.3.1 Paneles de facturación
Aquí puedes:
- Ver tus cargos actuales
- Configurar preferencias de entrega de facturas y moneda
- Hacer seguimiento de tu uso de la capa gratuita
- Suscribirte a alertas de facturación
- Profundizar en informes detallados de uso y costo

#### 2.3.2 Presupuestos (Budgets)
Te permiten marcar un límite en tu uso y te avisan cuando estás cerca de alcanzarlo. Los dos primeros presupuestos son gratuitos.

### 2.4 Servicios centrales de AWS
Este es uno de los temas más importantes, porque si no sabes qué hace cada servicio, no podrás responder muchas preguntas.
- **Amazon EC2 (Elastic Compute Cloud):** Máquinas virtuales (servidores) en la nube. Puedes personalizar el sistema operativo, el tamaño y la red para ejecutar casi cualquier aplicación.
- **Amazon S3 (Simple Storage Service):** Un servicio de almacenamiento de objetos ilimitado y altamente seguro. Piénsalo como un enorme disco duro en la nube para guardar archivos, medios y copias de seguridad.
- **Amazon RDS (Relational Database Service):** Un servicio administrado para bases de datos tradicionales (como MySQL o PostgreSQL). AWS gestiona automáticamente por ti las tediosas tareas de mantenimiento como copias de seguridad y parches de software.
- **Amazon Redshift:** Un potente data warehouse (almacén de datos) diseñado específicamente para analizar cantidades masivas de datos y crear paneles de inteligencia de negocio.
- **AWS Lambda:** Un servicio de cómputo "sin servidor" (serverless). Ejecuta tu código automáticamente en respuesta a disparadores (como la subida de un archivo) sin que tengas que gestionar ni mantener los servidores subyacentes.
- **Amazon CloudWatch:** La herramienta de monitoreo y observabilidad de AWS. Realiza seguimiento del rendimiento de tu sistema, recopila logs y envía alertas si algo falla.
- **AWS IAM (Identity and Access Management):** El guardián de seguridad de tu cuenta de AWS. Gestiona usuarios, grupos y los permisos exactos que tienen para acceder a recursos específicos de AWS.
- **AWS CloudTrail:** El rastro documental digital. Registra cada llamada a la API y cada acción realizada en tu cuenta de AWS (quién hizo qué y cuándo) para seguridad, cumplimiento y auditoría.
- **AWS Cost Explorer:** Una herramienta de visualización financiera que ayuda a analizar tu gasto y tus tendencias de uso de AWS a lo largo del tiempo para encontrar ahorros (se actualiza a diario).
- **AWS Budgets:** Una herramienta financiera proactiva que te permite establecer límites de gasto personalizados y te envía alertas _antes_ de que tu factura se dispare.
- **AWS Bedrock:** Una plataforma de IA generativa. Te da acceso a modelos fundacionales de primer nivel (de compañías como Anthropic, Meta y Amazon) para que puedas construir, escalar y evaluar tus propias aplicaciones de IA mediante APIs.

---

## Capítulo 3: Fundamentos de la computación en la nube

### 3.1 Computación en la nube
La computación en la nube es la entrega bajo demanda de recursos de TI a través de Internet con un modelo de precios de **pago por uso (pay-as-you-go)**. En lugar de comprar, poseer y mantener centros de datos y servidores físicos, puedes acceder a servicios tecnológicos, como capacidad de cómputo, almacenamiento y bases de datos, según los necesites, desde un proveedor de nube como Amazon Web Services (AWS).

### 3.2 Modelos de despliegue en la nube
Entender dónde y cómo se despliegan los recursos es fundamental:
* **Nube pública (Public Cloud)**: Los recursos son propiedad de un proveedor de servicios en la nube externo (como AWS), que los opera y entrega a través de Internet público. Ofrece escalabilidad masiva y ahorro de costos.
* **Nube privada (Private Cloud)**: Una organización aloja todo en su propio centro de datos (por ejemplo, en finanzas o salud). Ofrece máximo control y seguridad.
* **Nube híbrida (Hybrid Cloud)**: Una combinación de nubes públicas y privadas, unidas por tecnología que permite compartir datos y aplicaciones entre ellas, brindando flexibilidad y manteniendo datos sensibles en las instalaciones (on-premises) si es necesario.

### 3.3 Modelos de servicio en la nube
La nube entrega servicios en tres niveles principales:
* **IaaS (Infraestructura como Servicio)**: Pagas por lo que usas y obtienes control total sobre el entorno. Esto significa que puedes elegir tu sistema operativo, instalar el software que necesites y configurar los sistemas a tu gusto. No gestionas servidores físicos.
* **PaaS (Plataforma como Servicio)**: La plataforma te da todo lo que necesitas para construir y desplegar software: entornos de ejecución, bases de datos, frameworks y herramientas de integración y entrega/despliegue continuos (CI/CD). Solo escribes código, sin gestionar la infraestructura.
* **SaaS (Software como Servicio)**: El proveedor se encarga del software, las actualizaciones y la seguridad. Tú solo usas la aplicación. (Por ejemplo, Gmail, Dropbox).

### 3.4 Beneficios de la nube
Las ventajas principales de migrar a la nube incluyen:
* **Alta disponibilidad**: Los sistemas permanecen accesibles incluso durante fallas de hardware.
* **Tolerancia a fallos**: La capacidad de un sistema de seguir operativo a pesar de fallas de componentes.
* **Elasticidad y escalabilidad**: La capacidad de escalar recursos automáticamente hacia arriba o hacia abajo según la demanda.
* **Agilidad**: La velocidad con la que se pueden aprovisionar recursos, acelerando la innovación.
* **Alcance global**: Desplegar aplicaciones en múltiples regiones del mundo con unos pocos clics.

---

## Capítulo 4: Fundamentos de AWS

### 4.1 Economía de la nube (Economía de AWS)
#### 4.1.1 On-Premise (nube privada) vs. entornos de computación en la nube
Una de las métricas clave que ayuda a darle sentido a esto es el TCO (Costo Total de Propiedad, Total Cost of Ownership). No se trata solo del precio de un servidor. Más bien, engloba todo, como los costos de compra, los gastos operativos, el mantenimiento continuo y las personas que lo mantienen todo en funcionamiento.

#### 4.1.2 Gastos de capital vs. gastos operativos
- **Gasto de capital (CapEx)**: generalmente se refiere a inversiones on-premises, gastar por adelantado para adquirir activos físicos como edificios, centros de datos, servidores y licencias de software perpetuas.
- **Gasto operativo (OpEx)**: por el contrario, incluye costos operativos que surgen del uso diario de servicios como cómputo, almacenamiento, suscripciones SaaS y ofertas administradas.

#### 4.1.3 Bring-Your-Own-License (BYOL) vs. modelo de licencia incluida
- **Bring-Your-Own-License (traer tu propia licencia)**: Si tienes una licencia vinculada al hardware, puedes conservarla con instancias EC2 dedicadas. Con una licencia con Software Assurance (SA), puedes usar la movilidad de licencias para desplegar en instancias EC2 compartidas.
- **Modelo de licencia incluida**: Usa el sistema de pago por uso para incorporar los costos de licenciamiento del software al precio por hora de la instancia. No es beneficioso para una carga de trabajo de larga duración.

#### 4.1.4 Automatización
- **AWS Systems Manager**: Es un motor de automatización; Auto Scaling automatiza el escalado de recursos según la demanda, y Compute Optimizer automatiza los hallazgos de ahorro de costos.
- **Elastic Beanstalk y AWS Lambda**: Escalan automáticamente tu aplicación según la demanda.
- **AWS Config y CloudTrail**: Vigilan tu entorno haciendo seguimiento de los cambios de recursos y registrando la actividad de los usuarios.

### 4.2 AWS Well-Architected Framework
Este marco proporciona un enfoque coherente para que los clientes evalúen arquitecturas e implementen diseños que escalen con el tiempo. Se basa en seis pilares:
1. **Excelencia operativa**: Ejecutar y monitorear sistemas para entregar valor de negocio.
2. **Seguridad**: Proteger información, sistemas y activos.
3. **Fiabilidad**: Asegurar que una carga de trabajo cumpla su función prevista de forma correcta y coherente.
4. **Eficiencia del rendimiento**: Usar los recursos de TI y cómputo de manera eficiente.
5. **Optimización de costos**: Evitar costos innecesarios.
6. **Sostenibilidad**: Minimizar el impacto ambiental de ejecutar cargas de trabajo en la nube.

### 4.3 AWS Cloud Adoption Framework (CAF)
El CAF ayuda a las organizaciones a diseñar y recorrer un camino acelerado hacia una adopción exitosa de la nube. Cada perspectiva se dirige a partes interesadas específicas de la organización y les ayuda a actualizar sus habilidades y procesos. Organiza la orientación en seis perspectivas:
- **Perspectiva de negocio:** Se centra en el "porqué" de la adopción de la nube. Asegura que las inversiones en la nube estén alineadas con los objetivos financieros, las estrategias y los esfuerzos de transformación digital de la empresa. _(Objetivo: ejecutivos como CEOs y CFOs)_.
- **Perspectiva de personas:** Se centra en el elemento humano. Aborda la cultura organizacional, la mejora de habilidades, la capacitación y la gestión del cambio para asegurar que los empleados estén listos para adaptarse a la nube. _(Objetivo: RR. HH. y líderes de equipo)_.
- **Perspectiva de gobernanza:** Todo lo relacionado con reglas, riesgo y cumplimiento. Asegura que la organización tenga la supervisión, los controles financieros y los procesos adecuados para gestionar el uso de la nube de manera responsable. _(Objetivo: CIOs y gerentes de programa)_.
- **Perspectiva de plataforma:** El plano técnico. Se centra en cómo diseñar, construir, modernizar y escalar realmente las arquitecturas y aplicaciones en la nube. _(Objetivo: arquitectos de soluciones e ingenieros de TI)_.
- **Perspectiva de seguridad:** Dedicada a proteger datos y sistemas. Cubre la confidencialidad, la detección de amenazas, la gestión de identidades (IAM) y el cumplimiento para mantener seguro el entorno en la nube. _(Objetivo: CISOs y equipos de seguridad)_.
- **Perspectiva de operaciones:** Cubre el funcionamiento diario de la nube. Involucra monitoreo, mantenimiento, respuesta a incidentes y recuperación ante desastres para que todo siga funcionando sin problemas. _(Objetivo: operaciones de TI y DevOps)_.

### 4.4 Migración
AWS proporciona un conjunto de herramientas práctico conocido como las seis estrategias de migración, comúnmente llamadas las 6 R.
- **Rehost ("Lift and Shift"):** Mover la aplicación exactamente como está a la nube sin cambiar nada de código.
- **Replatform ("Lift and Tweak"):** Hacer ajustes menores a la aplicación para aprovechar algunos beneficios de la nube (como una base de datos administrada) sin una reescritura completa.
- **Refactor / Re-architect:** Rediseñar y reconstruir por completo la aplicación para aprovechar plenamente las características modernas nativas de la nube (como serverless).
- **Repurchase (recomprar):** Reemplazar por completo tu aplicación antigua comprando un producto en la nube listo para usar (SaaS, como Salesforce).
- **Retain (retener):** No hacer nada por ahora; dejar la aplicación on-premises porque no puede o no debe moverse todavía.
- **Retire (retirar):** Apagar y eliminar aplicaciones que ya no usas para ahorrar dinero y espacio.

#### 4.5 AWS Snow Family
Se usa para transferencias masivas de datos o en zonas remotas y sin conexión donde la transferencia por Internet es demasiado lenta o costosa.
- **Snowcone:** El dispositivo más pequeño y ultraportátil, para transferencias menores de datos y entornos remotos/IoT con espacio limitado.
- **Snowball:** Un dispositivo robusto del tamaño de una maleta para transferencias de datos a gran escala (de terabytes a petabytes) y computación en el borde (edge).
- **Snowmobile:** Un tráiler literal (camión con remolque) usado para mover cantidades masivas de datos a escala de exabytes.

---

## Capítulo 5: Cumplimiento y gobernanza en AWS

### 5.1 Comprendiendo las diferencias
- **Cumplimiento (Compliance):** Tus sistemas y prácticas de manejo de datos siguen reglas que provienen de leyes, estándares de la industria o tus propias políticas internas.
- **Gobernanza (Governance):** Crear y hacer cumplir las reglas; esto mantiene tus operaciones en la nube alineadas con los objetivos del negocio y la tolerancia al riesgo.
- **Seguridad (Security):** Conjunto de salvaguardas técnicas y de procedimiento que defienden tus datos, sistemas y cargas de trabajo frente a amenazas, tanto internas como externas.

### 5.2 Modelo de Responsabilidad Compartida
Este es un concepto crítico del examen que detalla quién es responsable de qué:
* **AWS es responsable de la seguridad "DE" la nube**: Esto incluye proteger la infraestructura física, el hardware, el software y las instalaciones de red que ejecutan los servicios de AWS Cloud.
* **El cliente es responsable de la seguridad "EN" la nube**: Esto incluye gestionar los datos del cliente, configurar la Gestión de Identidades y Accesos (IAM), cifrar los datos en reposo y en tránsito, y aplicar parches a los sistemas operativos invitados.

### 5.3 Panorama de los marcos de cumplimiento
AWS admite numerosos estándares de cumplimiento para ayudar a los clientes a cumplir requisitos regulatorios a nivel global.

| Marco     | Enfoque principal                                                                        |
| :-------- | :--------------------------------------------------------------------------------------- |
| PCI DSS   | Manejo seguro de datos de tarjetas de crédito (procesamiento, almacenamiento, transmisión) |
| ISO       | Estándares internacionales de seguridad y gestión de riesgos (p. ej., ISO/IEC 27001, 27017, 27018) |
| NIST      | Estándares de ciberseguridad de EE. UU. (p. ej., NIST 800-53, CSF)                       |
| FedRAMP   | Estándares de seguridad del gobierno federal de EE. UU. para servicios en la nube        |
| FINMA     | Cumplimiento regulatorio financiero suizo                                                |
| HIPAA     | Salvaguardas para la información de salud protegida                                      |
| GDPR      | Protección de datos y privacidad para residentes de la UE                                |
| SOC 1     | Controles sobre los informes financieros                                                 |
| SOC 2     | Controles de seguridad, disponibilidad y confidencialidad                                |

### 5.4 Trabajando con marcos de cumplimiento
AWS proporciona herramientas para ayudar a las organizaciones a mantener el control de su entorno:

| Herramienta         | Función principal                                                                                                                                                   |
| :------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Amazon Inspector    | Escanea instancias EC2 y cargas de trabajo en busca de vulnerabilidades                                                                                            |
| AWS Config          | Rastrea y registra los cambios de configuración en los recursos de AWS                                                                                             |
| AWS Trusted Advisor | Ofrece recomendaciones de buenas prácticas de seguridad, costo y rendimiento                                                                                       |
| AWS Audit Manager   | Automatiza la recopilación de evidencia para auditorías                                                                                                            |
| AWS Organizations   | Te ayuda a administrar múltiples cuentas de AWS desde una ubicación central                                                                                         |
| AWS Control Tower   | Automatiza la configuración de un entorno multicuenta de AWS seguro y bien gobernado                                                                               |
| AWS License Manager | Ayuda a gestionar licencias de software                                                                                                                            |
| AWS Security Hub    | Centraliza y agrega hallazgos de seguridad de servicios de AWS y herramientas de terceros; verifica continuamente el cumplimiento frente a estándares como PCI DSS y NIST CSF |
| AWS Budgets         | Permite el monitoreo de costos y uso con límites y alertas personalizados; apoya la gobernanza financiera y ayuda a hacer cumplir el cumplimiento del gasto        |

### 5.5 Documentación de cumplimiento
Cuando lleguen las auditorías o revisiones legales, necesitarás documentación.

- **AWS Artifact:** es un repositorio de informes de cumplimiento y acuerdos. Ofrece acceso inmediato a informes de auditoría de terceros como SOC, PCI DSS e ISO, así como documentos legales como los Acuerdos de Asociado de Negocios (BAA) de HIPAA.
- **AWS Customer Compliance Center:** Incluye whitepapers, preguntas frecuentes, listas de verificación de auditoría y casos de estudio de clientes de industrias reguladas.

---

## Capítulo 6: AWS Identity and Access Management (IAM)

### 6.1 Identidad
Los sistemas necesitan una forma de reconocer usuarios, aplicaciones y dispositivos. Y no solo reconocerlos, sino verificar que están autorizados a hacer lo que intentan hacer.
AWS IAM es central para la gestión de identidades y accesos; sin embargo, no es en sí un proveedor de identidad. En cambio, IAM controla quién puede acceder a los recursos de AWS y qué acciones puede realizar.

### 6.2 Autenticación vs. autorización
- **Autenticación:** ¿Quién eres?
- **Autorización:** ¿Qué puedes hacer?

### 6.3 Fundamentos de IAM
IAM es el servicio fundamental para controlar el acceso a los recursos de AWS. Sus principales entidades son:
* **Usuarios**: Personas o aplicaciones individuales que interactúan con AWS.
* **Grupos**: Colecciones de usuarios. Aplicar una política a un grupo otorga automáticamente esos permisos a todos los usuarios del grupo.
* **Roles**: Identidades con políticas de permisos que determinan lo que la identidad puede y no puede hacer en AWS. A diferencia de los usuarios, los roles no tienen credenciales de largo plazo y son asumidos temporalmente por servicios (como una instancia EC2) o por usuarios federados.

### 6.4 Políticas de IAM
Las políticas son documentos JSON que definen permisos: qué acciones se permiten o deniegan, sobre qué recursos de AWS y bajo qué condiciones.

| Campo clave          | Descripción                                                                                  |
| :------------------- | :------------------------------------------------------------------------------------------ |
| Version              | Especifica la versión del lenguaje de la política. "2012-10-17" es la más usada.            |
| Statement            | Una o más reglas que definen los permisos.                                                   |
| Effect               | "Allow" o "Deny": controla si la acción está permitida.                                      |
| Action               | Las operaciones específicas de la API permitidas (p. ej., `ec2:RunInstances`).              |
| Resource             | El o los recursos de AWS a los que aplican las acciones; puede ser * o Amazon Resource Names (ARNs) específicos. |
| Condition (opcional) | Restricciones adicionales (p. ej., dirección IP, hora).                                      |

### 6.5 Buenas prácticas de seguridad
El examen evalúa mucho las buenas prácticas de IAM:
* **Autenticación multifactor (MFA)**: Añadir una capa extra de seguridad más allá de solo una contraseña para el usuario root y los usuarios de IAM.
* **Principio de mínimo privilegio**: Otorgar a los usuarios solo el mínimo absoluto de permisos que necesitan para desempeñar sus funciones específicas.
* **Políticas de contraseñas**: Hacer cumplir reglas de longitud, complejidad y caducidad de las contraseñas.

### 6.6 Seguridad para IAM
- **IAM Credential Reports:** te da una instantánea de cada usuario de IAM en tu cuenta de AWS. Muestra si cada usuario tiene contraseña, claves de acceso activas, MFA habilitado o certificados de firma antiguos habilitados.
- **IAM Access Advisor:** ofrece información sobre los permisos otorgados a usuarios y roles de IAM. Destaca los servicios de AWS a los que pueden acceder y la última vez que se usaron esos servicios. Esta herramienta es útil para identificar permisos no utilizados.

---

## Capítulo 7: Seguridad

### 7.1 Amenazas de seguridad comunes
La mayoría de los ataques involucran malware. Estas son las grandes categorías de amenazas que debes conocer para el examen:
- **Ransomware**: extorsión mediante cifrado de datos.
- **Phishing**: ingeniería social.
- **DDoS (denegación de servicio distribuida)**: ataques diseñados para saturar sistemas.
- **Ataques de intermediario (Man-in-the-middle, MitM)**: interceptan la comunicación entre dos sistemas.
- **Exploits de día cero (Zero-day)**: Aprovechan vulnerabilidades de software que aún no han sido parcheadas.
- **Ataques de fuerza bruta**: Se basan en herramientas automatizadas para adivinar credenciales de inicio de sesión o en ingeniería social.
- **Ataques de inyección**: insertar código malicioso en formularios web o aplicaciones para obtener control de los sistemas backend.

### 7.2 Modelo de Responsabilidad Compartida de AWS
#### 7.2.1 Clientes (responsabilidad por la seguridad **en** la nube)
* **Datos del cliente:** Propiedad, clasificación, gestión y protección de los datos.
* **Plataforma, aplicaciones, identidad y gestión de accesos:** Gestión de la autorización, cuentas de usuario, mecanismo de autenticación, credenciales, seguridad de aplicaciones y permisos.
* **Sistemas operativos, red y configuración de firewall:** Fortalecimiento (hardening) del sistema operativo, gestión de parches de las instancias del usuario, configuración de security groups, ACLs de red y reglas de firewall.
* **Protección y cifrado de datos:**
    * Cifrado de datos del lado del cliente
    * Cifrado del lado del servidor
    * Protección del tráfico de red (p. ej., cifrado en tránsito, TLS)

#### 7.2.2 AWS (responsabilidad por la seguridad **de** la nube)
* **Software:** Gestión de los sistemas operativos anfitriones, la capa de virtualización y el software nativo que impulsa los servicios centrales de la nube.
* **Servicios de infraestructura central:**
    * Cómputo
    * Almacenamiento
    * Base de datos
    * Redes
* **Hardware / infraestructura global de AWS:** Mantener y proteger las instalaciones físicas, los centros de datos, los servidores de hardware y los componentes físicos subyacentes de la infraestructura.
* **Elementos de la infraestructura global:**
    * Regiones
    * Zonas de Disponibilidad
    * Ubicaciones de borde (Edge Locations)

### 7.3 Defensa en profundidad (Defense-in-Depth)
Estas son las capas de un sistema de defensa en profundidad. Cada capa aborda una porción específica del panorama de amenazas:

#### 7.3.1 Capa 1: Protección en el borde (Edge)
Esta es tu primera línea de defensa. Filtras el tráfico entrante, bloqueas a los actores maliciosos y mejoras el rendimiento en el camino.
* **Route 53 y DNS Firewall:** Enrutamiento global de tráfico con verificaciones de estado; bloquea búsquedas de dominios maliciosos.
* **CloudFront:** CDN que absorbe picos de tráfico, almacena contenido en caché y proporciona TLS/filtrado geográfico.
* **AWS Shield:** Protección contra DDoS. **Standard** es gratuito/automático; **Advanced** añade soporte 24/7 del DRT y protección financiera.
* **AWS WAF:** Inspecciona el tráfico HTTP/HTTPS para bloquear inyecciones SQL, bots e IPs maliciosas.
* **Firewall Manager:** Centraliza la aplicación de políticas de firewall en múltiples cuentas de AWS.
* **Security Hub:** Consolida los hallazgos de seguridad en un solo panel y los mapea a estándares de cumplimiento (PCI, NIST).
* **AWS Config:** Registra y audita las configuraciones de recursos para detectar brechas de seguridad.

#### 7.3.2 Capa 2: Filtrado del tráfico entrante
El filtrado del tráfico entrante en esta etapa te da un control preciso sobre quién puede comunicarse con tus sistemas y cómo.
* **Elastic Load Balancing (ELB):** Actúa como un único punto de entrada ("puerta principal") que enruta el tráfico a destinos sanos (EC2, contenedores). Oculta la infraestructura backend de la exposición directa y ofrece resiliencia frente a picos de tráfico o fallas.
* **AWS Network Firewall:** Se despliega en el borde de la VPC (IGW, VPN) para inspeccionar el tráfico en profundidad mediante reglas con estado (conscientes de la sesión) y sin estado. Incluye descifrado TLS, escaneo de protocolos y prevención de intrusiones (IPS).
* **Security Groups:** Control de tráfico con estado a nivel de recurso (asociado a instancias/ENIs). Permite automáticamente el tráfico de retorno según reglas granulares de permiso para IPs, puertos y protocolos.
* **Network ACLs (NACLs):** Control de tráfico sin estado a nivel de subred que evalúa los paquetes en ambos sentidos. Evalúa reglas de permitir/denegar en orden numérico para hacer cumplir límites amplios antes de que el tráfico llegue a las instancias.

#### 7.3.3 Capa 3: Protección del cómputo
Se trata de proteger los sistemas que ejecutan tu código.
* **Auto Scaling**: Ajusta dinámicamente los recursos de cómputo según la demanda.
* **Amazon Inspector**: Escaneo automatizado de vulnerabilidades y detección de exposiciones.
* **AWS Systems Manager**: Gestión centralizada de operaciones, aplicación de parches y cumplimiento en distintos entornos.

#### 7.3.4 Capa 4: Salvaguardas de datos e identidad
Esta capa se trata de proteger tus activos más críticos.
* **AWS Key Management Service (KMS)**: Gestiona claves de cifrado en los servicios de AWS.
* **AWS CloudHSM**: Gestión de claves dedicada basada en hardware.
* **AWS Certificate Manager (ACM)**: Aprovisiona, gestiona y despliega certificados SSL/TLS para conexiones seguras.
* **AWS Secrets Manager**: Almacenamiento seguro y rotación de información sensible como credenciales.

#### 7.3.5 Capa 5: Monitoreo y detección
En esta capa se recopilan logs, se marcan comportamientos inusuales, se envían alertas y los manuales de respuesta a incidentes se activan automáticamente.
* **GuardDuty:** Detección de amenazas con ML (CloudTrail, VPC Flow Logs, DNS).
* **Security Hub:** Panel de seguridad unificado; se mapea al cumplimiento (PCI, NIST).
* **CloudTrail y CloudWatch:** CloudTrail registra las llamadas a la API; CloudWatch monitorea métricas/logs en tiempo real.
* **Macie:** Encuentra y clasifica datos sensibles en S3 mediante ML.
* **Trusted Advisor:** Comprobaciones de optimización automatizadas (seguridad, costo, rendimiento).

### 7.4 Recursos para la seguridad en AWS Cloud
* **AWS Knowledge Center:** Guías paso a paso, preguntas frecuentes y videos para tareas comunes (p. ej., configuración de IAM, MFA, configuraciones de la CLI).
* **AWS Trust Center:** Artefactos de cumplimiento, whitepapers de seguridad, avisos y herramientas de reporte de vulnerabilidades.
* **AWS Security Blog:** Publicaciones de expertos que cubren actualizaciones de servicios, escenarios del mundo real y análisis profundos de seguridad (p. ej., Secrets Manager, seguridad de IA).

---

## Capítulo 8: Infraestructura global de AWS

### Componentes centrales de la infraestructura
La presencia global de AWS se construye sobre una arquitectura altamente resiliente:
* **Regiones**: Grandes agrupaciones geográficas de centros de datos. Las regiones están completamente aisladas entre sí para lograr la mayor tolerancia a fallos y estabilidad posibles, algo vital para el cumplimiento de la soberanía de datos.
* **Zonas de Disponibilidad (AZs)**: Cada región consta de varias AZs aisladas y físicamente separadas. Una AZ es uno o más centros de datos independientes con energía, red y conectividad redundantes. Están conectadas mediante redes de alto ancho de banda y latencia ultrabaja.

### Red de borde y entrega de contenido
Para acercar los datos a los usuarios finales a nivel global, AWS usa una red de borde (Edge Network):
* **Edge Locations**: Puntos de presencia (PoPs) globales usados principalmente para almacenar contenido en caché más cerca de los usuarios y reducir la latencia.
* **Amazon CloudFront**: El servicio de red de entrega de contenido (CDN) de AWS que entrega de forma segura datos, videos, aplicaciones y APIs a clientes de todo el mundo con baja latencia usando las Edge Locations.
* **Amazon Route 53**: Un servicio web de sistema de nombres de dominio (DNS) en la nube, altamente disponible y escalable, diseñado para enrutar a los usuarios finales hacia aplicaciones de Internet.
* **AWS Global Accelerator**: Un servicio de red que mejora la disponibilidad y el rendimiento de aplicaciones con usuarios locales o globales enrutando el tráfico a través de la red privada global de AWS en lugar de Internet público.

### Computación de borde avanzada
Para requisitos específicos de baja latencia o híbridos:
* **AWS Outposts**: Un servicio totalmente administrado que ofrece la misma infraestructura, servicios, APIs y herramientas de AWS prácticamente en cualquier centro de datos on-premises o espacio de colocation, para una experiencia híbrida verdaderamente coherente.
* **Local Zones**: Coloca cómputo, almacenamiento, bases de datos y otros servicios selectos de AWS más cerca de los usuarios finales en grandes centros poblacionales o industriales.
* **Wavelength Zones**: Despliegues de infraestructura de AWS que integran los servicios de cómputo y almacenamiento de AWS dentro de los centros de datos de los proveedores de telecomunicaciones en el borde de la red 5G.

### Despliegue de servicios de AWS
- **AWS Management Console:** Una interfaz gráfica para tareas rápidas, pruebas y gestión manual sin escribir código.
- **AWS CLI:** Una herramienta de línea de comandos para automatizar tareas mediante scripts y gestionar recursos de forma reproducible.
- **AWS SDKs:** Bibliotecas de programación que integran la funcionalidad de AWS directamente en tus aplicaciones, manejando procesos complejos en segundo plano.
- **AWS APIs:** Endpoints HTTP de bajo nivel para interactuar directamente con los servicios de AWS al construir herramientas personalizadas o integraciones únicas.
- **Infraestructura como Código (IaC):** Herramientas como Terraform o CDK para definir, versionar y desplegar infraestructura como código, logrando entornos coherentes y escalables.

---

## Capítulo 9: Cómputo, contenedores y serverless en AWS

### Cómputo central (Amazon EC2)
Amazon Elastic Compute Cloud (EC2) proporciona capacidad de cómputo redimensionable en la nube.
* **Tipos de tenencia (Tenancy)**: La diferencia entre hardware compartido, *Dedicated Instances* (se ejecutan en una nube privada virtual sobre hardware dedicado a un solo cliente) y *Dedicated Hosts* (un servidor físico totalmente dedicado a tu uso, útil para BYOL - Bring Your Own License).
* **Familias de instancias**: Entender que hay instancias especializadas y optimizadas: propósito general (M, T) que equilibran recursos; optimizadas para cómputo (C) que priorizan la CPU; optimizadas para memoria (R, X, Z) que se enfocan en la RAM; y optimizadas para almacenamiento (I, D, H) que enfatizan el almacenamiento local rápido.

### Contenedores y orquestación
Los contenedores ofrecen un mecanismo lógico de empaquetado en el que las aplicaciones pueden abstraerse del entorno en el que realmente se ejecutan.
* **Amazon ECS (Elastic Container Service)**: Un servicio de orquestación de contenedores altamente escalable y de alto rendimiento que admite contenedores Docker y te permite ejecutar y escalar fácilmente aplicaciones en contenedores en AWS.
* **Amazon EKS (Elastic Kubernetes Service)**: Un servicio administrado que facilita usar Kubernetes en AWS sin necesidad de levantar ni mantener tu propio plano de control de Kubernetes. Internamente, agrupa contenedores en pods (esencialmente unidades de trabajo) y los distribuye a través de un clúster de nodos.
* **AWS Fargate**: Un motor de cómputo serverless para contenedores que funciona tanto con ECS como con EKS. Fargate elimina la necesidad de aprovisionar y gestionar servidores, permitiéndote especificar y pagar los recursos por aplicación.

### Cómputo serverless
* **AWS Lambda**: El servicio insignia de cómputo serverless que te permite ejecutar código sin aprovisionar ni gestionar servidores. Está impulsado por eventos (se activa por cambios en los datos, cambios de estado del sistema o acciones del usuario) y te factura estrictamente por el tiempo de cómputo consumido, medido en milisegundos.

### Escalado y balanceo de carga
* **Amazon EC2 Auto Scaling**: Te ayuda a mantener la disponibilidad de la aplicación y te permite añadir o eliminar automáticamente instancias EC2 según condiciones que defines, asegurando que tengas el número correcto de instancias para manejar la carga de tu aplicación.
* **Elastic Load Balancing (ELB)**: Distribuye automáticamente el tráfico entrante de la aplicación entre múltiples destinos, como instancias EC2, contenedores, direcciones IP y funciones Lambda, garantizando una tolerancia a fallos robusta.

---

## Capítulo 10: Servicios de almacenamiento de AWS

### Almacenamiento de objetos (Amazon S3)
Amazon Simple Storage Service (S3) proporciona almacenamiento de objetos altamente duradero y escalable. Está diseñado para mantener tus datos seguros con una durabilidad del 99,999999999 %, conocida como durabilidad de "11 nueves", distribuyendo automáticamente copias de tus archivos entre múltiples Zonas de Disponibilidad.
* **S3 Standard**: Para datos de acceso frecuente.
* **S3 Standard-Infrequent Access (Standard-IA)**: Para datos de acceso menos frecuente pero que requieren acceso rápido cuando se necesitan.
* **S3 Express**: S3 Express es para casos de uso como ejecutar analítica en tiempo real, entrenamiento de ML o cargas de trabajo estrechamente acopladas. Esto lo hace ideal para aplicaciones que exigen acceso a datos ultrarrápido.
* **S3 Glacier**:
	- **S3 Glacier Instant Retrieval:** Ofrece acceso en milisegundos para datos archivados a los que rara vez se accede pero que deben estar disponibles bajo demanda.
    - **S3 Glacier Flexible Retrieval:** Proporciona velocidades de recuperación variables (de minutos a horas) para copias de seguridad y archivos que no son urgentes.
    - **S3 Glacier Deep Archive:** El almacenamiento más rentable para datos de largo plazo, con recuperación de 12 a 48 horas; ideal para registros regulatorios o legales.

Para escenarios en los que los datos deben moverse rápidamente entre regiones, S3 Transfer Acceleration usa las ubicaciones de borde distribuidas globalmente de Amazon CloudFront para acelerar las subidas a los buckets de S3.

### Almacenamiento de bloques (Amazon EBS)
- **Concepto central:** Almacenamiento de bloques duradero y de alto rendimiento que actúa como un disco local persistente para EC2; los datos se replican dentro de una Zona de Disponibilidad (AZ).

- **Características clave:**
	- **Elastic Volumes:** Cambia el tamaño, el tipo o el rendimiento de forma dinámica sin tiempo de inactividad.
    - **Snapshots:** Copias de seguridad incrementales, en un momento específico, para recuperación ante desastres, migración y cumplimiento.
    - **Seguridad:** Cifrado AES-256 en reposo y en tránsito mediante AWS KMS.
    - **Multi-Attach:** Permite que un volumen `io2` sea compartido por múltiples instancias EC2 en la misma AZ.

- **Tipos de volumen:**
    - **General Purpose SSD (gp2/gp3):** Precio/rendimiento equilibrado para volúmenes de arranque y aplicaciones generales.
    - **Provisioned IOPS SSD (io1/io2):** Alto rendimiento y baja latencia para bases de datos de misión crítica y con muchas transacciones.
    - **Throughput Optimized HDD (st1):** Ideal para big data y almacenes de datos que requieren alto rendimiento (throughput).
    - **Cold HDD (sc1):** Almacenamiento de bajo costo para datos de acceso poco frecuente.

### Sistemas de archivos
* **Amazon EFS (Elastic File System)**: Proporciona un sistema de archivos NFS elástico, sencillo, escalable y totalmente administrado para usar con los servicios de AWS Cloud y recursos Linux on-premises. Puede ser accedido por múltiples instancias EC2 de forma concurrente. Ofrece durabilidad de 11 nueves (99,999999999 %).
* **Amazon FSx**: Proporciona sistemas de archivos de terceros totalmente administrados con compatibilidad nativa y conjuntos de características para cargas de trabajo como Windows File Server y Lustre (para computación de alto rendimiento).

### Almacenamiento híbrido y copias de seguridad
* **AWS Storage Gateway**: Un servicio de almacenamiento híbrido en la nube que te da acceso on-premises a almacenamiento en la nube prácticamente ilimitado. Opera en varios modos: *File Gateway* (acceso NFS/SMB a S3), *Volume Gateway* (almacenamiento de bloques iSCSI) y *Tape Gateway* (Biblioteca de cintas virtual o VTL, que reemplaza las copias de seguridad en cinta física).
* **AWS Backup**: Un servicio de copias de seguridad totalmente administrado y centralizado que facilita centralizar y automatizar las copias de seguridad de datos en los servicios de AWS en la nube y también on-premises.

---

## Capítulo 11: Servicios de bases de datos de AWS

### Bases de datos autoadministradas vs. totalmente administradas
Las diferencias operativas entre ejecutar una base de datos directamente en una instancia EC2 (donde el usuario debe gestionar los parches del sistema operativo, las actualizaciones de la base de datos y las copias de seguridad manuales) frente a usar servicios administrados de AWS (donde AWS se encarga del trabajo pesado y no diferenciado de la administración, el escalado y la alta disponibilidad).

### Bases de datos relacionales (SQL)
* **Amazon RDS (Relational Database Service)**: Facilita configurar, operar y escalar una base de datos relacional. Admite motores populares como MySQL, PostgreSQL, MariaDB, Oracle y Microsoft SQL Server.
* **Amazon Aurora**: Un motor de base de datos relacional totalmente administrado, compatible con MySQL y PostgreSQL, construido específicamente para la nube. Combina el rendimiento y la disponibilidad de las bases de datos empresariales tradicionales con la simplicidad y la rentabilidad de las bases de datos de código abierto.

### Bases de datos NoSQL y especializadas
* **Amazon DynamoDB**: Una base de datos NoSQL clave-valor totalmente administrada y serverless, diseñada para ejecutar aplicaciones de alto rendimiento a cualquier escala con latencia de un solo dígito de milisegundos. Incluye **Amazon DAX** (DynamoDB Accelerator) para escenarios extremos con muchas lecturas que requieren latencia de microsegundos. Escalado horizontal.
* **Amazon Neptune**: Un servicio de base de datos de grafos rápido, confiable y totalmente administrado que facilita construir y ejecutar aplicaciones que trabajan con conjuntos de datos altamente conectados (como redes sociales o motores de recomendación).
* **Amazon Timestream**: Un servicio de base de datos de series temporales rápido, escalable y totalmente administrado para aplicaciones de IoT y operativas.

### En memoria y almacenamiento de datos (Data Warehousing)
* **Amazon ElastiCache**: Te permite configurar, ejecutar y escalar sin problemas almacenes de datos en memoria populares y compatibles con código abierto (Redis y Memcached) para acelerar el rendimiento de las aplicaciones.
* **Amazon Redshift**: Un servicio de data warehouse (almacén de datos) en la nube ampliamente usado, totalmente administrado y a escala de petabytes, que hace simple y rentable analizar todos tus datos usando SQL estándar y herramientas de inteligencia de negocio (BI) existentes.

### Herramientas de migración de bases de datos
* **AWS Database Migration Service (DMS)**: Te ayuda a migrar bases de datos a AWS de forma rápida y segura. La base de datos de origen permanece plenamente operativa durante la migración. A menudo se usa junto con la **AWS Schema Conversion Tool (SCT)** al migrar entre diferentes motores de base de datos (migraciones heterogéneas).

---

## Capítulo 12: Servicios de redes de AWS

### Nube privada virtual (Amazon VPC)
Amazon VPC te permite aprovisionar una sección lógicamente aislada de la nube de AWS donde puedes lanzar recursos de AWS en una red virtual que tú defines. Entre los componentes arquitectónicos clave que se cubren están:
* **Subredes (Subnets)**: Subredes públicas (que tienen rutas directas a Internet) y subredes privadas (que no las tienen).
* **Tablas de rutas (Route Tables)**: Reglas que determinan hacia dónde se dirige el tráfico de red.
* **Internet Gateways (IGW)**: Un componente de la VPC que permite la comunicación entre tu VPC e Internet.

### DNS y enrutamiento
* **Amazon Route 53**: Más allá del enrutamiento DNS básico, ofrece políticas avanzadas de gestión de tráfico, como enrutar a los usuarios según su ubicación geográfica o la latencia hacia distintas regiones de AWS, e incluye verificaciones de estado robustas para asegurar que el tráfico solo se enrute a endpoints sanos.

### Opciones de conectividad de AWS
El libro explica cómo conectar las redes corporativas con AWS:
* **AWS Site-to-Site VPN**: Crea una conexión IPsec segura y cifrada a través de Internet público entre una red on-premises y una VPC.
* **AWS Direct Connect**: Una solución de servicio en la nube que establece una conexión de red física, dedicada y privada desde tus instalaciones hacia AWS. Esto evita por completo el Internet público, proporcionando un rendimiento más consistente, mayor ancho de banda y menor latencia.
* **VPC Peering**: Una conexión de red entre dos VPCs que te permite enrutar tráfico entre ellas usando direcciones IPv4 o IPv6 privadas.

---

## Capítulo 13: Inteligencia artificial y analítica de datos

### Conceptos y fundamentos de IA
- **Aprendizaje automático (Machine Learning, ML):** Enseñar a las computadoras a aprender patrones de los datos usando modelos estadísticos (p. ej., regresión, clustering) sin programación explícita; se usa para predicciones, filtros de spam y recomendaciones.
- **Aprendizaje profundo (Deep Learning, DL):** Un subconjunto especializado del ML que usa redes neuronales artificiales de múltiples capas para procesar datos crudos y no estructurados (p. ej., imágenes, audio, lenguaje natural); impulsa tareas complejas como el reconocimiento de imágenes y la traducción.
- **IA generativa (GenAI):** Un subconjunto del DL que aprovecha modelos como los LLMs y las GANs para **crear contenido nuevo** (texto, imágenes, código, audio); se ve en herramientas como ChatGPT, Claude y Amazon Bedrock.

### Servicios de aprendizaje automático de AWS
* **Amazon SageMaker**: Un servicio integral y totalmente administrado que brinda a desarrolladores y científicos de datos la capacidad de construir, entrenar y desplegar modelos de aprendizaje automático de forma rápida y a escala. SageMaker se integra con Bedrock, que te permite diseñar aplicaciones de GenAI, bases de conocimiento y agentes.
* **Amazon Lex**: El servicio de IA que impulsa Amazon Alexa, y te permite construir interfaces conversacionales (chatbots) en cualquier aplicación usando voz y texto.
* **Amazon Kendra**: Un servicio de búsqueda empresarial altamente preciso e inteligente, impulsado por aprendizaje automático, que permite a las organizaciones indexar y buscar en repositorios internos de documentos dispares.

### Analítica de datos
- **Amazon Athena:** Servicio de consultas serverless para ejecutar SQL directamente sobre datos de S3; pagas solo por los datos escaneados. Ideal para análisis ad hoc y exploración de logs usando Presto.
- **Amazon Kinesis:** Plataforma de streaming en tiempo real. Sus componentes incluyen:
    - **Data Streams:** Ingesta de alto rendimiento.
    - **Data Firehose:** Entrega streams a destinos (S3, Redshift).
    - **Data Analytics:** Consultas SQL sobre streams.
    - **Video Streams:** Procesamiento de video en tiempo real.

- **Amazon Glue:** Servicio ETL (Extract, Transform, Load) totalmente administrado. Usa **crawlers** para construir un Data Catalog, simplificando la preparación de datos y el descubrimiento de esquemas entre fuentes (S3, RDS, DynamoDB).
- **Amazon QuickSight:** Servicio de inteligencia de negocio (BI) para paneles interactivos y visualización de datos. Incluye **analítica embebida** e información impulsada por ML, como la detección de anomalías y la previsión.

---

## Capítulo 14: Herramientas para desarrolladores y otros servicios esenciales

### Integración de aplicaciones (desacoplamiento)
Construir arquitecturas de nube resilientes requiere desacoplar componentes:
* **Amazon SNS (Simple Notification Service)**: Un servicio de mensajería totalmente administrado para comunicación tanto de aplicación a aplicación (A2A) como de aplicación a persona (A2P), usando un modelo de publicación/suscripción (Pub/Sub).
* **Amazon SQS (Simple Queue Service)**: Un servicio de colas de mensajes totalmente administrado que te permite desacoplar y escalar microservicios, sistemas distribuidos y aplicaciones serverless. Actúa como un búfer para evitar que se pierdan mensajes si un servicio posterior falla.
* **Amazon EventBridge**: Un bus de eventos serverless que facilita construir aplicaciones basadas en eventos a escala usando eventos generados por tus aplicaciones, aplicaciones SaaS integradas y servicios de AWS.

### Aplicaciones de negocio
* **Amazon Connect**: Un centro de contacto (Call Center) en la nube omnicanal y fácil de usar que te ayuda a brindar un servicio al cliente superior a menor costo.
* **Amazon SES (Simple Email Service)**: Un servicio de correo electrónico rentable, flexible y escalable que permite a los desarrolladores enviar correos desde cualquier aplicación (transaccionales, de marketing o comunicaciones masivas).

### Herramientas para desarrolladores (DevOps)
* **AWS CodeBuild y AWS CodePipeline**: Servicios esenciales para implementar pipelines de Integración Continua y Entrega Continua (CI/CD). CodeBuild compila el código fuente, ejecuta pruebas y produce paquetes de software, mientras que CodePipeline automatiza el proceso de lanzamiento.
* **AWS X-Ray**: Un servicio que ayuda a los desarrolladores a analizar y depurar aplicaciones distribuidas en producción, como las construidas con una arquitectura de microservicios. Te permite rastrear las solicitudes de los usuarios a medida que viajan por tu aplicación.

### Servicios de aplicaciones y escritorios orientados al cliente
- **Amazon AppStream 2.0:** Transmite aplicaciones de escritorio individuales a cualquier navegador; permite la entrega SaaS sin reescribir código, manteniendo los datos seguros en la VPC.
- **Amazon WorkSpaces:** Escritorio como servicio (DaaS) que proporciona escritorios virtuales completos de Windows o Linux; se integra con Active Directory/SAML para una gestión de nivel empresarial.
- **WorkSpaces Secure Browser:** Proporciona una sesión de navegador aislada y efímera (transmitiendo solo píxeles) para evitar la fuga de datos locales y mejorar la seguridad basada en web sin necesidad de VPNs.
- **AWS Amplify:** Un conjunto completo de herramientas y bibliotecas para acelerar el desarrollo full-stack, con un pipeline de CI/CD integrado, componentes de UI e integración sencilla de backend (Auth, Storage, IA).
- **AWS AppSync:** Un servicio administrado que usa GraphQL para consolidar datos de múltiples fuentes (DynamoDB, Lambda, etc.) en un único endpoint, admitiendo actualizaciones en tiempo real mediante WebSockets y sincronización de datos sin conexión.

### Gestión de dispositivos IoT con AWS IoT Core
- **Propósito:** Servicio administrado para conectar y gestionar dispositivos IoT de forma segura y a escala.
- **Protocolos:** Usa MQTT (eficiente), HTTPS, WebSockets y LoRaWAN.
- **Seguridad:** Autenticación mutua y cifrado de extremo a extremo para todo el tráfico.
- **MQTT Broker:** Servicio administrado para mensajería de dispositivos confiable y ligera.
- **Rules Engine:** Filtra y enruta automáticamente los datos de los dispositivos hacia los servicios de AWS (p. ej., Lambda, DynamoDB).
- **Device SDKs:** Simplifica la programación en C, JavaScript y Arduino.

---

## Capítulo 15: Facturación, presupuestos y gestión de costos

### Modelos de precios y de compra
AWS ofrece una enorme flexibilidad en la forma en que pagas por los recursos de cómputo:
* **On-Demand Instances**: Paga por capacidad de cómputo por hora o por segundo sin compromisos a largo plazo. Ideal para aplicaciones con cargas de trabajo de corto plazo, con picos o impredecibles.
* **Reserved Instances (RIs)**: Ofrecen un descuento significativo (hasta 72 %) frente al precio On-Demand y proporcionan una reserva de capacidad cuando se usan en una Zona de Disponibilidad específica. Requieren un compromiso de plazo de 1 o 3 años.
* **Savings Plans**: Un modelo de precios flexible que ofrece precios bajos sobre el uso de EC2, Lambda y Fargate a cambio de un compromiso de una cantidad de uso constante (medida en $/hora) durante un plazo de 1 o 3 años.
* **Spot Instances**: Te permiten solicitar capacidad de cómputo sobrante de Amazon EC2 con hasta un 90 % de descuento sobre el precio On-Demand. Sin embargo, AWS puede recuperar la instancia con un aviso de 2 minutos. Son muy recomendables para cargas de trabajo tolerantes a fallos, flexibles y sin estado (como el procesamiento por lotes).
* **Precios de Dedicated Hosts**: Modelo de precios para servidores físicos con capacidad de instancias EC2 totalmente dedicada a tu uso, útil para necesidades específicas de cumplimiento regulatorio o de licenciamiento de software.

### Herramientas de control financiero
* **AWS Pricing Calculator**: Una herramienta de planificación basada en web que te permite crear estimaciones para tus casos de uso de AWS. Es crucial para estimar costos *antes* de construir una solución.
* **AWS Cost Explorer**: Una herramienta que te permite ver y analizar tus costos y uso. Puedes visualizar datos a lo largo del tiempo, identificar tendencias, señalar los principales generadores de costo y detectar anomalías.
* **AWS Budgets**: Te da la capacidad de establecer presupuestos personalizados que te alertan cuando tus costos o uso superan (o se prevé que superen) el monto presupuestado.
* **AWS Cost Allocation Tags**: son etiquetas de clave-valor adjuntas a los recursos para categorizar y rastrear el gasto en herramientas como Cost Explorer y Budgets, y requieren activación manual en la consola de facturación para que surtan efecto.

### AWS Organizations y consolidación
**AWS Organizations**, en particular la **facturación consolidada (Consolidated Billing)**, permite a una empresa combinar el uso de todas sus cuentas para compartir descuentos por volumen.

### Planes de soporte de AWS
Entender los niveles de soporte disponibles es vital para el examen:
* **Basic Support**: Gratuito para todos los clientes de AWS. Incluye acceso al servicio al cliente, documentación, whitepapers y foros de soporte.
* **Developer Support**: Recomendado para pruebas o desarrollo temprano en AWS. Incluye acceso por correo electrónico a Cloud Support Associates en horario laboral.
* **Business Support**: Diseñado para uso en producción. Incluye acceso 24/7 a ingenieros senior, el conjunto completo de herramientas de Trusted Advisor, soporte de software de terceros y soporte opcional de eventos mediante Infrastructure Event Management (IEM).
* **Enterprise On-Ramp**: Construido para cargas de trabajo críticas. Incluye un grupo de Technical Account Managers (TAMs), manejo priorizado de casos (p. ej., SLA de 30 minutos para problemas críticos), revisiones de arquitectura y planificación de AWS Countdown para eventos importantes.
* **Enterprise Support**: Obtienes un TAM dedicado, un equipo de facturación Concierge, SLAs más rápidos (tan bajos como 15 minutos), revisiones proactivas continuas y herramientas de automatización avanzadas para mantener todo funcionando sin problemas a escala.

---

## Capítulo 16: Estrategias y técnicas para el examen

### Recomendaciones para el día del examen
El capítulo final se centra en consejos prácticos para aprobar el examen. Hace énfasis en la importancia de un descanso adecuado. Para quienes toman el examen en línea mediante Pearson OnVUE, detalla los estrictos requisitos del entorno: un escritorio despejado, una webcam y un micrófono funcionales obligatorios, permanecer siempre dentro del encuadre de la cámara y la regla estricta de no leer las preguntas en voz alta.

### Gestión del tiempo
Con 65 preguntas y 90 minutos disponibles, los examinados tienen aproximadamente de 1,3 a 1,5 minutos por pregunta. La guía recomienda dosificar tu ritmo y no atascarte en una sola pregunta difícil.

### Estrategias para responder el examen
* **"Eliminar temprano"**: Responde de inmediato las preguntas más sencillas para ganar confianza y asegurar puntos. Marca las preguntas difíciles o ambiguas para volver a ellas durante una pasada de revisión final.
* **"Descarta las que no tienen sentido" (proceso de eliminación)**: Identifica y elimina activamente los distractores. Al descartar una o dos respuestas obviamente incorrectas, aumentas drásticamente tu probabilidad estadística de acertar (del 25 % al 33 % o 50 %).
* **Identifica palabras clave**: Lee las preguntas con mucho cuidado para identificar restricciones o requisitos específicos (p. ej., "más rentable", "altamente disponible", "serverless"). El libro advierte que leer las preguntas por encima suele llevar a malinterpretaciones y errores costosos.
