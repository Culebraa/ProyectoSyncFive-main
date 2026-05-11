Falta por hacer en el proyecto de SyncFive:

1. Arreglar los fallos esporádicos de la foto de perfil, a veces carga a veces no (DIEGO).
2. Coherencia en estilos en todas la páginas (DIEGO).
3. Filtros funcionando en todas las páginas (GERMÁN).
4. Integración en subpáginas. Hay páginas que dependen directamente de otras. Para hacer más usable el menú lateral integrarlas conjuntamente (JAVIER).
   a. Meter un botón para acceder a Tipos de Emergencias dentro de Partes de Intervención.
   b. Meter un botón para acceder a Motivos de Permisos dentro de Permisos.
   c. Meter un botón para acceder a Categorías Material dentro de Materiales.
   d. Meter un botón para acceder a los Cargos dentro de Usuarios.
   e. Controlar quien puede ver y quien tiene acceso a esas páginas desde los roles.
5. Paginación (DIEGO).
6. Mejor control de errores en temas como las claves foráneas, que lanzan mensajes técnicos que el usuario promedio no va a ser capaz de entender. (JAVIER)

Página de emergencias activas (JAVIER):
7. Añadir mapas en las emergencias activas, este mapa debe permitirte iniciar una ruta hasta la emergencia.

Página partes de intervención (JAVIER):
8. La responsividad sigue rompiendo en algunos puntos.
9. En la página de partes de intervención te debería cargar el ID Bombero automáticamente con la sesión iniciada.
   Lo mismo con las fechas y las fechas horas de la salida, llegada y regreso.
10. En el desplegable para añadir personas como mínimo te tendría que salir nombre y apellidos.
   ¿Qué pasa si hay dos personas con el mismo nombre?
11. Los vehículos asignados no se guardan correctamente, lo que rompe la inserción.
12. La actualización tampoco funciona.

Páginas de avisos (DIEGO):
13. No va nada.



Página de Alineación (JAVIER):
21. Ocurre algo raro al intentar guardar alineaciones con personas sin ningún cargo asignado. Revisarlo.

Página de Guardias (GERMÁN):
22. En el ver más información debería aparecer también el id de la guardia.
23. La modificación no funciona.
24. En la creación se crean dos registros con una sola acción del usuario.
25. No deja asignar correctamente personas a las guardias.
26. Me vas a matar Culebra <3 pero si nos da tiempo cambiaremos el formato actual (fecha, hora inicio, hora fin) por (fecha/hinicio - fecha/hfin)
27. Se queda corta en responsividad, habría que reducirla un campo más. Eso lo conseguiremos con el punto 5.

Página de Turnos de Refuerzo (GERMÁN):
28. El filtro de horas se comporta un poco extraño.
29. El detalle del Turno de Refuerzo no funciona.
30. El turno de refuerzo no tiene edición ni eliminación. Quizás por temas de permisos mal aplicados no me aparecen con mi rol superior.
31. El formulario solo te deja introducir fecha inicio, fecha fin y número de horas totales. Sin embargo los campos son TIMESTAMP por lo que te tendría que dejar introducir fecha/hinicio - fecha/hfin, siendo las horas un campo calculado que se calculara automáticamente con la diferencia de las dos.
32. La inserción no funciona si el turno de refuerzo empieza y acaba en el mismo día.
33. Se queda corta en responsividad, habría que reducirla un campo más. Eso lo conseguiremos quitando la suma de horas y dejando solo la fecha/hinicio - fecha/hfin

Página Cuadrante Anual (GERMÁN):
34. Hay algunas características de los PopUps que te muestran información que no me acaban de cuadrar, esto esta pendiente de una validación más a fondo para entender lo que pasa.
35. Revisar el estilo de la leyenda. Esta demasiada pegada a las migas de pan y sale un fondo que no se apreciaba en los monitores de clase.
36. Rompe demasiado pronto en responsividad pero no se me ocurre una solución para esta.

Página Cuadrante Mensual (JAVIER/GERMÁN):
37. Habría que revisar el tema de los permisos en esta página. Ver quien podrá ver que cosa.

Páginas Infraestructuras de Agua "Mapas" (DAVID) :
<----------------- FIN------------->
14. Cambiar el título a algo más descriptivo. Infraestructuras de Agua no involucra a los vehículos que también aparecen en el mapa.
15. Añadir un icono a la cuarta tarjeta en la que aparecen los "Activos", poner un nombre más descriptivo.
16. Los filtros solo filtran las infraestructuras de agua, deben filtrar también los vehículos.
17. ¿Quizás estaría bien que los municipios fueran un desplegable?¿O quedaría demasiado largo? Al ser un campo de texto puedes escribir mal en nombre y dar la falsa sensación de que ese municipio no existe. Si no otra opción es un campo de texto que te vaya dando sugerencias de los registros que se parecen a los que estás escribiendo.
18. Falta añadir a los filtros el Tipo "Vehículo".
20. La eliminación se debe hacer un modal de bootstrap como en el resto de página, no con un alert javascript.



38. No funciona nada. Arreglado por Diego
39. En el ojo de ver más estaría bien poner el ID.

43. No deja ver más detalles. 
44. No deja editar.
45. No deja eliminar. 
<-------------------- Por hacer ---------------------->

19. Da error a la hora de editar las infraestructuras de agua. El municipio con ese código tan extraño puede causar confusión. Añadir algo como en el punto 4.

Página de Formaciones (DAVID):
40. Hay que mejorar el trato a las claves foráneas aquí, no se tratan de la mejor manera posible pues no puede ser que porque haya un bombero asignado a una formación ya no te puedas apuntar a ella.

41. Lo mismo que en otros casos, recordatorio global. Hay que mejorar mucho la forma de tratar los errores y más aún cuando entran de por medio excepciones por foráneas o claves primarias.

Página de Ediciones (DAVID):
42. En el formulario de inserción a la relación. El campo del ID de los Bomberos igual sería más comodo si fuera desplegable. Yo creo que lo mejor aquí sería copiar el formulario de inserción de destinatarios que se usa en la página de avisos.


Página de Personas/Trabajadores/Usuarios (DAVID):
77. En el filtro en vez de localidad añadiría parque, además las localidades son cargadas con las provincias, no con las localidades por lo que el filtro pierde toda su utilidad.
78. En la página de los detalles de la persona debe aparecer el id de bombero y el número de funcionario. En este punto la localidada también aparece como provincia, no como localidad, esto es un error. Deberían aparecer las dos, tanto la localidad como la provincia. Revisar el resto de datos que podrían faltar o estar erróneos.
79. No funciona la inserción por la validación del número de funcionario. "A priori"
80. Faltaría probar la eliminación cuando funcione la inserción.
81. Responsividad HORRIBLE.

Página de Carnets (DIEGO):
46. Añadir el id en el ojo de ver más.
47. Estaría bien que la fecha de vencimiento en el formulario de inserción se pusiera automáticamente relativamente a la fecha de optención obtenida, hay que tener en cuenta que se guarda la duración en meses para ese tipo de carnet.
48. Categorías de los carnets en desplegable porfa.
49. Rompe responsividad, hay que revisarlo.

Página de Permisos (DIEGO):
50. No va nada.

Página de Motivos Permiso (DIEGO):
52. No va la inserción.
53. Hay que revisar los estilos de los botones.

Página de Vehículos (JAVIER):
54. Problemas con la validación de la matrícula en la inserción. Revisar el resto de las validaciones en la inserción una vez funcione la matrícula.
55. Hay que revisar migas de pan.

Página de Salidas (JAVIER):
56. Añadir el número de registro en el modal de ver. Además interesaría ordenador los campos mejor, están mal ordenados respecto a la tabla de manera que causan un confusión.
57. Los ids de los bomberos tanto en la edición como en la inserción sería interesante que fueran un desplegable.
58. Si te salta error porque una matrícula no existe te da error de formato de matrícula, lo cual no es descriptivo.
59. Hay que hacerla más responsive, habría que quitar como mínimo un campo más para la pantalla de los teléfonos.

Página de Materiales (GERMÁN):
60. En la edición de materiales si intentas borrar una relación te salta con un alert de javascript, tendría que ser con un modal de bootstrap.
61. Si tienes unidades 1 y un número de serie te da error, como el unidades 1 te sale por defecto tienes que borrarlo, lo cuál es molesto. Esto ocurre en los vehículos y en los almacenes.

Página de Mantenimientos (DIEGO):
62. Rompe la responsividad entre los 992px y los 1075px
63. Puedes guardar un mantenimiento como realizado sin antes haber asignado la fecha fin
64. Los campos descripción en la inserción sería mejor que fueran de estos que les puedes editar el alto tu como usuario (textarea).
65. No creo que tenga sentido que puedas abrir un mantenimiento con estado realizado, bajo mi punto de vista en la creación siempre será abierto hasta que por edición pase a ser cerrado.

Página de Incidencias (JAVIER):
66. El ID de la incidencia en la tabla aparece como undefined
67. La responsividad rompe demasiado pronto, habría que quitar como mínimo un campo más.
68. Ver más, edición y eliminación no funcionan.
69. Tendría que validar que solo se puede crear una incidencia sobre un material o sobre un vehículo pero no sobre dos a la vez.
70. Hay algun problema con la validación de matrícula en la inserción.

Página de Categorías de los Materiales (GERMÁN):
71. La responsividad parte demasiado pronto, hay que revisar las columnas de la tabla.

Página de Almacenes (GERMÁN):
72. No funciona la edición.
73. No funciona la inserción.
74. Por algún motivo no saca todos los almacenes que hay en la base de datos.
75. No es todo lo responsive que debería, habría que quitarle como mínimo un campo más.

Página de Instalaciones (DIEGO):
76. Hay que añadir el id de la instalación tanto a la tabla como al modal de ver datos completos. No puede ser que en ningún punto puedas ver el id de la instalación.


Página de Roles/Cargos (DIEGO):
82. Hay que eliminar el filtro.
83. Asegurar coherencia de estilos con el resto de páginas.
84. Acabar de probar todo una vez este más coherente, pero en principio funciona.

Sumas totales por persona (+-):
Diego: 19
David: 20
Javier: 20
Germán: 24