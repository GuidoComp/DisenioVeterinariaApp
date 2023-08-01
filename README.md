# DisenioVeterinariaApp
Diagrama UML de clases (40 clases) y de secuencia con implementación de patrones de diseño (Proxy, Strategy, Memento, State, Observer, Singleton, Composite y Factory)

Una afamada clínica veterinaria de la Ciudad de Buenos Aires “Cuidamos tu mascota” nos solicita el desarrollo de una aplicación para poder hacer la gestión de las mascotas (Perros, Gatos y Conejos) que quedan internadas en su institución. Al ingresar a la clínica se verifica si la mascota cuenta o no con ficha medida. Si no posee, debe crease una y asignarla. En la misma se incluirá todo el historial clinico. El
dueño de la mascota podrá pedir en cualquier momento el historial clínico. Las mascotas son examinadas por un doctor (del cual se sabe nombre, apellido, dni, email y número de celular, y una especialidad que se corresponde al tipo de animal que manejan), el cual realiza una observación de cada una, identificando su nombre, peso, si tiene o no una vacuna y su estado, que puede ser Feliz, Enfermo, Hambriento o Sediento.

Dependiendo de cómo esté cada mascota, ella responderá de manera distinta ante las acciones que puede realizar el doctor (Dar de comer, Dar de tomar, Dar Medicina), de la siguiente manera:

    ● Si nuestra mascota está hambrienta y le doy de comer, se pone feliz. De la misma
    manera si está sediento y le doy de tomar o si está enfermo y le doy medicina.
    ● Si le doy de comer y está feliz, de tanta comida se va a poner enfermo.
    ● Si las acciones que hago son distintas a las enunciadas arriba, el comportamiento no
    es importante, puede hacer un ruido, hacer que vomite, etc, pero el estado va seguir
    siendo el mismo.

La aplicación a desarrollar le permitirá a los dueños (se sabe de ellos nombre, apellido, dni, email y número de celular) enterarse del estado de todas sus mascotas en tiempo real. Por ejemplo si ingreso a mi mascota que se encuentra enferma, y deja de estarlo, debería recibir una notificación en mi correo electrónico. Por otro lado los Doctores pueden decidir a qué Mascotas hacerle seguimiento continuo, de tal manera que también pueden recibir estas notificaciones así no se encuentren de guardia en la clínica.

Los Doctores tienen distinto criterio a la hora de atender (Realizar una operación, Inyectar medicina, Hacer masajes) a las mascotas, que pueden variar dependiendo de los síntomas que presente. El sistema debe soportar que el doctor cambie dicha manera en que atiende las mascotas a demanda. Dichos criterios deben ser únicos y compartidos por todos los Doctores de la veterinaria.

Al momento de facturar los servicios realizados, la veterinaria deberá poder ofrecer tanto tratamientos individuales como conjuntos de tratamientos que incluyan varios procedimientos a realizar por cada Doctor (como por ejemplo, Vacunar como tratamiento individual o “Tiene un año”, el paquete que incluye todos los tratamientos a aplicarle a una mascota al cumplir un año, como vacunarlo, hacerle masajes, etc.).

A las Mascotas atendidas en la veterinaria se les coloca un collar antipulgas, que puede ser de distintas marcas (Antipulg, PulgByeBye o “YaNo Mepica”). El Doctor debe colocarles el collar que la veterinaria esté usando ese día sin que le importe de que marca es.

Se pide:
    1. Realizar el Diagrama de Clases incluyendo todas las relaciones, métodos, y
    atributos necesarios para que la solución sea integral aplicando los patrones
    de diseño que crea convenientes. Los atributos deben tener siempre definido
    su tipo. Los getters/setters pueden ser definidos solamente cuando sean
    requeridos para la solución que requiere el negocio. Se deben incluir todos los
    constructores necesarios para la solución del problema.
    Debe contener mínimo 40 clases.
    2. Realizar Diagramas de Secuencia de los flujos que consideren relevantes (como mínimo deben realizar 4 Diagramas de Secuencia).