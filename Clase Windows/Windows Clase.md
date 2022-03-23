# Windows Server

## Clase 1

### Active directory (AD)

Es una base de datos y un conjunto de servicios que conectan a los usuarios con los recursos de la red.

Utiliza protocolos como LDAP, DNS, DHCP Y Kerberos.

Permite a los administradores establecer políticas de nivel de empresa, despliega programas en multiples sistemas y aplica actualizaciones de seguridad a toda la organización.

#### Funcionamiento

Los usuarios pueden acceder al repositorio para una variedad de propósitos:
- Autenticación de Usuario
- Almacenamiento de datos de configuración
- Acceder a archivos a archivos e impresoras

#### Arquitectura

Active Directory es un servicio de *directorio jerárquico* basado en el dominio.

- Es posible subdividir un dominio en unidades organizativas y probarlo con objetos.
- Puede crear múltiples dominios y agruparlos en sitios, arboles y bosques.

### Active Directory Domain Services (AD DS)

AD DS es una implementación de Active Directory que utiliza un servidor de base de datos para almacenar los datos.

Un domino es un contenedor lógico de componentes de red hospedado por al menos un servidor controlado de dominio.

### Objetos y Atributos
- Un dominio de AD DS es na estructura jerárquica que toma la forma de un árbol y es muy similar a un sistema de archivos.
- Consiste en objetos, cada uno de los cuales representa un recurso lógico o físico.
- Cada objeto consta de atributos que almacenan información sobre el objeto.

Un contenedor puede tener otros objetos subordinados a el:
- Domino
- Unidad organizacional

Un objeto hoja no puede tener objetos subordinados:
- Usuarios
- Ordenadores
- Grupos
- Aplicaciones
- Recursos de red

### Dominio
Puede crear una jerarquía dentro de un dominio.

```
        bosque-----es.cl              <-----Bosque
        /    \
       /      \
      /        \
     /          \
    Árbol      Árbol----Universidad  <--IP<--Arboles
     |  \           \
     |   \           \
     |    duoc.cl     \              <-----Dominio
   inacap.cl         usach.cl
    /       \
Profesores  Alumnos                  <-----Unidad Organizacional
            /    \
           /      \
   Informáticos  Diseñadores          <-----Grupos

```

### Unidades Organizativas

Contenedores  Dentro de un dominio, utilizados para dividir la seguridad y la responsabilidad administrativa entre varias divisiones o departamentos.

Función en una capacidad subordinada a un dominio, como subdominio, pero sin la separación completa de la política de la seguridad.

### Catalogo Global

Cada bosque tiene un catalogo global, que es una lista de todos los objetos en el bosque, junto con un subconjunto de los atributos de cada objeto.

### Instalación de Active Directory

Hay muchas variables que pueden afectar el rendimiento de una instalación de AD:
 - El hardware que seleccionas para tus controladores.
 - Las capacidades de su red.
 - Los tipos de enlaces WAN que conectas a sus sitios remotos.
