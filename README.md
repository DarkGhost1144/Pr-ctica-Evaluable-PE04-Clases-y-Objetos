# Practica-Evaluable-PE04-Clases-y-Objetos
1. [Calendario] Implementa una clase Calendario que representa una fecha concreta (año, mes
y día).
  + Calendario
  - día: int
  - mes: int
  - anyo: int
  + Calenario(int, int, int)
  + incrementarDía()
  + IncrementarMes()
  + incrementarAnyo(int)
  + toString():String
  + equals(Calendario): boolean
  + getDia(): int
  + getMes(): int
  + getAnyo(): int
Consideraciones:
o incremetarDía() incrementa en un día el calendario.
o incremetarMes() incrementa en un mes el calendario.
o incrementarAnyo(int) incrementa el calendario en el número de años que se le pasa
como parámetro.
o equals(Calendario) devuelve true si el calendario pasado como parámetro es igual al
que invoca al método, y false si no son iguales.
o Escribe también una clase Principal que incluya un método main en el que se creen
objetos de la clase Calendario y se prueben los métodos anteriores.

2. [Vehículo, Cliente y VehículoAlquilado] Implementa las siguientes 3 clases:
o Clase Vehiculo. Tiene los atributos matrícula, marca, modelo, tarifa y disponible.
Todos String salvo tarifa que es double y disponible boolean. Métodos: constructor,
getters y setters.
o Clase Cliente. Tiene los atributos DNI, nombre, apellidos y teléfono, todos String.
Métodos: constructor, getters, setters y al menos getNombreCompleto.
o La clase VehiculoAlquilado tiene como atributos un vehículo, un cliente, la fecha de
alquiler (que será un objeto de la clase LocalDate) y el número de días de alquiler.
Métodos: constructor, getters/setters y getImporteTotal (número de días de alquiler
por tarifa).
Escribe también una clase Principal que incluya un método main en el que se creen
objetos de las clases anteriores y se prueben sus métodos.

3. [Cuenta Corriente I] Diseña una clase CuentaCorriente que almacena los datos: DNI y nombre
del titular, así como el saldo. Las operaciones típicas con una cuenta corriente son:
o Crear una cuenta: se necesita el DNI y el nombre del titular. El saldo inicial será 0.
o Sacar dinero: el método recibe una cantidad y actualiza en consecuencia el saldo.
Además, el método devuelve un booleano (true/false) indicando si ha sido posible
realizar la operación o no:
▪ Si solicita sacar más dinero del disponible, la operación no se materializa y el
método devuelve un false.
▪ Si solicita sacar menos dinero del disponible, entonces la operación sí se
materializa (se actualiza el saldo) y el método devuelve un true.
o Ingresar dinero: se incrementa el saldo.
o Mostrar información: muestra información disponible de la cuenta corriente.
Escribe una clase Principal que incluya un método main en el que se creen objetos de la clase
CuentaCorriente y se prueben los métodos anteriores.

4. [Cuenta Corriente II] A partir de la clase anterior, sobrecarga el constructor para poder crear
objetos.
o Con el DNI del titular de la cuenta y un saldo inicial.
o Con el DNI, nombre y saldo inicial.
Escribe un programa Principal que incluya un método main en el que se creen objetos de la
clase CuentaCorriente y se prueben los métodos anteriores.

5. [Cuenta Corriente III] A partir de la clase anterior, modifica la visibilidad de atributos y
métodos para que:
o El saldo no sea visible para otras clases.
o Nombre sea público para cualquier clase.
o Para el DNI no se definirá ningún tipo de visibilidad (visibilidad por defecto).
Escribe un prgrama Principal que incluya un método main en el que se creen objetos de la
clase CuentaCorriente y se prueben los niveles de visibilidad anteriores.

6. [Cuenta Corriente IV] Todas las cuentas corrientes con las que se va a trabajar pertenecen al
mismo banco (que es único). Añadir un atributo (estático) a la clase CuentaCorriente con el nombre
de dicho banco. Diseñar dos métodos para recuperar (getter) y modificar (setter) el nombre del
banco (al que pertenecen todas las cuentas corrientes).
Escribe un programa Principal que incluya un método main en el que se creen objetos de la
clase CuentaCorriente y se prueben los métodos anteriores.

7. [Gestores] Teniendo en cuenta el último desarrollo de la clase CuentaCorriente, existen
gestores que administran cuentas bancarias y atienden a sus propietarios. Cada cuenta, en caso de
tenerlo, cuenta con un único gestor. Diseñar la clase Gestor, de la que interesa guardar su nombre,
teléfono y el importe máximo autorizado con el que pueden operar. Con respecto a los gestores,
existen las siguientes restricciones:
o Un gestor tendrá siempre un nombre y un teléfono.
o Si no se asigna, el importe máximo autorizado por operación será de 10.000 euros.
o Un gestor, una vez asignado, no podrá cambiar su número de teléfono. Y todo el
mundo podrá consultarlo.
o El nombre será público y el importe máximo tendrá visibilidad por defecto.
Modificar la clase CuentaCorriente para que pueda disponer de un atributo de tipo Gestor.
Escribir los métodos necesarios.
Escribe, igualmente, un programa Principal que incluya un método main en el que se creen
objetos de la clase Gestor y CuentaCorriente y se prueben los métodos anteriores.

8. [Hora] Escribe un programa que lea por teclado una hora cualquiera y un número n que
representa una cantidad en segundos. El programa mostrará la hora introducida y las n siguientes,
que se diferencian en 1 segundo. Para ello, hemos de diseñar previamente la clase Hora.
  + Hora
  - hora: int
  - minutos: int
  - segundos: int
  + Hora (int, int, int)
  + getHora(): int
  + getMinutos(): int
  + getSegundos(): int
  + setHora(int)
  + setMinutos(int)
  + setSegundos(int)
  + toString(): String
  + incrementarSegundo()
Consideración: el método incrementarSegundo incrementa en un segundo la Hora. Ten en
cuenta que, por ejemplo, después de 3:35:59 viene 3:36:00. O que después de 8:59:59 viene
9:00:00

Telf.: 959 14 95 23 - Correo electrónico: 21001028.edu@juntadeandalucia.es
9. [Texto] Diseña una clase Texto que gestione una cadena de caracteres con las siguientes
propiedades y operaciones:
  + Texto
  - cadena: String
  - creacion: LocalDate
  - longitudMaxima: int
  + Texto(int)
  + addFinal(char)
  + addFinal(String)
  + addPrincipio(char)
  + addPrincipio(String)
  + mostrar()
Consideraciones:
o La cadena de caracteres tendrá una longitud máxima que se especifica en el constructor.
El constructor, además, inicializa la cadena a “”, y el atributo creación a LocalDate.now(),
que es la fecha actual.
o El método addFinal permite añadir un carácter (char) o una palabra (String) al final de la
cadena.
o El método addPrincipio permite añadir un carácter (char) o una palabra (String) al inicio
de la cadena.
o El método mostrar imprime por pantalla información sobre el Texto (la cadena, la fecha
de creación y la longitud máxima que puede tener).

10. [SintonizadorFM] Definir una clase que permita controlar un sintonizador digital de emisoras
FM; concretamente, se desea dotar al controlador de una interfaz que permita subir (up) o bajar
(down) la frecuencia en saltos de 0,5 MHz, y mostrar la frecuencia sintonizada en un momento dado
(display). Supondremos que el rango de frecuencias para manejar oscila entre los 80 MHz y los 108
MHz. Al inicio, el controlador sintoniza la frecuencia indicada en el constructor, u 80 MHz por defecto
si no se le indica ninguna. Si durante una operación de subida o bajada se sobrepasa uno de los
límites, la frecuencia sintonizada debe pasar a ser la del extremo contrario. Escribir también una
clase Principal, con el método main en el que probar la clase SintonizadorFM que se ha creado.
+ SintonizadorFM
- frecuenciaActual: double
+ SintonizadorFM(double)
+ SintonizadorFM()
+ up()
+ down()
+ mostrarDisplay() : String

11. [Empresa Ferroviaria] Hemos recibido el encargo de un cliente para definir los paquetes y las
clases necesarias para gestionar una empresa ferroviaria. Sólo es necesario, para cada clase,
implementar los atributos necesarios y los métodos constructores. En la empresa se distinguen 2
grandes grupos: el personal y la maquinaria. En el primero se ubican todos los empleados de la
empresa, que se clasifican en 3 grupos: los maquinistas, los mecánicos y los jefes de estación. De
cada uno de ellos se desea guardar:
• Maquinistas: su nombre, DNI, sueldo y el rango que tienen adquirido. Éste último se modela
como una cadena de caracteres (String).
• Mecánicos: su nombre, teléfono (para contactar en caso de urgencia) y en qué especialidad
desarrollan su trabajo (frenos, hidráulica, electricidad ó motor). Éste último atributo se
modela como una cadena de caracteres (String).
• Jefes de Estación: su nombre, DNI y la fecha de fue nombrado de estación. Éste último
atributo se modela como un objeto de la clase Date (fecha).
En la parte de maquinaria podemos encontrar trenes, locomotoras y vagones. De cada uno de
ellos hay que considerar:
• Vagones: tiene un número que lo identifica, una carga máxima (en kilos), la carga actual y el
tipo de mercancía (un String).
• Locomotoras: disponen de una matrícula (que las identifica), la potencia de sus motores y
una antigüedad (año de fabricación). Además, cada locomotora tiene asignado un mecánico
que se encarga de su mantenimiento.
• Trenes: están formados por una locomotora y tres vagones. Cada tren tiene asignado un
maquinista que es responsable de él.
Todas las clases correspondientes al personal (Maquinista, Mecánico y JefeDeEstación) será de
uso público. Entre las clases relativas a la maquinaria sólo será posible construir, desde clases
externas, objetos de tipo Tren y de tipo Locomotora. La clase Vagon tendrá visibilidad por
defecto.

12. [NumeroEntero] Implementa la siguiente clase, tal y como se recoge en el UML:
  + NumeroEntero
  - valor: int
  + VALOR_MAXIMO: int <<static>>
  + VALOR_MÍNIMO: int <<static>>
  + Entero(int)
  + compareTo(Integer): int
  + getValor(): int
  + signo(): int
  + getValorDecimal(): double
  + toString(): String
Consideraciones:
• VALOR_MAXIMO es una constante (static y final) con los siguientes valores (actualiza sus
valores en el constructor):
o VALOR_MAXIMO = 999999.
o VALOR_MINIMO = -999999.
• El método compareTo devuelve:
o 1 si el objeto (el atributo valor) que llama el método es mayor que el pasado
como parámetro.
o -1 si el objeto (el atributo valor) que llama el método es menor que el pasado
como parámetro.
o 0 si el objeto (el atributo valor) que llama el método es igual que el pasado como
parámetro.
• El método signo devuelve:
o 1 si el atributo valor del objeto que llama el método es un número positivo.
o -1 si el atributo valor del objeto que llama el método es un número negativo.
o 0 si el atributo valor del objeto que llama el método es 0.
• El método getValorDecimal devuelve un número decimal con el atributo valor (entero),
pasado a decimal.
• El método toString() devuelve una cadena de texto con el atributo valor del objeto que
llama el método.

13. [Producto] Implementa la siguiente clase, tal y como se recoge en el UML:
  + Producto
  - id: int
  - nombre: String
  - precio: double
  + Producto(int, String, double)
  + getId():int
  + getNombre(): String
  + getPrecio(): double
  + setPrecio(double): void
  + aplicarDescuento(int): void
  + toString(): String
  + equals(Object) : boolean
  Consideraciones:
• toString y equals sobrescriben los métodos equivalentes que hereda de Object.
• Dos productos se consideran iguales cuando tienen mismo id y mismo nombre.

14. [SensorTemperatura] Implementa la siguiente clase, tal y como se recoge en el UML:
+ SensorTemperatura
- ubicacion: String
- temperaturaActual: double
- temperaturaMaximaMedible: double <<satic>>
+ SensorTemperatura (String,double)
+ esPeligrosa() : boolean
+ getTemperaturaMaximaMedible(): double <<static>>
+ toString():String
Consideraciones:
• Considera que la temperatura máxima medible es de 98.9 grados centígrados.
• esPeligrosa devuelve true si la temperatura actual es menor a -40.0ºC o superior 50.0ºC.

15. [Factura] Implementa la siguiente clase, tal y como se recoge en el UML:
+ Factura
- numero: int
- concepto: String
- importeSinIva: double
- IVA: int <<static>>
+ Factura(int, String, double)
+ getNumero(): int
+ getConcepto(): String
+ getImporteTotal(): double
+ setImporte(double): void
+ setConcepto(String): void
+ toString():String
Consideraciones:
• El IVA es un atributo estático que vale 21.
• getImporteTotal devuelve el importe IVA incluido.
