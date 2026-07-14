# Prompt para resolver examen final Backend Spring Boot

Quiero que resuelvas un examen final de backend para el curso Desarrollo de Aplicaciones Open Source.

Debes trabajar como un estudiante preparado que entiende el proyecto backend Learning Center Platform visto en clase, pero sin sobredisenar la solucion. El codigo debe verse natural, ordenado y coherente con un examen universitario. No quiero codigo innecesariamente complejo, ni patrones que no aparezcan en el proyecto de referencia, ni tecnologia que no se haya trabajado en clase.

Debes seguir el estilo del backend Learning Center Platform en Java/Spring Boot revisado en clase, adaptandolo al alcance del examen final. A diferencia de una practica calificada simple, un examen final puede requerir varios bounded contexts, mas de un aggregate root, un endpoint POST, un endpoint GET, seeding inicial con `ApplicationReadyEvent`, ACL, integration events y event handlers.

## Datos que completare

```text
Ruta donde se debe crear el proyecto del examen: /Users/alumnos/IdeaProjects/

Ruta del proyecto Learning Center Platform de referencia: /Users/alumnos/downloads/learning-center-platform-v2610-master/docs/backend-spring-opensource.md

Mi nombre completo: Josep Eliu Melgarejo Quiroz

Mi codigo de estudiante: u202315165

Mi NRC: 11990

Password en caso de necesitar usar sudo : d3v3l0p3rUPC

```

## Enunciado del examen

```text

```

## Objetivo

Debes resolver el examen final backend creando un proyecto Spring Boot desde cero en la ruta indicada, usando el nombre exacto indicado y cumpliendo estrictamente el enunciado.

La solucion debe seguir el estilo del proyecto Learning Center Platform, pero de forma controlada y adecuada para un examen final. Normalmente estos examenes pueden requerir:

- Dos o tres bounded contexts.
- Dos o tres aggregate roots.
- Value objects.
- Enums.
- Embedded types.
- Records para valores inmutables.
- Reglas de negocio.
- Persistencia JPA con MySQL.
- Datos iniciales poblados automaticamente al iniciar la aplicacion.
- Un endpoint POST para registrar el aggregate principal.
- Un endpoint GET para listar otro aggregate.
- Anti-Corruption Layer entre bounded contexts.
- Integration event.
- Event handler.
- Resource y Assembler.
- Command services.
- Query services si el GET lo requiere.
- Repository.
- Physical naming strategy.
- Auditing.
- Exception handling.
- OpenAPI/Swagger.
- JavaDoc.
- README.

La unica referencia de arquitectura, patrones, estructura y estilo sera el proyecto Learning Center Platform indicado en los datos. No uses practicas pasadas, ejemplos externos ni proyectos distintos como referencia.

Usa el proyecto Learning Center Platform solo como referencia de arquitectura, estructura, nomenclatura y estilo. No copies entidades, bounded contexts, reglas de negocio, endpoints ni textos que pertenezcan al dominio Learning Center.

No modifiques el proyecto Learning Center Platform de referencia. Solo debes leerlo para analizar estructura y patrones. Todos los cambios deben hacerse unicamente dentro de la ruta indicada para el nuevo proyecto del examen.

## Extraccion de datos del enunciado

Si un dato como nombre del proyecto, root package, version de Java, version de Spring Boot, base de datos, nombre del esquema, puerto, endpoints o nombre del zip aparece en el enunciado, debes extraerlo del enunciado.

Solo pregunta si un dato no aparece y no puede inferirse con seguridad.

Debes detectar explicitamente:

- Nombre exacto del proyecto.
- Root package requerido.
- Version de Java.
- Version de Spring Boot.
- Base de datos.
- Nombre del esquema/base de datos.
- Puerto requerido.
- Endpoints requeridos.
- Operaciones permitidas por endpoint.
- Bounded contexts.
- Aggregate roots.
- Value objects.
- Enums.
- Embedded types.
- Records requeridos.
- Integration events.
- Event handlers.
- ACL requerido.
- Datos iniciales para seeding.
- Nombre final del archivo zip.
- Elementos fuera de alcance.

## Restricciones estrictas

Usa solo tecnologias trabajadas en clase o exigidas por el enunciado:

- Java en la version indicada.
- Spring Boot en la version indicada.
- Spring Web.
- Spring Data JPA.
- Jakarta Validation si corresponde.
- Maven.
- MySQL o la base de datos indicada por el enunciado.
- Lombok solo si el enunciado lo permite o si ayuda con constructores/getters/setters.
- SpringDoc OpenAPI / Swagger UI.
- JavaDoc.
- Spring application events para integration events y event handlers.
- `ApplicationReadyEvent` para seeding inicial si el enunciado lo pide.

No uses:

- Spring Security, salvo que el enunciado lo pida explicitamente.
- JWT.
- CORS, si el enunciado lo excluye.
- Testing, si el enunciado lo excluye.
- Docker, salvo que el enunciado lo pida.
- Flyway.
- Liquibase.
- MapStruct.
- WebFlux.
- Kafka.
- RabbitMQ.
- Microservicios.
- Arquitectura hexagonal completa si no aparece en el proyecto de referencia.
- Endpoints extra no pedidos.
- CRUD completo si el enunciado solo pide POST y GET.
- Funcionalidades que no aparezcan en el enunciado.

Si el enunciado dice que algo no forma parte del alcance, no lo implementes.

## Estilo obligatorio del codigo

El codigo debe:

- Estar en ingles.
- Usar nombres claros y simples.
- Seguir convenciones de Java:
  - Upper-Camel-Case para clases, records y enums.
  - Lower-Camel-Case para atributos y metodos.
  - Packages en minusculas.
- Usar packages coherentes con el root package requerido.
- Usar rutas REST en minusculas y con terminos compuestos separados por guion medio.
- Usar nombres de tablas en plural y snake_case.
- Evitar comentarios obvios.
- Usar JavaDoc solo en clases y metodos relevantes.
- Incluir mi nombre completo como `@author` cuando el enunciado lo pida.
- Mantener una estructura academica, no excesivamente empresarial.

El codigo no debe parecer generado por IA. Para lograrlo:

- No agregues clases innecesarias.
- No agregues abstracciones que no se usen.
- No inventes validaciones fuera del enunciado.
- No agregues endpoints de prueba.
- No agregues endpoints CRUD completos si solo piden POST y GET.
- No agregues datos semilla que no aparezcan en el enunciado.
- No agregues helpers genericos que no aporten.
- No escribas README demasiado publicitario.
- No uses mensajes exageradamente largos.

## Flujo obligatorio por pasos

No debes crear todo el proyecto de golpe.

Debes trabajar por pasos y detenerte al final de cada paso para pedirme confirmacion antes de continuar. No pases al siguiente paso sin mi aprobacion explicita.

Al final de cada paso, responde con:

```text
Paso X completado.
Resumen:
- ...

Confirmas que continue con el Paso Y?
```

Solo cuando yo confirme, continuas.

No uses tiempos exactos ni digas que haras algo en determinada cantidad de minutos. El avance sera controlado por pasos.

## Paso 1: Analisis del enunciado y del proyecto de referencia

En este paso no debes crear ni modificar archivos.

Debes analizar:

- El enunciado completo.
- La ruta donde se creara el proyecto.
- El nombre exacto del proyecto.
- El root package requerido.
- La version de Java.
- La version de Spring Boot.
- La base de datos requerida.
- El nombre del esquema/base de datos.
- El puerto requerido.
- Los bounded contexts.
- Que conceptos pertenecen a cada bounded context.
- Los conceptos que pertenecen a shared.
- Los aggregate roots.
- Los atributos de cada aggregate root.
- Los value objects.
- Los enums.
- Los embedded types.
- Los records requeridos.
- Las reglas de negocio.
- Los datos iniciales que deben poblarse.
- Los endpoints exactos.
- Los metodos HTTP requeridos.
- Los path variables.
- Los request bodies.
- Los responses esperados.
- Los atributos que no deben aparecer en responses.
- Los errores esperados.
- El ACL requerido.
- El integration event requerido.
- El event handler requerido.
- Las actualizaciones o creaciones entre bounded contexts.
- Los requisitos de JavaDoc.
- Los requisitos de Swagger/OpenAPI.
- Los requisitos de README.
- El nombre del zip.
- Lo que explicitamente no forma parte del alcance.

Tambien debes revisar el proyecto Learning Center Platform de referencia para identificar:

- Estructura de carpetas.
- Shared kernel.
- Auditing.
- Physical naming strategy.
- Resources.
- Assemblers.
- Controllers.
- Command services.
- Query services.
- Repositories.
- Exception handling.
- Configuracion de JPA.
- Application events o event handlers si existen.
- ACL si existe.
- Estilo de JavaDoc.

Resultado del Paso 1:

- Resumen del caso.
- Tabla o lista con los elementos extraidos del enunciado.
- Lista de bounded contexts y responsabilidades.
- Lista de clases que se van a crear.
- Lista de paquetes principales.
- Flujo esperado del POST.
- Flujo esperado del GET.
- Flujo esperado del seeding.
- Flujo esperado del integration event.
- Alcance exacto de lo que se implementara.
- Cosas que explicitamente no se implementaran.

Luego pide confirmacion para el Paso 2.

## Paso 2: Creacion del proyecto base y configuracion inicial

Solo despues de mi confirmacion, crea el proyecto Spring Boot en la ruta indicada.

Debes crear el proyecto con:

- Nombre exacto indicado.
- Root package exacto indicado.
- Maven.
- Java indicado.
- Spring Boot indicado.
- Dependencias minimas necesarias:
  - Spring Web.
  - Spring Data JPA.
  - Driver de MySQL o de la base de datos indicada.
  - Validation si corresponde.
  - Lombok si corresponde.
  - SpringDoc OpenAPI.

Debes configurar:

- `application.properties` o `application.yml`, segun el estilo del proyecto de referencia.
- Puerto.
- Datasource.
- Nombre de esquema/base de datos.
- JPA.
- Physical naming strategy.
- Nombre de la aplicacion.
- Swagger/OpenAPI basico.

No implementes todavia el dominio completo.

Resultado del Paso 2:

- Proyecto creado.
- Dependencias configuradas.
- Configuracion base lista.
- Comando para ejecutar la aplicacion.
- Confirmacion de estructura inicial.

Luego pide confirmacion para el Paso 3.

## Paso 3: Shared kernel

Solo despues de mi confirmacion, implementa el bounded context `shared`.

Debe incluir solo lo necesario para el examen:

- Clase base auditable para entidades JPA.
- Configuracion de auditoria si corresponde.
- Physical naming strategy para snake_case y tablas en plural.
- Recurso de error simple.
- Exception handler global.
- Assembler simple para errores si corresponde.
- Configuracion basica de OpenAPI si corresponde.
- Value objects compartidos si el enunciado indica que pertenecen a shared.
- Integration event record si el enunciado indica que el evento debe declararse en shared.

No implementes todavia los aggregate roots principales.

Resultado del Paso 3:

- Archivos creados en shared.
- Explicacion breve de su proposito.
- Confirmacion de que no se agrego tecnologia fuera de alcance.

Luego pide confirmacion para el Paso 4.

## Paso 4: Domain de los bounded contexts

Solo despues de mi confirmacion, implementa la capa domain de cada bounded context requerido.

Para cada bounded context debes incluir lo necesario:

- Aggregate root.
- Value objects del bounded context.
- Enums.
- Embedded types.
- Records para valores inmutables si corresponde.
- Commands para operaciones de escritura.
- Queries para operaciones de lectura si el GET lo requiere.
- Repository interface.
- Domain services solo si son necesarios.

Las reglas de negocio deben estar preferentemente en:

- Constructores de value objects.
- Constructores o metodos factory del aggregate root.
- Metodos del aggregate root.
- Command service si dependen de consultas al repositorio.
- ACL o application service cuando una regla requiere consultar otro bounded context.

No implementes todavia controllers REST.

Resultado del Paso 4:

- Domain model completo por bounded context.
- Reglas implementadas en dominio.
- Lista de validaciones cubiertas.
- Relacion conceptual entre bounded contexts.

Luego pide confirmacion para el Paso 5.

## Paso 5: Infrastructure persistence y seeding

Solo despues de mi confirmacion, implementa la capa infrastructure de persistencia.

Debe incluir:

- JPA entity o aggregate persistente segun el estilo del proyecto de referencia.
- Embeddables si corresponden.
- Attribute converters si corresponden.
- Spring Data JPA repository por aggregate.
- Repository adapter que implementa el repository interface del domain si el proyecto de referencia separa domain y persistence.
- Persistence assembler si separas domain model y persistence entity.
- Consultas necesarias para reglas de negocio.
- Consultas necesarias para GET.
- Seeding automatico de datos iniciales si el enunciado lo pide.

Para seeding:

- Usa `ApplicationReadyEvent` si el enunciado lo pide.
- Carga solo los registros indicados por el enunciado.
- Evita duplicar datos si la aplicacion se inicia varias veces.
- No agregues datos inventados.

Resultado del Paso 5:

- Persistencia lista.
- Tablas esperadas.
- Campos mapeados.
- Datos iniciales configurados.
- Reglas de unicidad o consultas de negocio listas.

Luego pide confirmacion para el Paso 6.

## Paso 6: Application layer, ACL y event handling

Solo despues de mi confirmacion, implementa la capa application.

Debe incluir, segun el enunciado:

- Command service interface.
- Command service implementation.
- Query service interface.
- Query service implementation.
- Validaciones que requieren repositorio.
- ACL entre bounded contexts.
- Facade o service interno para exponer capacidades de un bounded context a otro.
- Integration event.
- Event publisher usando application events de Spring si corresponde.
- Event handler usando `@EventListener` o el mecanismo trabajado en clase.
- Retorno de resultado o manejo claro de errores.

El command service del POST debe:

- Validar duplicados.
- Validar reglas de negocio que involucren datos existentes.
- Consultar otro bounded context mediante ACL si corresponde.
- Crear el aggregate root.
- Guardar mediante repository.
- Publicar el integration event si corresponde.
- Retornar el aggregate creado o su id.

El event handler debe:

- Recibir el integration event.
- Ubicarse en el bounded context que necesita reaccionar al evento.
- Consultar el aggregate afectado.
- Actualizar o crear solo lo indicado por el enunciado.
- Guardar cambios mediante repository.

No implementes endpoints extra.

Resultado del Paso 6:

- Caso de uso POST implementado.
- Caso de uso GET preparado si corresponde.
- ACL implementado.
- Integration event implementado.
- Event handler implementado.
- Reglas de negocio de aplicacion cubiertas.
- Errores principales considerados.

Luego pide confirmacion para el Paso 7.

## Paso 7: Interfaces REST

Solo despues de mi confirmacion, implementa la capa interfaces/rest.

Debe incluir:

- Request resource para POST.
- Response resources para POST y GET.
- Command-from-resource assembler.
- Resource-from-entity assembler.
- REST controllers.
- Swagger/OpenAPI annotations en ingles.

Los controllers deben:

- Usar los endpoints exactos del enunciado.
- Usar los metodos HTTP exactos.
- Tomar path variables si corresponde.
- No pedir en el body campos que el enunciado dice que no se deben ingresar.
- Recibir enums como string si el enunciado lo pide.
- Recibir fechas como string con el formato indicado si el enunciado lo pide.
- Retornar HTTP 201 en caso de POST exitoso.
- Retornar HTTP 200 en caso de GET exitoso.
- Retornar errores con status correcto y body simple.
- No incluir atributos de auditoria en response si el enunciado lo prohibe.
- Usar URL en minusculas y kebab-case.

Resultado del Paso 7:

- Endpoints implementados.
- Request esperado para POST.
- Response esperado para POST.
- Response esperado para GET.
- Ejemplo de request JSON.
- Ejemplo de response JSON.

Luego pide confirmacion para el Paso 8.

## Paso 8: JavaDoc, README y limpieza academica

Solo despues de mi confirmacion, revisa y completa:

- JavaDoc en ingles.
- `@author` con mi nombre completo.
- README.md en ingles.
- Descripcion de la aplicacion.
- Tecnologias usadas.
- Arquitectura breve.
- Bounded contexts implementados.
- Como configurar base de datos.
- Como ejecutar.
- Seeding si corresponde.
- Integration event si corresponde.
- Endpoints implementados.
- Ejemplo de request.
- Ejemplo de response.

No agregues marketing exagerado.

Resultado del Paso 8:

- README actualizado.
- JavaDoc revisado.
- Proyecto mantiene estilo de estudiante preparado.

Luego pide confirmacion para el Paso 9.

## Paso 9: Verificacion

Solo despues de mi confirmacion, ejecuta verificaciones.

Debes intentar:

```bash
mvn clean compile
```

Si existe base de datos configurada y es posible:

```bash
mvn spring-boot:run
```

No crees tests porque normalmente no forman parte del alcance.

Verifica:

- Compilacion.
- Paquetes correctos.
- Puerto correcto.
- Endpoints correctos.
- No hay tecnologias prohibidas.
- No hay endpoints extra innecesarios.
- No hay security ni CORS si no se pidieron.
- No hay testing si fue excluido.
- El POST retorna 201 en caso exitoso.
- El GET retorna 200 con los datos esperados.
- El seeding carga los registros requeridos.
- El event handler actualiza o crea el aggregate indicado.
- No hay datos sensibles en responses.
- No aparecen atributos de auditoria en responses si el enunciado lo prohibe.
- README existe.
- JavaDoc existe.
- Swagger/OpenAPI esta configurado.

Resultado del Paso 9:

- Estado de compilacion.
- Problemas encontrados.
- Ajustes realizados si fueron necesarios.
- Pendientes reales si algo no se pudo verificar.

Luego pide confirmacion para el Paso 10.

## Paso 10: Preparacion para entrega

Solo despues de mi confirmacion, prepara la entrega.

Debes:

- Eliminar carpetas innecesarias si corresponde.
- No eliminar codigo fuente.
- No eliminar archivos necesarios de Maven.
- No incluir `target` si el zip final no debe llevar compilados.
- Crear el `.zip` con el nombre exacto requerido.

Resultado del Paso 10:

- Ruta del zip generado.
- Nombre final del zip.
- Resumen final breve.

## Reglas de implementacion

Durante todos los pasos:

- No avances sin confirmacion.
- No hagas pasos mezclados.
- No crees archivos de pasos futuros.
- No implementes endpoints no solicitados.
- No uses tecnologias fuera de clase.
- No sobredisenes.
- No hagas que el codigo parezca generado por IA.
- Mantiene nombres en ingles.
- Mantiene paquetes y clases ordenados.
- Usa JavaDoc en ingles.
- Usa mensajes de error claros.
- Usa Swagger/OpenAPI en ingles.
- Sigue el estilo del proyecto Learning Center Platform.
- Usa como unica referencia el proyecto Learning Center Platform indicado.
- No copies dominio del proyecto Learning Center Platform.
- No modifiques el proyecto Learning Center Platform.

Puedes modificar archivos creados en pasos anteriores solo cuando sea necesario para integrar el paso actual, por ejemplo registrar servicios, corregir configuracion, ajustar mappings o completar recursos. No rehagas archivos completos ni agregues elementos de pasos futuros.

## Estructura sugerida para un examen final

Adapta los nombres al caso real del enunciado.

```text
src/main/java/<root-package>/
  shared/
    domain/
      model/
        events/
      repositories/
    infrastructure/
      persistence/jpa/configuration/strategy/
      persistence/jpa/entities/
    interfaces/rest/
      resources/
      transform/

  <primary-bounded-context>/
    domain/
      model/
        aggregates/
        commands/
        queries/
        valueobjects/
      repositories/
      services/
    application/
      commandservices/
      queryservices/
      internal/
        commandservices/
        queryservices/
      acl/
    infrastructure/
      persistence/jpa/
        entities/
        repositories/
        adapters/
        assemblers/
    interfaces/
      rest/
        resources/
        transform/

  <secondary-bounded-context>/
    domain/
      model/
        aggregates/
        commands/
        queries/
        valueobjects/
      repositories/
      services/
    application/
      commandservices/
      queryservices/
      internal/
        commandservices/
        queryservices/
        eventhandlers/
      acl/
    infrastructure/
      persistence/jpa/
        entities/
        repositories/
        adapters/
        assemblers/
    interfaces/
      acl/
      rest/
        resources/
        transform/
```

## Recordatorio final

El objetivo no es construir un backend empresarial enorme. El objetivo es resolver correctamente un examen final siguiendo el estilo visto en clase:

- Java.
- Spring Boot.
- Spring Web.
- Spring Data JPA.
- MySQL.
- DDD academico.
- Bounded contexts.
- Layered architecture.
- Aggregate roots.
- Value objects.
- Enums.
- Embedded types.
- Records cuando corresponda.
- Reglas de negocio.
- Persistencia JPA.
- Physical naming strategy.
- Resource y Assembler.
- CQRS simple.
- POST endpoint.
- GET endpoint.
- Seeding con ApplicationReadyEvent si corresponde.
- ACL.
- Integration event.
- Event handler.
- Manejo de excepciones.
- Swagger.
- JavaDoc.
- README.
- Zip final.
