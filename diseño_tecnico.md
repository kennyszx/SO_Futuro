# Diseño Técnico de EcoLearn OS

## 1. Nombre y propósito  
EcoLearn OS está pensado para facilitar la educación sostenible y remota en centros educativos con recursos limitados. Su objetivo es maximizar el rendimiento y la seguridad en un entorno colaborativo.

## 2. Tipo de núcleo  
Microkernel  
Justificación: Modularidad que mejora la estabilidad. Los servicios del sistema se ejecutan en espacio de usuario, reduciendo el riesgo de fallos críticos.

## 3. Gestión de procesos  
- Planificación por prioridad con envejecimiento para evitar inanición.  
- Estados: listo, ejecución, bloqueado, suspendido.  
- Soporte multiproceso y multihilo para tareas concurrentes.

## 4. Gestión de memoria  
- Paginación con asignación dinámica para eficiencia y adaptación a dispositivos de bajo recurso.  
- Segmentación para separación segura de procesos.

## 5. Sistema de archivos  
- Estructura jerárquica en árbol con carpetas para asignaturas, usuarios y proyectos.  
- Control granular de permisos (lectura, escritura, ejecución) según roles.  
- Integración con almacenamiento en nube local (edu-cloud).

## 6. Mecanismos de seguridad  
- Autenticación multifactor (contraseña + biometría facial).  
- Control de acceso basado en roles para usuarios.  
- Cifrado AES en almacenamiento y comunicaciones.

## 7. Interfaz de usuario  
- GUI limpia e intuitiva, adaptada para dispositivos táctiles y PCs.  
- Soporte para comandos de voz para mayor accesibilidad.

## 8. Comparación con sistemas reales

| Característica           | EcoLearn OS          | Linux                  | Windows               |
|-------------------------|----------------------|------------------------|-----------------------|
| Núcleo                  | Microkernel          | Monolítico             | Híbrido               |
| Enfoque principal       | Educación sostenible | General                | General               |
| Gestión de memoria      | Paginación + segmentación | Paginación           | Paginación + segmentación |
| Seguridad               | MFA + encriptación   | Depende de la distribución | Autenticación básica  |
| Interfaz                | GUI + voz            | CLI y GUI              | GUI                   |
| Almacenamiento en nube  | Local (edu-cloud)    | Opcional               | Opcional              |

## 9. Reflexión final  
Diseñar EcoLearn OS me permitió integrar conocimientos teóricos con necesidades reales, entendiendo la importancia de adaptar sistemas operativos a contextos específicos enfocando en seguridad, accesibilidad y eficiencia.

