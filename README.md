# POO-C-
Fundamentos de la programación orientada a objetos 

#Pilares de la  programacion orientada a objetos

Polimorfismo:
el polimorfismo es la capacidad que tiene un lenguaje orientado a objetos de 
llamar a un metodo anulado en funcion de que clase lo este llamando

//conversion implicita
int integerVariable;
long longVariable;

integerVariable = 123;
longVariable = integerVariable;


//converison explicita 
int integerVariable;
char charVariable;

integerVariable = 9;
charVariable = (char)integerVariable;

Sobre carga de metodos
Revisar sobrecarga de metodos mediante la utilizacion de metodos sobrecargados:
la sobrecagra de metodos se basa en que los metodos sobrecargados tienen los mismos nombres pero
diferentes listas de parametros. Revisar pagina 164 del libro

Constructores
Un constructor inicializa las variables a utilizar o metodos en una clase puede haber mas de 
un constructor y este puede recibir parametros distientos al igual que un constructor no puede ser vacio.

indexadores
Los indexadores son una comodidad sint�ctica que le permiten crear una clase, 
un struct o una interfaz a los que pueden acceder las aplicaciones cliente simplemente como una matriz

GET/SET
Son descriptores de acceso que permiten. El descriptor de acceso get permite devolver el valor de la propiedad 
mientras que el descriptor de acceso set permite establecer un valor a la propiedad

Interfaces
Una interfaz en C# es un conjunto de firmas de metodos. propiedades y eventos o 
indexadores agrupados con un nombre comun. Las interfaces funcionan  como
de funcionalidades definidas que pueden implementarse  en una clase o estructura
de C#.

Una interfaz es como una clase base abstracta cualquier clase o estructura que implemente una interfaz debe de implementar todos
sus miembros, una interfaz no puede ser instanciada directamente, sus miembros son implementados por cualquier clase
o estructura que implementa la interfaz
Las interfaces pueden contener eventos, indexadores, metodos y propiedades.
Las interfaces no contienen implementacion de metodos
Una clase o estructura puede implementar multiples intefaces. Una clase puede heredar una clase base y tambien implementar una o mas interfaces.


Objetos
Los objetos son entidades que contienen un conjunto de valores definidos(Estado del objeto) y un conjunto de operaciones que pueden ejecutarse sobre ese objeto
(los comportamientos del objeto).

Clase
una clase es una coleccion de codigo y de variables, las clases gestionan el estado en forma de las variables que contienen y comportamientos en forma de los
metodos que contienen

Tipos de datos primitivos
son los tipos de datos C# reconoce cuando se instala como por ejemplo int, long, char, string

Tipos de datos abstractos
los tipos de datos abstractos son tipos de datos que C# no admite cunado se 
instalan, antes de poder utilizar un tipo de dato abstracto hay que declararlo en 
el codigo.Los tipos de datos abstractos se definen en el codigo en lugar del 
compilador de C#.

Encapsulacion de datos
Mediante la encapsulacion de datos se encapsulan los datos de manera que se pueden
ocultar para que solo puedan se accedidos de una forma segura existen varios 
tipos de encapsulacion de datos las cuales son ambitos de clases 

Miembros Publicos
Los miembros marcados como public son visibles para las clases derivadas y para
el codigo que crea los objetos de la clase.

Miembros private
Los miembros marcados como private solo son visibles para la clase en la que se 
definen. Los miembros privados no son accesibles desde las clases derivadas ni 
desde el codigo que crea los objetos de la clase si no se le asigna nombre a
un miembro este por default pasa a ser miembro privado.

Miembros Protected
Los miembros protected solo son visibles para la clase en la que se definen o 
desde las clases derivadas de esa clase no se pueden acceder a los miembros 
protegidos desde el codigo que crea los miembros protegidos de su clase.

Miembros internal
Los miembros marcados como internal son visibles para cualquier codigo en el mismo
archivo binario. pero no son visibles para otros archivos binarios.

Miembros protected intrnal.
Los miembros marcados como protected internal son visibles para todo el codigo
incluido en el mismo archivo binario y para las clases externas que se deriven de
su clase 


Campos: 
los campos son miembros de datos de una clase son variables que pertenecen a una 
clasemediante cualquier metodo definido en la misma clase, un camo se define 
exactamente igual que cualquier variable.

Metodos:
Los metodos son bloques de codigo con nombre en una clase. los metodos proporcionan
los comportamientos de las clases, pueden ejecutarse por cualquier otro fragmento 
de codigo de la clase.

Propiedades:
Las propiedades son miembros identificados que proporcionan acceso al estado de 
un objeto suelen tener descriptores de acceso llamados get y set.

GET
Los descriptores de acceso get devuelven el valor actual del campo correspondiente.

SET
asignan un nuevo valor al campo se puede validar en el descriptor que pueda ser 
asignado un valor correcto de lo contrario se mandara un mensaje de error

Eventos
Los eventos son acciones que ocurren cuando se realiza una tarea especifica como
click sobre un boton



Indexadores
Los indexadores permiten que se acceda a una clase como si fuera una matriz.
Para especificar que se debe devolver cuando el elemento hace llamada se utilizan
corchetes para acceder al elemento de la clase se usa un fragmento de codigo 
llamado descriptor de acceso de indexador.

Operadores
Un operador permite definir el comportamiento de la clase cuando se usa en una
expresion con un operador unuario o binario. Esto sicnifica que se puede ampliar
el comportamiento de operadores predefinidos para que se ajusten a las necesidades
de las clases.

Sobrecarga de Operadores
Sobrecarga de operador que define el comportamiento de un operador cuando aparece 
en una expresion con clase o estructura.Para sobrecargar operadores uniarios mas 
o menos de negacion o complemento bit a bit en una clase o estructura hay que 
definir un metodo con un tipo devuelto deseado, el operador que se esta 
sobrecargando y un solo parametro del tipo de la clase o estructura
 que contiene  el metodo sobrecargado.

Para sobrecargar operadores de tipo true o false  en una clase o estructura hay
que definir un metodo con un tipo de devolucion  booleano y un solo parametro
del tipo de la clase o estructura que contiene el metodo de operador sobrecargado

Para sobrecargar los operadores binarios  en una clase o estructura, hay que 
definirun metodo con un tipo de devolucion booleano  y un solo parametro de tipo 
claseo estructura y dos peametros. al menos uno de los dos parametros debe de 
ser de tipo clase que contiene el metodo del operador sobrecargado.

Constructores 
Los constructores de estructura son metodos especiales que se ejecutan cuando se
crea una variable de tipo estructura. Los constructores suelen usuarse para
inicializar una estructura con un estado conocido. 

Destructores:
son lo coantrario a los contructores, los destructores se ejecutan cuando el
recolector de objetos no utilizados destruye los objetos. A diferencia de 
los contructores los destructores solo pueden escribirse una vez para la clase
los destructores se inicializan con (~), el identificador del destructor debe
corresponder al nombre de la clase.

Modificador Static
Cuando se define un campo o un metodo en una clase, cada objeto creado por el
codigo tiene su propia copia de valores de campo y metodos. Mediante la palabra
clave static. Se puede invalidar este comportamiento lo que permite que varios
objetos de la misma clase compartan valores de camo y metodos.

Espacios de Nombre
Los espacios de nombres organizan  las clases mediante un grupo designado y el
nombre del espacio de nombre puede se usado para diferenciar dos clases con el
mismo nombre. El codigo C# debe usar espacios de nombre para posteriormente 
ayudar a identificar nuestras clases mediante un grupo comun. Se pueden declarar
espacios de nombre dentro de otros espacios de nombre o declarano el espacion de
nombres seguido del principal, pueden contener: Clases, Estrucuturas, Interfaces
Enumeriaciones y Delegados.
Exixten una multitud de espacios de nombre en .NET FRAMEWORK  por mencionar
algunas y su funcionalidad son:
