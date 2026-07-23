# AWS Certified Cloud Practitioner (CLF-C02) - Apuntes del curso

> **Curso:** AWS Certified Cloud Practitioner Certification Course (CLF-C02) - Pass the Exam!
> **Instructor:** Andrew Brown (ExamPro)
> **Canal:** freeCodeCamp.org
> **Enlace:** https://www.youtube.com/watch?v=NhDYbskXRgc

---

## Tabla de contenidos

1. [[#1. Introducción y guía del examen|Introducción y guía del examen]]
2. [[#2. Conceptos de la nube|Conceptos de la nube]]
3. [[#3. Primeros pasos|Primeros pasos]]
4. [[#4. Transformación digital|Transformación digital]]
5. [[#5. Los beneficios de la nube|Los beneficios de la nube]]
6. [[#6. Infraestructura global|Infraestructura global]]
7. [[#7. Arquitectura en la nube|Arquitectura en la nube]]
8. [[#8. Herramientas de gestión y desarrollo|Herramientas de gestión y desarrollo]]
9. [[#9. Modelo de Responsabilidad Compartida|Modelo de Responsabilidad Compartida]]
10. [[#10. Cómputo|Cómputo]]
11. [[#11. Servicios de almacenamiento|Servicios de almacenamiento]]
12. [[#12. Bases de datos|Bases de datos]]
13. [[#13. Redes|Redes]]
14. [[#14. EC2|EC2]]
15. [[#15. Modelos de precios de EC2|Modelos de precios de EC2]]
16. [[#16. Identidad|Identidad]]
17. [[#17. Integración de aplicaciones|Integración de aplicaciones]]
18. [[#18. Contenedores|Contenedores]]
19. [[#19. Gobernanza|Gobernanza]]
20. [[#20. Aprovisionamiento|Aprovisionamiento]]
21. [[#21. Serverless|Serverless]]
22. [[#22. Windows en AWS|Windows en AWS]]
23. [[#23. Registro (Logging)|Registro (Logging)]]
24. [[#24. ML, IA y Big Data|ML, IA y Big Data]]
25. [[#25. AWS Well-Architected Framework|AWS Well-Architected Framework]]
26. [[#26. TCO y migración|TCO y migración]]
27. [[#27. Facturación y precios|Facturación y precios]]

---

## 1. Introducción y guía del examen

### Sobre el examen CLF-C02
- **Nombre:** AWS Certified Cloud Practitioner (CLF-C02)
- **Duración:** 90 minutos
- **Formato:** 65 preguntas (opción múltiple y respuesta múltiple)
- **Puntuación para aprobar:** 700/1000
- **Costo:** ~100 USD
- **Idiomas disponibles:** inglés, japonés, coreano, chino y otros
- **Validez:** 3 años

### ¿Para quién es este examen?
- Personas sin experiencia técnica previa en AWS
- Ideal como **primera certificación** en la ruta de AWS
- Excelente para roles no técnicos (ventas, gerentes, finanzas) que necesitan entender la nube
- Base para certificaciones más avanzadas (Solutions Architect, Developer, SysOps)

### Ruta de certificaciones de AWS
- **Foundational:** Cloud Practitioner (CLF-C02)
- **Associate:** Solutions Architect, Developer, SysOps Administrator
- **Professional:** Solutions Architect Professional, DevOps Engineer Professional
- **Specialty:** Security, Machine Learning, Advanced Networking, Database, Data Analytics, SAP

### Contenido del examen (dominios)
| Dominio | Ponderación |
|--------|--------|
| 1. Conceptos de la nube | 24 % |
| 2. Seguridad y cumplimiento | 30 % |
| 3. Tecnología y servicios de la nube | 34 % |
| 4. Facturación, precios y soporte | 12 % |

---

## 2. Conceptos de la nube

### ¿Qué es la computación en la nube?
- La entrega **bajo demanda** de recursos de TI a través de Internet con un modelo de precios de **pago por uso (pay-as-you-go)**
- En lugar de comprar y mantener servidores físicos, accedes a servicios tecnológicos (cómputo, almacenamiento, bases de datos) según los necesites

### Evolución del hosting en la nube
1. **Servidor dedicado:** Un único servidor físico para un negocio. Muy costoso, mucho mantenimiento
2. **Servidor privado virtual (VPS):** Un único servidor físico dividido en múltiples máquinas virtuales. Mejor uso de los recursos
3. **Hosting compartido (Shared Hosting):** Un único servidor compartido entre muchos usuarios. Barato pero limitado
4. **Cloud Hosting:** Múltiples servidores actuando como un solo sistema. Flexible, escalable, pago por uso

### ¿Qué es Amazon?
- Empresa fundada en 1994 por Jeff Bezos como una librería en línea
- Creció hasta convertirse en el minorista más grande del mundo
- Amazon Web Services (AWS) nació de la infraestructura interna de Amazon

### ¿Qué es AWS?
- **Amazon Web Services** es el proveedor de servicios en la nube (CSP) más grande del mundo
- Lanzado oficialmente en **2006** con S3 y EC2
- Ofrece **más de 200** servicios
- Genera miles de millones de dólares en ingresos anuales
- Usado por empresas como Netflix, Twitch, LinkedIn, Facebook

### ¿Qué es un CSP (Cloud Service Provider)?
- Una empresa que ofrece múltiples servicios en la nube
- Servicios accesibles mediante una única API unificada (p. ej., la API de AWS)
- Facturación medida según el uso
- Monitoreo integrado
- Infraestructura como Servicio (IaaS) con automatización
- Principales CSPs: **AWS, Azure, GCP**

### Panorama de los CSPs
- **Tier 1 (líderes):** AWS, Azure, GCP — Amplia gama de servicios, líderes del mercado
- **Tier 2:** Alibaba Cloud, IBM Cloud, Oracle Cloud, Huawei Cloud
- **Tier 3:** Rackspace, DigitalOcean, Linode, Vultr

### Gartner Magic Quadrant para la nube
- AWS ha sido un líder constante en el Cuadrante Mágico de Gartner para IaaS
- AWS y Azure son los líderes, con GCP como "visionario" poniéndose al día

### Servicios comunes de la nube
Los 4 servicios más comunes de cualquier CSP:
1. **Cómputo (Compute)** — Servidores virtuales (EC2)
2. **Almacenamiento (Storage)** — Almacenamiento de archivos (S3)
3. **Redes (Networking)** — Redes virtuales (VPC)
4. **Bases de datos (Databases)** — Bases de datos administradas (RDS)

### Panorama tecnológico de AWS
- AWS tiene **más de 200** servicios agrupados en categorías:
  - Cómputo, Almacenamiento, Base de datos, Redes, Machine Learning, Analítica, Seguridad, IoT, etc.

### Evolución del cómputo
1. **Dedicado:** Servidor físico completo para ti
2. **VMs (máquinas virtuales):** Múltiples VMs en un servidor físico mediante un hipervisor
3. **Contenedores:** Múltiples aplicaciones aisladas en una VM, compartiendo el sistema operativo
4. **Funciones (Serverless):** Ejecutar código sin gestionar servidores (AWS Lambda)

### Tipos de computación en la nube
| Tipo | Descripción | Ejemplo en AWS |
|------|-------------|-------------|
| **IaaS** (Infraestructura como Servicio) | Obtienes la infraestructura básica, tú gestionas el resto | EC2, VPC |
| **PaaS** (Plataforma como Servicio) | Obtienes la plataforma, solo subes tu código | Elastic Beanstalk, Heroku |
| **SaaS** (Software como Servicio) | Software listo para usar | Gmail, Salesforce, Office 365 |

### Modelos de despliegue en la nube
| Modelo | Descripción |
|-------|-------------|
| **Nube pública (Public Cloud)** | Todo en la nube del CSP. P. ej., AWS, Azure |
| **Nube privada (Private Cloud)** | Tu propia nube en tu centro de datos (on-premise). P. ej., OpenStack, VMware |
| **Nube híbrida (Hybrid Cloud)** | Combinación de nube pública + privada |
| **Cross-Cloud / Multi-Cloud** | Uso de múltiples CSPs (AWS + Azure + GCP) |

---

## 3. Primeros pasos

### Creación de una cuenta de AWS
- Necesitas: correo electrónico, tarjeta de crédito/débito, número de teléfono
- AWS ofrece una **capa gratuita (Free Tier)** para nuevos usuarios durante 12 meses
- Se crea una cuenta root con acceso total — **NUNCA uses la cuenta root para tareas diarias**

### La historia del sobrecosto (Overbilling)
- Es común que los nuevos usuarios dejen recursos en ejecución y reciban facturas inesperadas
- **Siempre** configura alertas de facturación y presupuestos al crear tu cuenta

### AWS Budgets
- Servicio para crear **presupuestos** y recibir alertas cuando te acercas o superas el límite
- Puedes crear presupuestos por costo, uso o reservas
- Configura alertas por correo electrónico cuando alcances el 50 %, 80 % o 100 % de tu presupuesto
- **Esto es lo primero que deberías configurar al crear tu cuenta**

### AWS Free Tier
Tres tipos de ofertas gratuitas:
1. **Siempre gratis (Always Free):** Servicios que siempre son gratis (p. ej., Lambda 1M de solicitudes/mes, DynamoDB 25 GB)
2. **12 meses gratis:** Gratis durante 12 meses desde la creación de la cuenta (p. ej., EC2 t2.micro 750 h/mes, S3 5 GB)
3. **Pruebas (Trials):** Pruebas gratuitas de corta duración para servicios específicos

### Activar MFA (autenticación multifactor)
- **Crítico** para la seguridad de tu cuenta
- Habilita MFA en la cuenta root de inmediato
- Opciones: aplicación de autenticación (Google Authenticator, Authy), llave de seguridad (YubiKey), MFA por hardware
- Ve a IAM > Security credentials > MFA > Assign MFA device

---

## 4. Transformación digital

### Olas de innovación
- Las ondas de Kondratiev muestran ciclos de innovación tecnológica cada ~50 años
- Estamos en la ola de la **transformación digital** impulsada por la nube, la IA, IoT y Big Data

### Plataforma en llamas (Burning Platform)
- Concepto: cuando una empresa **debe** cambiar porque el statu quo es más peligroso que el cambio
- Ejemplo: Nokia no adoptó los smartphones y desapareció del mercado
- La nube es la respuesta a muchas "plataformas en llamas" corporativas

### Lista de verificación de transformación digital
- Migrar de on-premise a la nube
- Modernizar aplicaciones heredadas (legacy)
- Adoptar DevOps y CI/CD
- Usar datos para impulsar las decisiones (Data-Driven)
- Implementar Machine Learning e IA

### Evolución de la capacidad de cómputo
- De los mainframes a las PCs, a los servidores, a las VMs, a los contenedores, al serverless
- **AWS Graviton** — Procesadores ARM diseñados por AWS, más eficientes y rentables
- **AWS Inferentia** — Chips optimizados para inferencia de Machine Learning

### Amazon Braket
- Servicio de **computación cuántica** de AWS
- Permite experimentar con simuladores cuánticos y hardware cuántico real
- Admite múltiples tecnologías: D-Wave, IonQ, Rigetti

---

## 5. Los beneficios de la nube

### Las 6 ventajas de la computación en la nube (según AWS)
1. **Cambiar gastos de capital por gastos variables** — Pasar de CAPEX a OPEX. Sin inversión en centro de datos, paga solo por lo que usas
2. **Beneficiarse de economías de escala masivas** — AWS compra a escala masiva y traslada los ahorros a los clientes
3. **Dejar de adivinar la capacidad** — No necesitas adivinar cuánta capacidad necesitas; escala hacia arriba o hacia abajo según la demanda
4. **Aumentar la velocidad y la agilidad** — Despliega recursos en minutos en lugar de semanas
5. **Dejar de gastar dinero en operar y mantener centros de datos** — Enfócate en tu negocio, no en mantener servidores
6. **Volverse global en minutos** — Despliega tu aplicación en múltiples regiones del mundo en minutos

### La 7.ª ventaja (añadida en CLF-C02)
7. **Seguridad** — AWS ofrece seguridad de nivel empresarial. El modelo de responsabilidad compartida garantiza que AWS protege la infraestructura y tú proteges tus datos y configuraciones

---

## 6. Infraestructura global

### Panorama general
- AWS tiene la infraestructura en la nube más grande del mundo
- Distribuida globalmente para alta disponibilidad, baja latencia y resiliencia

### Regiones
- Una **región** es un área geográfica con 2 o más Zonas de Disponibilidad
- Ejemplo: `us-east-1` (N. Virginia), `eu-west-1` (Irlanda), `sa-east-1` (São Paulo)
- **Factores para elegir una región:**
  1. **Cumplimiento / regulación:** Leyes de residencia de datos
  2. **Latencia:** Proximidad a tus usuarios
  3. **Servicios disponibles:** No todos los servicios están disponibles en todas las regiones
  4. **Costo:** Los precios varían según la región

### Regiones vs. servicios globales
- **Servicios regionales:** EC2, RDS, Lambda (desplegados en una región específica)
- **Servicios globales:** IAM, Route 53, CloudFront, WAF, S3 (espacio de nombres global)

### Zonas de Disponibilidad (AZs)
- Cada región tiene un **mínimo de 3 AZs** (normalmente 3-6)
- Cada AZ es uno o más **centros de datos físicos** con energía, red y conectividad redundantes
- Las AZs están físicamente separadas (a decenas de km) pero conectadas con fibra de alta velocidad y baja latencia
- Se nombran como: `us-east-1a`, `us-east-1b`, `us-east-1c`
- **Diseñar con múltiples AZs es clave para la alta disponibilidad**

### Tolerancia a fallos
- **Fault Domain (dominio de falla):** Sección de la infraestructura que puede fallar sin afectar a otras secciones
- **Fault Level (nivel de falla):** Define qué tan grande es la falla (servidor, rack, centro de datos, AZ, región)
- Distribuir recursos entre múltiples AZs protege contra fallas a nivel de centro de datos

### AWS Global Network
- La red privada de fibra óptica de AWS que conecta todas las regiones y AZs
- Proporciona alta velocidad y baja latencia entre los servicios de AWS

### Puntos de presencia (PoP)
- Ubicaciones intermedias entre los usuarios y las regiones de AWS
- Usadas por **CloudFront (CDN)** y **Route 53 (DNS)**
- **Más de 400 PoPs** a nivel global (Edge Locations + Regional Edge Caches)
- **ISPs Tier 1:** AWS tiene acuerdos de peering con los principales proveedores de Internet

### AWS Direct Connect
- Una conexión de red **dedicada y privada** entre tu centro de datos y AWS
- No atraviesa el Internet público
- Proporciona mayor ancho de banda, menor latencia y mayor consistencia
- Ideal para cargas de trabajo que requieren una conexión estable y rápida

### Ubicaciones de Direct Connect
- Instalaciones físicas donde puedes establecer una conexión Direct Connect
- Operadas por socios de AWS en todo el mundo

### AWS Local Zones
- Extensión de una región de AWS más cerca de los usuarios finales
- Para cargas de trabajo que requieren latencia de **un solo dígito de milisegundos**
- P. ej., gaming, streaming en tiempo real, AR/VR
- Ejemplo: `us-east-1-bos-1a` (Boston)

### Wavelength Zones
- Infraestructura de AWS desplegada dentro de los centros de datos de operadores de telecomunicaciones 5G
- Latencia ultrabaja para aplicaciones móviles y de borde
- Ideal para IoT, gaming móvil, streaming

### Residencia de datos
- Las leyes de algunos países exigen que los datos permanezcan dentro de sus fronteras
- AWS te permite elegir la región donde se almacenan los datos
- **AWS Outposts:** Extensión de AWS en tu propio centro de datos para cumplir requisitos de residencia

### AWS para el gobierno
- AWS cumple los requisitos de cumplimiento gubernamental (FedRAMP, ITAR, etc.)
- **AWS GovCloud:** Regiones aisladas diseñadas para cargas de trabajo del gobierno de EE. UU.
  - Solo accesibles por ciudadanos estadounidenses autorizados
  - Cumple regulaciones como ITAR, FedRAMP High, DoD SRG

### AWS en China
- AWS opera en China a través de socios locales (Sinnet, NWCD)
- Las regiones de China están **completamente aisladas** del resto de AWS
- Se requiere una cuenta separada y una licencia comercial china (ICP License)

### Sostenibilidad
- AWS se comprometió a usar **100 % de energía renovable** para 2025
- Es el mayor comprador corporativo de energía renovable del mundo
- Los clientes pueden reducir su huella de carbono migrando a AWS

### AWS Ground Station
- Servicio totalmente administrado para controlar **comunicaciones satelitales**
- Descarga datos de satélites directamente en AWS
- Casos de uso: clima, cartografía, comunicaciones

### AWS Outposts
- Hardware de AWS instalado en **tu propio centro de datos**
- Ejecuta servicios de AWS localmente (EC2, EBS, S3, EKS, RDS)
- Para cargas de trabajo que deben permanecer on-premise por latencia o regulación
- AWS lo instala, administra y actualiza

---

## 7. Arquitectura en la nube

### Terminologías clave

| Término | Definición |
|------|-----------|
| **Alta disponibilidad (HA)** | Tu sistema permanece accesible la mayor parte del tiempo. Tiempo de inactividad mínimo. Usa múltiples AZs |
| **Alta escalabilidad** | Capacidad de crecer para manejar más demanda. Vertical (más potencia) u Horizontal (más instancias) |
| **Alta elasticidad** | **Escala automáticamente** según la demanda. Auto Scaling Groups en AWS |
| **Tolerancia a fallos** | Capacidad de seguir operando incluso cuando un componente falla. Sin tiempo de inactividad para el usuario |
| **Alta durabilidad** | Los datos almacenados no se pierden. P. ej., S3 ofrece una durabilidad del 99,999999999 % (11 nueves) |

### Plan de continuidad del negocio (BCP)
- Plan para asegurar que el negocio siga operando durante desastres
- Define **RPO** y **RTO**

### Opciones de recuperación ante desastres (de menor a mayor costo y velocidad)
| Opción | Descripción | RTO |
|--------|-------------|-----|
| **Backup & Restore** | Respaldar datos y restaurar cuando ocurre un desastre | Horas |
| **Pilot Light** | Versión mínima de tu entorno siempre en ejecución | Decenas de minutos |
| **Warm Standby** | Versión reducida pero totalmente funcional | Minutos |
| **Multi-site / Hot Standby** | Copia completa ejecutándose activamente | Tiempo real / Segundos |

### RTO (Recovery Time Objective)
- **Tiempo máximo aceptable** para restaurar el servicio tras un desastre
- Ejemplo: "Nuestro RTO es de 4 horas" = debemos estar operativos en un plazo de 4 horas

### RPO (Recovery Point Objective)
- **Cantidad máxima de datos que puedes perder** medida en tiempo
- Ejemplo: "Nuestro RPO es de 1 hora" = perdemos como máximo 1 hora de datos
- Copias de seguridad más frecuentes = RPO más bajo = más costoso

---

## 8. Herramientas de gestión y desarrollo

### AWS API
- Todos los servicios de AWS se controlan a través de una **API HTTP**
- Puedes interactuar con AWS mediante: Web Console, CLI, SDK, IaC

### AWS Management Console
- Interfaz gráfica (GUI) basada en web para gestionar los servicios de AWS
- Accesible desde el navegador en https://console.aws.amazon.com
- Ideal para aprender y explorar servicios
- **No recomendada para producción** (es mejor usar IaC)

### AWS Account ID
- Cada cuenta de AWS tiene un **ID único de 12 dígitos**
- Se usa para identificar tu cuenta de forma única
- Útil para acceso entre cuentas (cross-account) y ARNs

### Amazon Resource Names (ARNs)
- Identificador **único a nivel global** para cualquier recurso en AWS
- Formato: `arn:aws:service:region:account-id:resource`
- Ejemplo: `arn:aws:s3:::my-bucket`
- Ejemplo: `arn:aws:ec2:us-east-1:123456789012:instance/i-1234567890abcdef0`

### AWS CLI (Command Line Interface)
- Herramienta de línea de comandos para interactuar con AWS
- Instalable en Windows, Mac, Linux
- Requiere **Access Keys** (Access Key ID + Secret Access Key)
- Ejemplo: `aws s3 ls` (listar los buckets de S3)
- **Ampliamente usada en automatización y scripting**

### AWS SDK (Software Development Kit)
- Bibliotecas de código para interactuar con AWS desde tu aplicación
- Disponibles para: Python (boto3), JavaScript, Java, .NET, Go, Ruby, PHP, C++
- Permite integrar los servicios de AWS directamente en tu código

### AWS CloudShell
- Terminal basado en navegador **dentro de la consola de AWS**
- Preinstalado con AWS CLI, Python, Node.js y herramientas comunes
- 1 GB de almacenamiento persistente por región
- Gratuito (sin costo adicional)

### AWS Tools for PowerShell
- Módulo de PowerShell para gestionar recursos de AWS
- Ideal para administradores de Windows

### Infraestructura como Código (IaC)
- Práctica de definir y gestionar la infraestructura usando **archivos de configuración** en lugar de procesos manuales
- Beneficios: reproducibilidad, control de versiones, automatización, consistencia

### AWS CloudFormation
- Servicio de IaC **nativo de AWS**
- Define la infraestructura en archivos **JSON o YAML** (plantillas)
- CloudFormation crea, actualiza y elimina recursos automáticamente
- Concepto de **Stacks**: grupo de recursos gestionados como una sola unidad
- Gratuito — solo pagas por los recursos creados

### AWS CDK (Cloud Development Kit)
- Framework para definir infraestructura usando **lenguajes de programación** (TypeScript, Python, Java, C#, Go)
- "Compila" a plantillas de CloudFormation
- Más amigable para desarrolladores que escribir YAML/JSON directamente
- Permite usar lógica de programación (bucles, condicionales, funciones)

### AWS Toolkit for VS Code
- Extensión de Visual Studio Code para trabajar con AWS
- Permite desplegar funciones Lambda, ver logs, explorar recursos

### Access Keys
- Credenciales para acceder a AWS desde la CLI o el SDK
- Compuestas por: **Access Key ID** (pública) + **Secret Access Key** (privada)
- **Nunca compartas tus Access Keys**
- **Nunca las pongas en tu código fuente**
- Buena práctica: usa IAM Roles en lugar de Access Keys siempre que sea posible

---

## 9. Modelo de Responsabilidad Compartida

### Concepto central
- La seguridad en la nube es una **responsabilidad compartida** entre AWS y el cliente
- **AWS es responsable de la seguridad "DE" la nube** (infraestructura)
- **El cliente es responsable de la seguridad "EN" la nube** (datos, configuración)

### Responsabilidades de AWS (seguridad DE la nube)
- Hardware físico y centros de datos
- Infraestructura de red global
- Hipervisores
- Software de los servicios administrados
- Seguridad física (guardias, controles de acceso, CCTV)

### Responsabilidades del cliente (seguridad EN la nube)
- Datos del cliente (cifrado)
- Configuración de la plataforma y las aplicaciones
- Gestión de identidades y accesos (IAM)
- Configuración del sistema operativo (parches, actualizaciones) en EC2
- Configuración de red (Security Groups, NACLs)
- Configuración del firewall

### Tipos de responsabilidad según el servicio

| Modelo | Responsabilidad del cliente |
|-------|------------------------|
| **IaaS (EC2)** | Máxima — SO, parches, redes, firewall, datos |
| **PaaS (Beanstalk, RDS)** | Media — Datos, código, configuración de la app |
| **SaaS (p. ej., S3)** | Mínima — Datos y permisos de acceso |

### Responsabilidad compartida para el cómputo
- **EC2 (IaaS):** El cliente gestiona SO, parches, seguridad, datos
- **Lambda (Serverless):** AWS gestiona casi todo, el cliente solo su código y datos
- **ECS/EKS (contenedores):** Depende de si usas EC2 (más responsabilidad) o Fargate (menos)

---

## 10. Cómputo

### VMs, contenedores y serverless
| Tipo | Descripción | Servicio de AWS |
|------|-------------|-------------|
| **Máquinas virtuales** | Servidor virtual completo con SO | EC2 |
| **Contenedores** | Empaquetado ligero de aplicación + dependencias | ECS, EKS, Fargate |
| **Serverless** | Ejecutar código sin gestionar servidores | Lambda |

### Servicios de cómputo de AWS
- **EC2** (Elastic Compute Cloud): Máquinas virtuales en la nube, gran variedad de tipos de instancia
- **ECS** (Elastic Container Service): Orquestación de contenedores Docker, nativo de AWS
- **EKS** (Elastic Kubernetes Service): Kubernetes administrado en AWS
- **Fargate**: Motor serverless para contenedores (sin instancias EC2 que gestionar)
- **Lambda**: Funciones serverless, paga solo por ejecución (máx. 15 minutos)
- **Elastic Beanstalk**: PaaS — sube tu código y AWS gestiona el resto
- **AWS Batch**: Procesa cargas de trabajo por lotes a gran escala
- **Lightsail**: VPS simplificado para proyectos pequeños (alternativa sencilla a EC2)

### Computación de alto rendimiento (HPC)
- **AWS ParallelCluster**: Crear y gestionar clústeres HPC
- **AWS Batch**: Para trabajos por lotes masivos
- **Instancias P y G**: GPUs NVIDIA para ML, renderizado, simulación
- **Elastic Fabric Adapter (EFA)**: Interfaz de red para HPC con latencia ultrabaja

### Computación de borde e híbrida
- **AWS Outposts**: Infraestructura de AWS en tu centro de datos
- **AWS Wavelength**: Cómputo en el borde de las redes 5G
- **AWS Local Zones**: Extensión de región para baja latencia
- **AWS IoT Greengrass**: Cómputo local en dispositivos IoT
- **AWS Snow Family**: Dispositivos físicos para computación de borde y transferencia de datos

### Gestión de costos y capacidad
- **AWS Savings Plans**: Descuentos por compromiso de uso (1 o 3 años)
- **Spot Instances**: Hasta 90 % de descuento por capacidad no utilizada
- **Reserved Instances**: Descuento por compromiso de uso
- **AWS Compute Optimizer**: Recomienda el tipo de instancia óptimo según el uso real

---

## 11. Servicios de almacenamiento

### Amazon S3 (Simple Storage Service)
- **Almacenamiento de objetos** (archivos) — prácticamente ilimitado
- Los objetos se almacenan en **Buckets**
- Cada objeto puede ser de hasta **5 TB**
- Durabilidad: **99,999999999 % (11 nueves)**
- Casos de uso: copias de seguridad, hosting estático, data lakes, archivos multimedia

### Clases de almacenamiento de S3
| Clase | Caso de uso | Costo |
|-------|----------|------|
| **S3 Standard** | Datos de acceso frecuente | Mayor costo de almacenamiento |
| **S3 Intelligent-Tiering** | Mueve datos automáticamente entre niveles según los patrones de acceso | Costo de monitoreo |
| **S3 Standard-IA** | Datos de acceso poco frecuente | Menor costo de almacenamiento, mayor costo de acceso |
| **S3 One Zone-IA** | Datos poco frecuentes y no críticos (una sola AZ) | Aún más barato |
| **S3 Glacier Instant Retrieval** | Archivos con acceso inmediato | Muy barato de almacenar |
| **S3 Glacier Flexible Retrieval** | Archivos con recuperación en minutos u horas | Más barato |
| **S3 Glacier Deep Archive** | Archivos de largo plazo (7-10 años), recuperación en 12 horas | El más barato |

### AWS Snow Family
- Dispositivos físicos para **transferir grandes volúmenes de datos** o computar en el borde

| Dispositivo | Capacidad | Uso |
|--------|----------|-----|
| **Snowcone** | 8-14 TB | Transferencias pequeñas, computación de borde |
| **Snowball Edge** | 80 TB (almacenamiento) / 42 TB (cómputo) | Transferencias medianas, borde |
| **Snowmobile** | 100 PB | Migraciones masivas (un camión literal) |

### Otros servicios de almacenamiento
- **EBS (Elastic Block Store)**: Disco duro virtual para EC2. Persistente. Una sola AZ. Tipos: gp3, io2, st1, sc1
- **EFS (Elastic File System)**: Sistema de archivos compartido (NFS) para Linux. Multi-AZ. Escala automáticamente
- **FSx**: Sistemas de archivos administrados (Windows File Server, Lustre, NetApp ONTAP, OpenZFS)
- **AWS Storage Gateway**: Conecta tu almacenamiento on-premise con la nube (File Gateway, Volume Gateway, Tape Gateway)
- **AWS Backup**: Servicio centralizado para respaldar automáticamente recursos de AWS

---

## 12. Bases de datos

### Tipos de bases de datos

#### Data Warehouse
- Base de datos optimizada para **analítica** (OLAP — Online Analytical Processing)
- Almacena grandes volúmenes de datos históricos
- **Amazon Redshift** es el data warehouse de AWS
- Almacenamiento columnar para consultas rápidas sobre grandes conjuntos de datos

#### Key-Value Store (almacén clave-valor)
- Base de datos NoSQL simple: clave -> valor
- Extremadamente rápida y escalable
- **Amazon DynamoDB** es el servicio de AWS (escala horizontal)

#### Document Database (base de datos de documentos)
- Almacena datos en formato de documento (JSON, BSON)
- Flexible, sin esquema fijo
- **Amazon DocumentDB** (compatible con MongoDB)

### Servicios de bases de datos NoSQL
- **DynamoDB**: BD clave-valor y de documentos serverless. Latencia de milisegundos. Escala automáticamente en horizontal
- **DocumentDB**: Compatible con MongoDB
- **Amazon Keyspaces**: Compatible con Apache Cassandra
- **Neptune**: Base de datos de grafos (relaciones complejas, redes sociales)
- **Amazon QLDB**: Base de datos de libro mayor (ledger) inmutable y verificable (similar a blockchain)
- **ElastiCache**: Caché en memoria (Redis / Memcached). Latencia de microsegundos
- **Amazon MemoryDB for Redis**: Base de datos en memoria duradera compatible con Redis

### Servicios de bases de datos relacionales (RDBMS)
- **Amazon RDS** (Relational Database Service):
  - Admite: MySQL, PostgreSQL, MariaDB, Oracle, SQL Server
  - Administrado por AWS (copias de seguridad, parches, réplicas)
  - Multi-AZ para alta disponibilidad
- **Amazon Aurora**:
  - Compatible con MySQL y PostgreSQL
  - **5 veces más rápido que MySQL, 3 veces más rápido que PostgreSQL**
  - Escala automáticamente hasta 128 TB
  - Aurora Serverless: escala automáticamente la capacidad de cómputo
- **Amazon Aurora Global Database**: Replica entre múltiples regiones para DR (recuperación ante desastres)

### Otros servicios de bases de datos
- **Redshift**: Data warehouse columnar a escala de petabytes
- **Redshift Serverless**: Redshift sin gestionar clústeres
- **Amazon Timestream**: Base de datos de series temporales
- **DMS (Database Migration Service)**: Migra bases de datos a AWS con mínimo tiempo de inactividad

---

## 13. Redes

### Servicios de red nativos de la nube
- **VPC** (Virtual Private Cloud): Tu red virtual privada en AWS
- **Subnets (subredes)**: Segmentos dentro de tu VPC (públicos y privados)
- **Internet Gateway**: Permite que tu VPC se conecte a Internet
- **NAT Gateway**: Permite que las subredes privadas accedan a Internet (solo salida)
- **Route Tables (tablas de rutas)**: Definen las rutas de tráfico dentro de tu VPC

### Servicios de red empresariales/híbridos
- **AWS Direct Connect**: Conexión privada dedicada a AWS
- **AWS VPN (Site-to-Site)**: VPN cifrada entre tu red y AWS a través de Internet
- **AWS Transit Gateway**: Concentrador central para conectar múltiples VPCs y redes on-premise
- **AWS PrivateLink**: Accede a los servicios de AWS de forma privada sin salir a Internet

### VPC y subredes
- La **VPC** abarca una región completa
- Las **subredes** existen dentro de una AZ específica
- **Subred pública:** Tiene una ruta al Internet Gateway (recursos accesibles desde Internet)
- **Subred privada:** Sin ruta directa a Internet (bases de datos, servidores de aplicaciones)

### Security Groups vs. NACLs
| Característica | Security Groups | NACLs |
|---------|----------------|-------|
| Nivel | Instancia (ENI) | Subred |
| Estado | **Con estado (stateful)** (el tráfico de retorno es automático) | **Sin estado (stateless)** (debes definir reglas de entrada Y de salida) |
| Reglas | Solo ALLOW | ALLOW y DENY |
| Evaluación | Se evalúan todas las reglas | Reglas evaluadas en **orden numérico** |
| Por defecto | Deniega todo el tráfico entrante, permite todo el saliente | Permite todo el tráfico entrante y saliente |

### AWS CloudFront
- El **CDN (Content Delivery Network)** global de AWS
- Distribuye contenido desde **Edge Locations** cercanas al usuario
- Reduce la latencia y mejora el rendimiento
- Protección DDoS integrada (AWS Shield)
- Funciona con S3, EC2, ALB y orígenes personalizados
- Admite HTTPS, geo-restricción y caché configurable

---

## 14. EC2

### Familias de instancias EC2
| Familia | Optimizada para | Ejemplo |
|--------|--------------|---------|
| **Propósito general (T, M)** | Equilibrio de cómputo, memoria y redes | t3.micro, m6i.large |
| **Optimizada para cómputo (C)** | Cómputo intensivo, batch, gaming | c6i.xlarge |
| **Optimizada para memoria (R, X, z)** | Bases de datos en memoria, cachés | r6i.large, x2idn |
| **Optimizada para almacenamiento (I, D, H)** | Alta E/S secuencial, data warehouses | i3.large |
| **Cómputo acelerado (P, G, Inf, Trn)** | ML, GPU, HPC, video | p4d.24xlarge |

### Tipos de instancias EC2 — Convención de nomenclatura
- Formato: `m5.xlarge`
  - `m` = familia (propósito general)
  - `5` = generación
  - `xlarge` = tamaño (nano, micro, small, medium, large, xlarge, 2xlarge, etc.)

### Dedicated Hosts vs. Dedicated Instances
| | Dedicated Host | Dedicated Instance |
|--|---------------|-------------------|
| **Hardware** | Servidor físico completo para ti | Instancia sobre hardware dedicado |
| **Visibilidad** | Ves sockets, núcleos, host ID | No ves los detalles del hardware |
| **Licenciamiento** | Puedes traer tus propias licencias (BYOL) | No |
| **Costo** | Más caro | Menos caro |

### Tenencia de EC2 (Tenancy)
- **Compartida (por defecto):** Tu instancia comparte hardware con otros clientes
- **Dedicated Instance:** Hardware dedicado, pero gestionado por AWS
- **Dedicated Host:** Servidor físico completo para ti, con visibilidad del hardware

### Lanzar una EC2 — Conceptos clave
- **AMI** (Amazon Machine Image): Plantilla del SO y el software
- **Key Pair**: Para acceso SSH (Linux) o acceso RDP (Windows)
- **Security Group**: Firewall de la instancia
- **User Data**: Script que se ejecuta cuando se lanza la instancia
- **Instance Profile / IAM Role**: Permisos de AWS para la instancia

### Auto Scaling Group (ASG)
- Escala automáticamente el número de instancias EC2 según la demanda
- Define: número **mínimo, deseado y máximo** de instancias
- Políticas de escalado: Target Tracking, Step Scaling, Scheduled
- Reemplaza automáticamente las instancias que fallan (health checks)

### Application Load Balancer (ALB)
- Distribuye el tráfico entre múltiples instancias EC2
- Opera en la **capa 7** (HTTP/HTTPS)
- Admite enrutamiento basado en ruta, host y encabezado
- Integrado con los Auto Scaling Groups
- Otros LBs: NLB (capa 4, TCP/UDP), CLB (heredado), GLB (capa 3, appliances)

---

## 15. Modelos de precios de EC2

### On-Demand
- Paga por **hora o segundo** sin compromiso
- Sin pago inicial
- Ideal para: cargas de trabajo impredecibles, desarrollo, pruebas
- La opción **más cara** a largo plazo

### Reserved Instances (RI)
- Descuento de **hasta 72 %** vs. On-Demand por un compromiso de 1 o 3 años
- **Pago:** All Upfront (mayor descuento) | Partial Upfront | No Upfront
- Ideal para cargas de trabajo **predecibles y de estado estable (steady-state)**

### Atributos de las Reserved Instances
- Tipo de instancia, plataforma (Linux/Windows), tenencia, región/AZ

### RI regional vs. zonal
- **RI regional:** El descuento aplica a cualquier AZ de la región. NO incluye reserva de capacidad
- **RI zonal:** El descuento solo aplica en la AZ especificada. SÍ incluye reserva de capacidad

### Límites de RI
- Máximo 20 RIs por región por defecto (puedes solicitar un aumento)

### Reservas de capacidad (Capacity Reservations)
- Reserva capacidad de EC2 en una AZ específica sin compromiso de tiempo
- Pagas el precio On-Demand esté o no la instancia en ejecución
- Útil cuando necesitas garantizar disponibilidad

### RI Standard vs. Convertible
| | Standard RI | Convertible RI |
|--|------------|----------------|
| **Descuento** | Hasta 72 % | Hasta 66 % |
| **Cambiar atributos** | No | Sí (familia, SO, tenencia) |
| **Vender en el Marketplace** | Sí | No |

### RI Marketplace
- Puedes **vender tus RIs no utilizadas** a otros clientes de AWS
- Solo se pueden vender las RIs Standard

### Spot Instances
- Hasta **90 % de descuento** vs. On-Demand
- Usas la **capacidad no utilizada** de AWS
- **AWS puede recuperar tu instancia con 2 minutos de aviso**
- Ideal para: procesamiento por lotes, big data, CI/CD, cargas de trabajo tolerantes a fallos
- **NO usar para:** bases de datos, cargas de trabajo críticas

### Dedicated
- **Dedicated Instances:** Hardware dedicado, costo por instancia + cargo por región
- **Dedicated Hosts:** Servidor físico completo, útil para BYOL (Bring Your Own License)

### Savings Plans
- Descuento de hasta **72 %** vs. On-Demand por un compromiso de uso ($/hora) por 1 o 3 años
- **Compute Savings Plan:** Aplica a EC2, Lambda, Fargate. El más flexible
- **EC2 Instance Savings Plan:** Solo EC2, especificas familia e instancia. Mayor descuento
- Más flexible que las Reserved Instances

---

## 16. Identidad

### Modelo Zero-Trust
- Modelo de seguridad: **"Nunca confíes, siempre verifica"**
- Cada solicitud se autentica y autoriza sin importar de dónde provenga
- Principios: verificación continua, mínimo privilegio, asumir la brecha (assume breach)

### Zero-Trust en AWS
- Se implementa usando una combinación de servicios: IAM, VPC, Security Groups, AWS SSO
- AWS no tiene un único servicio "Zero Trust", sino una combinación de servicios

### Directory Services
- **AWS Directory Service**: Active Directory administrado en AWS
- Opciones: AWS Managed Microsoft AD, AD Connector, Simple AD

### Active Directory
- Servicio de directorio de Microsoft para gestionar usuarios y permisos en una red empresarial
- Base de la autenticación corporativa en Windows

### Proveedores de identidad (IdP)
- Sistemas que manejan la autenticación y la pasan a tu aplicación
- Protocolos: **SAML 2.0**, **OpenID Connect (OIDC)**, **OAuth 2.0**
- Ejemplos: Okta, Auth0, AWS SSO, Google, Facebook

### Single Sign-On (SSO)
- Inicia sesión una vez y accede a múltiples aplicaciones sin volver a autenticarte
- **AWS IAM Identity Center** (antes AWS SSO): SSO para múltiples cuentas y aplicaciones de AWS

### LDAP
- Protocolo para consultar y modificar directorios de usuarios
- Base de Active Directory

### Autenticación multifactor (MFA)
- Requiere **dos o más factores** para autenticarse: algo que sabes (contraseña) + algo que tienes (token/teléfono)
- **Habilita siempre MFA**, especialmente en la cuenta root

### Llaves de seguridad
- Dispositivos físicos para MFA (YubiKey, FIDO2)
- Más seguras que las aplicaciones de autenticación
- Resistentes al phishing

### AWS IAM (Identity and Access Management)
- Servicio **gratuito** y **global** para controlar el acceso a los recursos de AWS
- Componentes principales:
  - **Users (usuarios)**: Personas o aplicaciones
  - **Groups (grupos)**: Colección de usuarios (p. ej., Developers, Admins)
  - **Roles**: Permisos temporales asignables a servicios o usuarios
  - **Policies (políticas)**: Documentos JSON que definen permisos (Allow/Deny)

### Anatomía de una política de IAM
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-bucket/*"
    }
  ]
}
```
- **Effect:** Allow o Deny
- **Action:** Qué operaciones se permiten/deniegan
- **Resource:** A qué recursos aplica (ARN)
- **Condition (opcional):** Condiciones adicionales

### Principio de mínimo privilegio
- Otorga solo los **permisos mínimos necesarios** para realizar una tarea
- Concepto de seguridad fundamental en AWS
- Empieza sin permisos y añade solo lo necesario

### Usuario root de la cuenta de AWS
- Usuario con **acceso completo y sin restricciones** a todos los recursos
- Se crea cuando se crea la cuenta de AWS
- **Tareas exclusivas de root:** cambiar el plan de soporte, cerrar la cuenta, cambiar la configuración de la cuenta
- **Nunca uses root para tareas diarias** — crea usuarios de IAM
- **Habilita siempre MFA en root**

### AWS SSO (IAM Identity Center)
- Servicio para gestionar el acceso SSO a múltiples cuentas de AWS y aplicaciones de negocio
- Se integra con Active Directory y proveedores de identidad SAML 2.0
- Portal centralizado para que los usuarios accedan a todas sus cuentas

---

## 17. Integración de aplicaciones

### Colas y Amazon SQS
- **Amazon SQS** (Simple Queue Service): Servicio de colas de mensajes totalmente administrado
- Desacopla los componentes de la aplicación
- **Standard Queue:** Ordenamiento de mejor esfuerzo, rendimiento ilimitado
- **FIFO Queue:** Ordenamiento estricto (First-In-First-Out), 300 msg/seg
- Los mensajes persisten hasta que se procesan o expiran

### Streaming y Amazon Kinesis
- **Amazon Kinesis**: Procesamiento de datos en streaming **en tiempo real**
- **Kinesis Data Streams**: Ingesta de streaming en tiempo real
- **Kinesis Data Firehose**: Carga datos de streaming a S3, Redshift, etc.
- **Kinesis Data Analytics**: Analítica SQL/Apache Flink sobre datos de streaming
- Casos de uso: logs en tiempo real, IoT, analítica de clickstream

### Pub/Sub y Amazon SNS
- **Amazon SNS** (Simple Notification Service): Servicio Pub/Sub (publicación/suscripción)
- Un publicador envía un mensaje a un **Topic (tema)**
- Todos los suscriptores del Topic reciben el mensaje
- Suscriptores: correo electrónico, SMS, Lambda, SQS, endpoints HTTP, push móvil
- Útil para alertas, notificaciones, fan-out

### API Gateway y Amazon API Gateway
- **Amazon API Gateway**: Crea, publica y gestiona APIs (REST, HTTP, WebSocket)
- Maneja autenticación, limitación de tasa (rate limiting), caché, transformación
- Se integra con Lambda para crear APIs serverless

### Máquinas de estado y AWS Step Functions
- **AWS Step Functions**: Orquesta múltiples servicios de AWS en flujos de trabajo
- Define flujos usando **Amazon States Language** (JSON) o el Workflow Studio visual
- Ideal para coordinar microservicios y procesos complejos

### Bus de eventos y Amazon EventBridge
- **Amazon EventBridge** (antes CloudWatch Events): Bus de eventos serverless
- Conecta aplicaciones usando eventos de AWS, SaaS o tus propias apps
- Enrutamiento basado en reglas
- Ideal para arquitecturas basadas en eventos

### Otros servicios de integración de aplicaciones
- **Amazon MQ**: Broker de mensajes administrado (ActiveMQ, RabbitMQ) para migraciones on-premise
- **AWS AppSync**: API GraphQL administrada, sincronización en tiempo real
- **Amazon AppFlow**: Integración de datos entre SaaS (Salesforce, SAP) y AWS

---

## 18. Contenedores

### VMs vs. contenedores
| Característica | VMs | Contenedores |
|---------|-----|-----------|
| **Aislamiento** | Completo (SO propio) | Comparten el kernel del host |
| **Tamaño** | GBs | MBs |
| **Arranque** | Minutos | Segundos |
| **Sobrecarga (overhead)** | Alta | Baja |
| **Densidad** | Menos VMs por host | Muchos contenedores por host |

### Microservicios
- Arquitectura donde cada función de la aplicación es un servicio independiente
- Cada microservicio puede desplegarse, escalarse y actualizarse de forma independiente
- Los contenedores son ideales para microservicios

### Kubernetes
- Plataforma de código abierto para orquestar contenedores
- Maneja el despliegue, escalado y las redes de los contenedores
- **AWS EKS** (Elastic Kubernetes Service): Kubernetes administrado en AWS

### Docker
- Plataforma de código abierto para construir, empaquetar y ejecutar aplicaciones en contenedores
- **Dockerfile**: Define cómo construir la imagen
- **Docker Image**: Plantilla inmutable
- **Docker Container**: Instancia en ejecución de una imagen
- **Amazon ECR** (Elastic Container Registry): Repositorio privado de imágenes Docker

### Podman
- Alternativa a Docker, sin daemon (daemonless), sin root (rootless) por defecto
- Compatible con imágenes y comandos de Docker

### Servicios de contenedores en AWS
- **ECS** (Elastic Container Service): Orquestación de contenedores nativa de AWS
- **EKS** (Elastic Kubernetes Service): Kubernetes administrado
- **Fargate**: Motor serverless para contenedores (sin gestión de EC2)
- **ECR** (Elastic Container Registry): Registro de imágenes Docker
- **AWS App Runner**: Despliegue simplificado de contenedores/código fuente (similar a PaaS)
- **AWS Copilot**: CLI para desplegar contenedores fácilmente en ECS/Fargate

---

## 19. Gobernanza

### Organizations y cuentas
- **AWS Organizations**: Gestiona de forma centralizada múltiples cuentas de AWS
- **Root Account User**: Acceso completo a todos los servicios de AWS
- **Organizational Units (OUs)**: Agrupación lógica de cuentas
- **Service Control Policies (SCPs)**: Políticas que restringen lo que pueden hacer las cuentas
- **Consolidated Billing**: Factura única para todas las cuentas + descuentos por volumen
- Estructura típica: Root Account > OUs > Member Accounts

### AWS Control Tower
- Configura y gobierna un entorno multicuenta **seguro y conforme (compliant)**
- Automatiza la creación de cuentas con buenas prácticas
- **Guardrails**: Reglas de gobernanza (preventivas y detectivas)
- Usa: AWS Organizations, AWS SSO, AWS Config, CloudTrail
- **Landing Zone**: Entorno multicuenta bien configurado y creado automáticamente

### AWS Config
- Servicio que **audita y evalúa la configuración** de tus recursos de AWS por región
- Es Compliance-as-Code (CaC)
- Se usa para configurar recursos de una forma específica
- Lleva el seguimiento de los cambios de configuración
- Lista de todos los recursos de una región
- No previene los cambios, solo los **detecta e informa**

### AWS Quick Starts
- Plantillas de CloudFormation y guías de despliegue creadas por AWS y sus socios
- Despliega arquitecturas populares en minutos
- Disponibles en la **AWS Solutions Library**

### Etiquetado (Tagging)
- Las **Tags (etiquetas)** son pares clave-valor que asignas a los recursos de AWS
- P. ej., `Environment: Production`, `Team: DevOps`, `Project: WebApp`
- Usos: organización, control de costos, automatización, control de acceso
- **Buena práctica:** Define una estrategia de etiquetado consistente

### Resource Groups
- Colección de recursos de AWS agrupados por etiquetas
- Permite ver y gestionar recursos relacionados como una unidad
- **Tag Editor**: Herramienta para buscar y etiquetar recursos de forma masiva

### Servicios centrados en el negocio
- **Amazon Connect**: Centro de contacto basado en la nube
- **Amazon WorkSpaces**: Escritorios virtuales (VDI)
- **Amazon WorkDocs**: Almacenamiento y uso compartido de documentos empresariales
- **Amazon Chime**: Videoconferencias y chat
- **Amazon WorkMail**: Correo electrónico empresarial administrado
- **Amazon Pinpoint**: Servicio de marketing para enviar correo dirigido vía SMS
- **Amazon Email Service (SES)**: Servicio de correo transaccional
- **Amazon QuickSight**: Servicio de inteligencia de negocio (BI)

---

## 20. Aprovisionamiento

### Servicios de aprovisionamiento
La asignación o creación de recursos y servicios para un cliente.

| Servicio                            | Descripción                                    |
| ----------------------------------- | --------------------------------------------- |
| **CloudFormation**                  | IaC con plantillas YAML/JSON                   |
| **Elastic Beanstalk**               | PaaS — sube tu código                          |
| **AWS OpsWorks**                    | Gestión de configuración con Chef y Puppet     |
| **AWS QuickStarts**                 | Paquetes prediseñados para lanzar y configurar |
| **AWS Marketplace**                 | Catálogo digital de listados de software       |
| **AWS Amplify**                     | Un framework de aplicaciones móviles y web     |
| **AWS App Runner**                  | Facilita el despliegue de contenedores         |
| **AWS Copilot**                     | CLI para lanzar y gestionar aplicaciones rápidamente |
| **AWS CodeStar**                    | Interfaz de usuario para gestionar el desarrollo de software |
| **AWS Cloud Development Kit (CDK)** | Herramienta de IaC para usar cualquier lenguaje de programación |

### AWS Elastic Beanstalk
- **PaaS** (Plataforma como Servicio) de AWS
- No recomendado para producción (solo para grandes empresas)
- Sube tu código y Beanstalk automáticamente:
  - Aprovisiona EC2, Load Balancers, Auto Scaling...
  - Configura monitoreo y logging
  - Gestiona despliegues y reversiones (rollbacks)
- Admite: Java, .NET, PHP, Node.js, Python, Ruby, Go, Docker
- Conservas el control total sobre los recursos subyacentes si lo necesitas
- **Gratuito** — solo pagas por los recursos creados (EC2, RDS, etc.)

---

## 21. Serverless

### Servicios serverless en AWS
El CSP se encarga de los servidores subyacentes, la infraestructura y el sistema operativo.

| Servicio              | Función                                                                              |
| --------------------- | ----------------------------------------------------------------------------------- |
| **AWS Lambda**        | Ejecuta código sin servidores. Máx. 15 min por ejecución. Paga por invocación y duración |
| **ECS Fargate**       | Servicio de orquestación de contenedores serverless                                 |
| **Amazon S3**         | Almacenamiento de objetos serverless                                                |
| **DynamoDB**          | Base de datos NoSQL serverless                                                       |
| **Aurora Serverless** | Versión serverless bajo demanda de Aurora (base de datos relacional)                |
| **Amazon SQS**        | Cola de mensajes serverless                                                          |
| **Amazon SNS**        | Notificaciones serverless                                                            |
| **API Gateway**       | APIs serverless                                                                      |
| **Step Functions**    | Servicio de máquina de estados                                                       |
| **EventBridge**       | Bus de eventos serverless                                                            |
| **Amazon Cognito**    | Autenticación de usuarios serverless                                                 |

**Serverless = Sin gestión de servidores, escala automáticamente, paga por uso**

---

## 22. Windows en AWS

### EC2 Windows
- Puedes lanzar instancias EC2 con Windows Server
- Licencia de Windows incluida en el precio de la instancia (License Included)
- Acceso vía **RDP** (Remote Desktop Protocol) puerto 3389
- Admite: IIS, SQL Server, Active Directory, .NET Framework

### AWS License Manager
- Gestiona licencias de software de Microsoft, Oracle, SAP, etc.
- Para las licencias de Microsoft Windows Server y Microsoft SQL Server necesitas usar un **Dedicated Host**
- Opciones:
  - **License Included (LI):** AWS proporciona la licencia
  - **Bring Your Own License (BYOL):** Trae tus licencias existentes

---

## 23. Registro (Logging)

### AWS CloudTrail
- Registra **todas las llamadas a la API** realizadas en tu cuenta de AWS
- Responde: Dónde, Cuándo, Quién y Qué
- Esencial para auditoría, cumplimiento y seguridad
- Los trails se guardan en S3; para analizarlos usa **Amazon Athena**
- **CloudTrail es para AUDITORÍA (quién hizo qué)**

### Amazon CloudWatch
- Servicio de **monitoreo y observabilidad** de AWS
- Componentes principales: Logs, Metrics, Events, Alarms, Dashboards

#### CloudWatch Alarms
- Alerta cuando una métrica cruza un umbral definido
- Acciones: notificación SNS, Auto Scaling, acción de EC2 (detener, terminar, reiniciar)
- **Anatomía de una alarma:**
  - Métrica (p. ej., CPU Utilization)
  - Umbral (p. ej., > 80 %)
  - Período de evaluación (p. ej., 5 minutos)
  - Acción (p. ej., enviar correo vía SNS)

#### CloudWatch Logs
- **Log Events**: Registros individuales de actividad
- **Log Groups**: Colección de Log Streams de la misma fuente
- **Log Streams**: Secuencia de Log Events de una fuente específica
- Puedes configurar la retención (de 1 día a 10 años o que nunca expire)

#### CloudWatch Logs Insights
- Consulta y analiza logs usando un lenguaje de consulta interactivo
- Busca patrones, filtra y agrega datos de logs

#### CloudWatch Metrics
- Métricas de rendimiento de los servicios de AWS
- Métricas por defecto: CPU, NetworkIn/Out, DiskRead/Write
- **Custom Metrics**: Tus propias métricas mediante la API PutMetricData

**Resumen:**
- **CloudTrail** = AUDITORÍA (quién hizo qué)
- **CloudWatch** = MONITOREO (cómo se están desempeñando los recursos)

---

## 24. ML, IA y Big Data

### Introducción a ML e IA
- **IA (Inteligencia Artificial):** Máquinas que imitan la inteligencia humana
- **ML (Machine Learning):** Subconjunto de la IA; las máquinas aprenden de los datos sin ser programadas explícitamente
- **Deep Learning:** Subconjunto del ML que usa redes neuronales profundas

### Servicios de IA y ML en AWS
| Servicio                      | Función                                                           |
| ----------------------------- | ----------------------------------------------------------------- |
| **Amazon SageMaker**          | Plataforma completa para construir, entrenar y desplegar modelos de ML |
| **Amazon Rekognition**        | Análisis de imágenes y video (detección de rostros, objetos, texto) |
| **Amazon Transcribe**         | Speech-to-Text (audio a texto)                                    |
| **Amazon Polly**              | Text-to-Speech (texto a voz)                                      |
| **Amazon Translate**          | Traducción automática de idiomas                                  |
| **Amazon Comprehend**         | Procesador de lenguaje natural (NLP). Analiza datos.              |
| **Amazon Lex**                | Chatbots conversacionales (la tecnología detrás de Alexa)         |
| **Amazon Textract**           | Extrae texto y datos de documentos/PDFs                           |
| **Amazon Forecast**           | Predicciones de series temporales mediante ML                     |
| **Amazon Personalize**        | Recomendaciones personalizadas (como Amazon.com)                  |
| **Amazon Kendra**             | Búsqueda empresarial inteligente impulsada por ML                 |
| **Amazon CodeWhisperer**      | Asistente de programación con IA (sugerencias de código)          |
| **Amazon Bedrock**            | Acceso a modelos fundacionales de IA generativa de múltiples proveedores |
| **Amazon Deep Learning AMIs** | Preinstaladas con frameworks populares de deep learning           |

### Servicios de Big Data y analítica
Big Data: Término para describir volúmenes masivos de datos estructurados/no estructurados

| Servicio               | Función                                                                |
| ---------------------- | --------------------------------------------------------------------- |
| **Amazon Redshift**    | Data warehouse a escala de petabytes para analítica                   |
| **Amazon Athena**      | Consultas SQL sobre datos de S3 (serverless, paga por consulta)       |
| **Amazon EMR**         | Hadoop/Spark administrado para procesamiento de big data              |
| **Amazon Kinesis**     | Procesamiento de streaming en tiempo real                            |
| **AWS Glue**           | ETL (Extract, Transform, Load) serverless + Data Catalog             |
| **Amazon OpenSearch**  | Búsqueda y analítica de logs (antes ElasticSearch)                   |
| **Amazon QuickSight**  | BI (Business Intelligence) — paneles y visualizaciones serverless    |
| **AWS Data Pipeline**  | Orquestación del movimiento y la transformación de datos             |
| **AWS Lake Formation** | Crear y gestionar Data Lakes de forma segura                         |
| **Amazon MSK**         | Apache Kafka administrado                                            |
| **Amazon CloudSearch** | Servicio de búsqueda de texto completo                              |
| **Amazon Bedrock**     | LLM para generar respuestas de texto e imágenes                     |

### Amazon QuickSight
- Servicio de **inteligencia de negocio (BI) serverless**
- Crea paneles y visualizaciones interactivos
- Se conecta a: S3, RDS, Redshift, Athena y más
- Tecnología **SPICE** (Super-fast, Parallel, In-memory Calculation Engine)
- Paga por sesión (por uso)

### IA generativa
- **Amazon Bedrock**: Acceso a modelos fundacionales (FM) de AI21 Labs, Anthropic, Cohere, Meta, Stability AI y Amazon Titan
- Permite construir aplicaciones de IA generativa sin entrenar modelos desde cero
- **Amazon CodeWhisperer**: Programador en pareja (pair programmer) con IA para sugerencias de código

### Frameworks de ML y DL
- AWS admite: TensorFlow, PyTorch, Apache MXNet
- **AWS Deep Learning AMIs**: AMIs preconfiguradas con frameworks de ML
- **AWS Deep Learning Containers**: Contenedores Docker con frameworks de ML

### GPUs en AWS
- Instancias con GPUs NVIDIA para entrenamiento/inferencia de ML
- **CUDA**: Plataforma de computación paralela de NVIDIA para GPUs
- Familias: P (entrenamiento), G (gráficos/inferencia), Inf (Inferentia), Trn (Trainium)
- **AWS Trainium**: Chip diseñado por AWS para el entrenamiento de ML
- **AWS Inferentia**: Chip diseñado por AWS para la inferencia de ML

---

## 25. AWS Well-Architected Framework

### Panorama general
- Guía de **buenas prácticas** para diseñar sistemas en la nube
- Creada por los Solutions Architects de AWS con experiencia del mundo real
- Ayuda a evaluar y mejorar tus arquitecturas

### Principios generales de diseño
1. Deja de adivinar tus necesidades de capacidad
2. Prueba los sistemas a escala de producción
3. Automatiza para facilitar la experimentación arquitectónica
4. Permite arquitecturas evolutivas
5. Impulsa las arquitecturas usando datos
6. Mejora mediante Game Days (simulaciones)

### Los 6 pilares del Well-Architected Framework

#### 1. Excelencia operativa
- Ejecutar y monitorear sistemas para entregar valor de negocio
- Mejora continua de procesos y procedimientos
- Principios clave: operaciones como código, cambios pequeños, frecuentes y reversibles, anticipar la falla
- Servicios: CloudFormation, Config, CloudTrail, CloudWatch, X-Ray

#### 2. Seguridad
- Proteger información, sistemas y activos
- Principios clave: implementar una base de identidad sólida, trazabilidad, seguridad en todas las capas, automatizar buenas prácticas, proteger los datos en tránsito y en reposo, prepararse para eventos de seguridad
- Servicios: IAM, CloudTrail, KMS, WAF, Shield, GuardDuty, Inspector, Macie

#### 3. Fiabilidad
- Capacidad de recuperarse de fallas y escalar para satisfacer la demanda
- Principios clave: probar los procedimientos de recuperación, escalar horizontalmente, dejar de adivinar la capacidad, automatizar los cambios, recuperación automática
- Servicios: CloudWatch, CloudFormation, S3, Glacier, Route 53

#### 4. Eficiencia del rendimiento
- Usar los recursos de cómputo de manera eficiente y mantener la eficiencia con el tiempo
- Principios clave: democratizar las tecnologías avanzadas, volverse global en minutos, usar arquitecturas serverless, experimentar con frecuencia
- Servicios: Auto Scaling, Lambda, EBS, S3, RDS, CloudFront

#### 5. Optimización de costos
- Evitar gastos innecesarios
- Principios clave: implementar la gestión financiera de la nube (Cloud Financial Management), adoptar un modelo de consumo, medir la eficiencia, dejar de gastar en trabajo pesado no diferenciado
- Servicios: Cost Explorer, Budgets, Reserved Instances, Spot Instances, Trusted Advisor

#### 6. Sostenibilidad (nuevo en el WAF)
- Minimizar el impacto ambiental de las cargas de trabajo en la nube
- Principios: entender tu impacto, establecer objetivos de sostenibilidad, maximizar la utilización, usar servicios administrados, reducir el impacto posterior (downstream)

### AWS Well-Architected Tool
- Herramienta **gratuita** en la consola de AWS
- Evalúa tu arquitectura frente a los 6 pilares respondiendo preguntas
- Genera un **informe con recomendaciones de mejora**
- Disponible en AWS Console > Well-Architected Tool

### AWS Architecture Center
- Recurso en línea con **diagramas de referencia, whitepapers y guías**
- Arquitecturas de referencia para casos de uso comunes
- https://aws.amazon.com/architecture/

---

## 26. TCO y migración

### Costo Total de Propiedad (TCO)
- Comparación financiera del **costo total** de on-premise vs. nube
- On-premise incluye: hardware, licencias, electricidad, refrigeración, personal, espacio físico, mantenimiento
- En la nube solo pagas por lo que usas, sin costos ocultos de infraestructura

### CAPEX vs. OPEX
|                     | CAPEX (Gasto de capital)                                                          | OPEX (Gasto operativo)                      |
| ------------------- | --------------------------------------------------------------------------------- | ------------------------------------------- |
| **Qué**             | Gasto de capital inicial (comprar servidores, centro de datos, seguridad física, hardware) | Gasto operativo continuo (pago por uso)     |
| **Nube**            | N/A                                                                               | La nube es OPEX — pagos mensuales           |
| **On-Premise**      | Alto CAPEX inicial                                                                | Menor OPEX pero costos fijos                |
| **Ventaja de la nube** | Sin inversión inicial                                                          | Flexible, escala con el negocio             |

### Reubicación del personal de TI
- Al migrar a la nube, el personal de TI pasa de mantener hardware a tareas de mayor valor
- Una empresa puede cambiar las actividades de sus empleados de **gestionar infraestructura a generar ingresos**
- Enfoque en arquitectura, automatización, optimización y seguridad

### AWS Pricing Calculator
- Herramienta para **estimar costos** de los servicios de AWS antes de usarlos
- Permite construir escenarios y comparar opciones
- https://calculator.aws/
- Reemplazo de la antigua Simple Monthly Calculator y la TCO Calculator

### Migration Evaluator
- Herramienta para crear un **caso de negocio** para la migración a AWS
- Analiza tu entorno on-premise actual
- Proporciona una proyección de costos en AWS
- Antes conocido como TSO Logic

### VM Import/Export
- Permite **importar** imágenes de VM de tu entorno a EC2
- Permite **exportar** instancias EC2 de vuelta a tu entorno
- Admite: VMware, Hyper-V, Citrix Xen

### Database Migration Service (DMS)
- Migra bases de datos a AWS con **mínimo tiempo de inactividad**
- Admite migraciones homogéneas (p. ej., MySQL a MySQL) y heterogéneas (p. ej., Oracle a Aurora)
- **AWS Schema Conversion Tool (SCT)**: Convierte esquemas de bases de datos para migraciones heterogéneas
- La base de datos de origen permanece operativa durante la migración

### Cloud Adoption Framework (AWS CAF)
- Guía de AWS para planificar la migración a la nube
- **6 perspectivas:**
  1. **Business (negocio)**: Alinear la TI con los objetivos del negocio
  2. **People (personas)**: Cultura, organización, capacitación
  3. **Governance (gobernanza)**: Gobernanza de TI, gestión de riesgos
  4. **Platform (plataforma)**: Arquitectura, patrones, servicios
  5. **Security (seguridad)**: Seguridad, cumplimiento, controles
  6. **Operations (operaciones)**: Operaciones en la nube, monitoreo

---

## 27. Facturación y precios

### Servicios gratuitos de AWS
Servicios de AWS que **no tienen costo** (pero los recursos que crean sí):
- IAM, VPC, Organizations, Consolidated Billing
- Elastic Beanstalk (solo pagas por los recursos), CloudFormation, Auto Scaling Groups
- Servicios de la AWS Free Tier

### Planes de soporte de AWS
| Plan | Costo | Características |
|------|------|----------|
| **Basic** | Gratis | Acceso a documentación, whitepapers, foros. Servicio al cliente 24/7 para facturación. Trusted Advisor (7 comprobaciones básicas). Personal Health Dashboard |
| **Developer** | Desde $29/mes | Todo lo de Basic + soporte técnico por correo electrónico (horario laboral). 1 contacto principal. Respuesta: < 24 h general, < 12 h sistema con problemas |
| **Business** | Desde $100/mes | Todo lo de Developer + soporte telefónico 24/7. Contactos ilimitados. **Todas las comprobaciones de Trusted Advisor**. Respuesta: < 1 h para sistema de producción caído. AWS Support API |
| **Enterprise On-Ramp** | Desde $5,500/mes | Todo lo de Business + grupo de Technical Account Managers. Respuesta: < 30 min para casos críticos de negocio. Concierge Support Team |
| **Enterprise** | Desde $15,000/mes | Todo lo anterior + **TAM dedicado**. Respuesta: < 15 min para casos críticos de negocio. Infrastructure Event Management. Well-Architected Reviews |

### TAM (Technical Account Manager)
- Disponible solo en los planes **Enterprise On-Ramp** y **Enterprise**
- Tu punto de contacto técnico dedicado en AWS
- Ayuda con buenas prácticas, optimización, planificación de arquitectura
- Coordina el acceso a programas y expertos de AWS

### AWS Marketplace
- Catálogo digital con **miles de listados de software** de proveedores independientes (ISVs)
- Categorías: seguridad, redes, almacenamiento, ML, DevOps, BI
- Modelos: AMI, SaaS, Contenedores, Servicios profesionales
- La facturación se integra con tu factura de AWS

### Consolidated Billing (facturación consolidada)
- Característica de **AWS Organizations**
- Factura única para todas las cuentas de la organización
- **Descuentos por volumen**: El uso combinado de todas las cuentas puede generar descuentos por volumen
- Simplifica el seguimiento de costos por cuenta

### AWS Trusted Advisor
- Servicio que **inspecciona tu entorno** y hace recomendaciones en 5 categorías:
  1. **Optimización de costos**: Recursos subutilizados, RIs no usadas
  2. **Rendimiento**: Cuellos de botella, límites de servicio
  3. **Seguridad**: Permisos abiertos, MFA no habilitado
  4. **Tolerancia a fallos**: Copias de seguridad, multi-AZ, redundancia
  5. **Límites de servicio**: Uso cercano a los límites de servicio
- **Basic/Developer:** 7 comprobaciones básicas (Core checks) que incluyen permisos de buckets de S3, Security Groups, uso de IAM, MFA en root, snapshots de EBS, snapshots de RDS, límites de servicio
- **Business/Enterprise:** **Todas las comprobaciones** + acceso a la API + integración con CloudWatch

### SLAs (Service Level Agreements)
- Acuerdos de nivel de servicio que AWS garantiza
- Si AWS no los cumple, recibes créditos de servicio
- Ejemplo: SLA de EC2 = 99,99 % de tiempo de actividad mensual
- Si el tiempo de actividad es < 99,99 %, recibes créditos de entre el 10-100 % de tu factura del servicio afectado

### SLI (Service Level Indicator)
- Métrica/medición que indica qué nivel de rendimiento está recibiendo un cliente
- Puede ser tiempo de actividad, rendimiento, disponibilidad, latencia...

### SLO (Service Level Objective)
- El objetivo que el proveedor ha acordado cumplir
- Se representa como un porcentaje objetivo específico durante un período de tiempo

### Ejemplos de SLA
| Servicio | SLA |
|---------|-----|
| EC2 | 99,99 % |
| S3 | 99,9 % (disponibilidad) |
| RDS Multi-AZ | 99,95 % |
| Lambda | 99,95 % |
| CloudFront | 99,9 % |

### Service Health Dashboard
- Muestra el estado de **todos los servicios de AWS** a nivel global
- Panorama de los incidentes actuales y pasados
- https://health.aws.amazon.com/health/status

### AWS Personal Health Dashboard
- Muestra los eventos que afectan a **tus recursos específicos**
- Alertas proactivas y personalizadas
- Accesible desde la consola como **AWS Health Dashboard**
- Muestra mantenimiento programado, problemas de rendimiento, etc.

### AWS Abuse
- Canal para reportar el **uso abusivo** de los recursos de AWS
- Reporta: spam, escaneo de puertos, DDoS, malware, contenido ilegal
- Contacto: email-abuse@amazon.com / trustandsafety@support.aws.com o formulario web en la consola

### AWS Free Tier
- Recordatorio: 3 tipos (Always Free, 6 meses gratis, Trials)
- $200 en créditos
- Consulta https://aws.amazon.com/free/ para detalles actualizados
- Configura **AWS Budgets** para evitar superar la capa gratuita

### AWS Credits
- Cupones aplicados a tu factura de AWS
- Se obtienen mediante: eventos, programas de AWS, AWS Activate (startups), promociones
- Se aplican automáticamente a tu factura

### AWS Partner Network (APN)
- Red global de socios de AWS
- **Technology Partners**: Proveedores de software/SaaS que se integran con AWS
- **Consulting Partners**: Firmas de consultoría que ayudan a migrar y usar AWS
- **Training Partners**: Organizaciones autorizadas para impartir capacitación de AWS

### AWS Budgets
- Crea presupuestos de **costo, uso o reserva**
- Alertas cuando superas o te acercas al presupuesto
- **Budget Reports**: Informes de presupuesto programados enviados por correo electrónico

### AWS Cost & Usage Reports (CUR)
- El informe de costos y uso **más detallado** disponible
- Datos por hora, día o mes; desglosados por servicio, recurso, etiquetas
- Se exporta a S3 en formato CSV
- Se puede analizar con Athena, Redshift, QuickSight

### Cost Allocation Tags
- Etiquetas específicas para el seguimiento de costos
- **AWS-generated tags**: Creadas automáticamente por AWS (p. ej., aws:createdBy)
- **User-defined tags**: Creadas por ti (p. ej., Department, Project)
- Deben ser **activadas** en la consola de facturación para aparecer en los informes

### Billing Alarms
- Alarmas de CloudWatch basadas en los cargos estimados
- Se configuran en la región **us-east-1**
- Diferencia vs. Budgets: las Billing Alarms son básicas, los Budgets son más avanzados

### AWS Cost Explorer
- Herramienta visual para **analizar y comprender** tu gasto de AWS a lo largo del tiempo
- Filtra por servicio, cuenta, región, etiqueta, etc.
- Previsión de costos (12 meses)
- Recomendaciones de Savings Plans y Reserved Instances
- Gratuito

### APIs de precios programáticas
- **Price List API**: Obtiene los precios actuales de los servicios de AWS
- **Savings Plans Purchase Recommendation API**: Recomendaciones de Savings Plans
- Útil para integrar datos de precios en tus herramientas internas
- JSON o HTML

### AWS Savings Plans
- Descuentos por compromiso de gasto ($/hora) por 1 o 3 años
- **Compute Savings Plans**: El más flexible, aplica a EC2, Lambda, Fargate
- **EC2 Instance Savings Plans**: Específico para la familia de EC2 en una región
- **SageMaker Savings Plans**: Para el uso de SageMaker
- Se gestionan desde **AWS Cost Explorer > Savings Plans**

### AWS Service Quotas
- Ve y gestiona tus cuotas de servicio a escala a medida que crecen tus cargas de trabajo de AWS.
- Gestiona tus cuotas de servicio de AWS desde una ubicación central

## 28. Defensa en profundidad (Defence in Depth)

### Etapas
1. **Datos (Data)**: Cifrado y protección de la información sensible.
2. **Aplicación (Application)**: Asegurar que el software sea seguro y esté libre de vulnerabilidades.
3. **Cómputo (Compute)**: Proteger las máquinas virtuales y gestionar los puertos de acceso.
4. **Red (Network)**: Segmentación de recursos y control de la comunicación.
5. **Perímetro (Perimeter)**: Defensa contra amenazas externas como los ataques DDoS.
6. **Identidad (Identity)**: Gestión de accesos y control de cambios en la infraestructura.
7. **Físico (Physical)**: Restringir el acceso físico al hardware y a los centros de datos.

### Triada CIA (Confidencialidad, Integridad, Disponibilidad)
La **triada CIA** es un modelo fundamental de los principios de seguridad que describe la relación y las compensaciones entre tres conceptos centrales.
#### Confidencialidad
* **Definición:** Proteger los datos de espectadores no autorizados.
* **En la práctica:** Usar claves criptográficas para el cifrado e implementar "cifrado de sobre" (envelope encryption) (cifrar claves con otras claves).
#### Integridad
* **Definición:** Garantizar la exactitud y la integridad de los datos a lo largo de todo su ciclo de vida.
* **En la práctica:** Usar bases de datos con cumplimiento ACID para las transacciones y emplear Módulos de Seguridad de Hardware (HSM) que sean a prueba de manipulaciones (tamper-evident o tamper-proof).
#### Disponibilidad
* **Definición:** Garantizar que la información sea accesible siempre que se necesite.
* **En la práctica:** Implementar sistemas de alta disponibilidad (HA), mitigar ataques DDoS y garantizar el acceso adecuado para el descifrado.
#### Historia y evolución
* **Origen:** Mencionada por primera vez en una **publicación de NIST en 1977**.
* **Esfuerzos de modernización:**
  * **1998:** Ampliada a los "Seis Elementos Atómicos de la Información" (Confidencialidad, Posesión, Integridad, Autenticidad, Disponibilidad y Utilidad).
  * **2004:** Los NIST Engineering Principles for IT Security introdujeron 33 principios de seguridad.

## Vulnerabilidades
Un agujero o debilidad en la aplicación, que puede ser un fallo de diseño o un error de implementación, que permite a un atacante causar daño.

#### Ejemplos
- Buffer Overflow (desbordamiento de búfer)
- Validación de datos inadecuada
- Violación del mínimo privilegio
- Fuga de memoria (memory leak)
- Usar un algoritmo criptográfico roto o riesgoso

### Cifrado (Encryption)
#### ¿Qué es la criptografía?
La criptografía es la práctica y el estudio de técnicas usadas para garantizar la **comunicación segura** incluso en presencia de adversarios externos.
#### ¿Qué es el cifrado?
El cifrado es el proceso específico de codificar (revolver) la información para almacenar datos sensibles en un formato ininteligible como protección.
* **Mecanismo**: Usa una **clave (key)** y un **cifrador (cypher)** (algoritmo).
* **Entrada**: Texto plano (datos legibles).
* **Salida**: Texto cifrado (ciphertext) (datos ilegibles/protegidos).

## Claves criptográficas
- **Clave criptográfica**: Una variable usada con un algoritmo para cifrar o descifrar datos.
- **Cifrado simétrico**: Usa la **misma clave** para cifrar y descifrar. *Ejemplo:* AES
- **Cifrado asimétrico**: Usa **dos claves diferentes** (una para codificar, otra para decodificar). - *Ejemplo:* RSA

## Hashing y Salting
- **Hashing**: Una función **unidireccional** y **determinista** que convierte cualquier entrada en una cadena de tamaño fijo.
  - *Propósito*: Almacenar contraseñas de forma segura (solo se guarda el hash, no el texto plano).
  - *Funciones comunes*: MD5, SHA256, Bcrypt.
- **Salting**: Añadir una **cadena aleatoria** (salt) a la contraseña antes del hashing.
  - *Propósito*: Rompe la naturaleza determinista del hashing para prevenir ataques de diccionario y de tablas arcoíris (rainbow table).

## Cifrado en tránsito vs. en reposo
- **Cifrado en tránsito (In-Transit)**: Protege los datos mientras se **mueven** entre ubicaciones.
  - *Protocolos*: **TLS** (v1.2/1.3 son las mejores prácticas actuales) y **SSL** (obsoleto).
- **Cifrado en reposo (At-Rest)**: Protege los datos mientras están **almacenados** en un disco o en una base de datos.
  - *Algoritmos*: **AES**, **RSA**.

## AWS Artifact
- Es un portal de autoservicio para acceso bajo demanda a los informes de cumplimiento de AWS
- Obtén certificaciones ISO, informes SOC, informes PCI y acuerdos de procesamiento de datos del GDPR

## AWS Inspector
- Ejecuta un benchmark de seguridad contra instancias EC2 específicas.
- Puede realizarse tanto a nivel de red (Network) como de host
- Ejecutado por CIS, tiene 699 comprobaciones

## AWS Shield
- Es un servicio administrado de protección contra DDoS
- **Shield Standard (gratuito)**: protección contra los ataques DDoS más comunes
- **Shield Advanced (3000 USD/año)**: protección adicional contra ataques más grandes y sofisticados

## Amazon GuardDuty
- Es un servicio de detección de amenazas que monitorea continuamente en busca de actividad maliciosa y sospechosa.
- Analiza: CloudTrail, VPC Flow, logs de DNS

## AWS Web Application Firewall (WAF)
- Protege tus aplicaciones web de exploits web comunes
- Escribe tus propias reglas para ALLOW o DENY.
- Cubre el OWASP Top 10

## Conoce tus siglas (Initialisms)
| Sigla    | Significado                    |
| :------- | :----------------------------- |
| **IAM**  | Identity and Access Management |
| **S3**   | Simple Storage Service         |
| **SWF**  | Simple Workflow Service        |
| **SNS**  | Simple Notification Service    |
| **SQS**  | Simple Queue Service           |
| **SES**  | Simple Email Service           |
| **SSM**  | Simple Systems Manager         |
| **RDS**  | Relational Database Service    |
| **VPC**  | Virtual Private Cloud          |
| **VPN**  | Virtual Private Network        |
| **CFN**  | CloudFormation                 |
| **WAF**  | Web Application Firewall       |
| **MQ**   | Amazon ActiveMQ                |
| **ASG**  | Auto Scaling Groups            |
| **TAM**  | Technical Account Manager      |
| **ELB**  | Elastic Load Balancer          |
| **ALB**  | Application Load Balancer      |
| **NLB**  | Network Load Balancer          |
| **GWLB** | Gateway Load Balancer          |
| **CLB**  | Classic Load Balancer          |
| **EC2**  | Elastic Cloud Compute          |
| **ECS**  | Elastic Container Service      |
| **ECR**  | Elastic Container Repository   |
| **EBS**  | Elastic Block Storage          |
| **EFS**  | Elastic File Storage           |
| **EMR**  | Elastic MapReduce              |
| **EB**   | Elastic Beanstalk              |
| **ES**   | Elasticsearch                  |
| **EKS**  | Elastic Kubernetes Service     |
| **MSK**  | Managed Kafka Service          |
| **RAM**  | AWS Resource Manager           |
| **ACM**  | Amazon Certificate Manager     |
| **PoLP** | Principle of Least Privilege   |
| **IoT**  | Internet of Things             |
| **RI**   | Reserved Instances             |

---

## Resumen del examen

### Consejos para aprobar el CLF-C02
1. Concéntrate en los **4 dominios del examen** (Conceptos de la nube 24 %, Seguridad 30 %, Tecnología 34 %, Facturación 12 %)
2. Comprende bien el **Modelo de Responsabilidad Compartida** — aparece en MUCHAS preguntas
3. Conoce las diferencias entre **Security Groups y NACLs**
4. Conoce los **modelos de precios de EC2** (On-Demand, Reserved, Spot, Savings Plans)
5. Comprende los **6 pilares del Well-Architected Framework**
6. Conoce las **6+1 ventajas de la computación en la nube**
7. Diferencia entre servicios similares (p. ej., CloudTrail vs. CloudWatch, SQS vs. SNS)
8. Comprende Región vs. AZ vs. Edge Location
9. Conoce los **planes de soporte** y qué incluye cada uno
10. Practica con exámenes simulados antes del examen real

### Servicios clave que deberías conocer
| Categoría | Servicios |
|----------|----------|
| Cómputo | EC2, Lambda, ECS, Fargate, Lightsail, Elastic Beanstalk |
| Almacenamiento | S3, EBS, EFS, Glacier, Snow Family |
| Base de datos | RDS, Aurora, DynamoDB, Redshift, ElastiCache |
| Redes | VPC, CloudFront, Route 53, Direct Connect, API Gateway |
| Seguridad | IAM, KMS, WAF, Shield, GuardDuty, Inspector, Macie |
| Gestión | CloudWatch, CloudTrail, Config, Trusted Advisor, Organizations |
| Costo | Cost Explorer, Budgets, Pricing Calculator, Savings Plans |

---

> **Nota:** Estos apuntes cubren los temas principales del curso de Andrew Brown para el examen CLF-C02. Se recomienda complementarlos con la documentación oficial de AWS y exámenes de práctica.
