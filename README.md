# Testing

Primero realizamos una clase Math con una suma. Creamos un test para esta.

Creamos la clase Math.java y la compilamos. Necesitamos tener al menos un jar en la ruta que elijamos. La mía es: /home/alumnado/mirepo/lovillo/tercera/TPs/tp1/*:.

Para hacerlo funcionar primero:

TESTING

· Git clone:
$ git clone https://github.com/sergiolovillo/testing.git
$ cd testing

· Compilamos Math.java con la dirección de los jars y la dependencia:
$ javac -cp /home/alumnado/mirepo/lovillo/tercera/TPs/tp1/*:.  Math.java

· Compilamos el testing:
$ javac -cp /home/alumnado/mirepo/lovillo/tercera/TPs/tp1/*:.  MathTest.java

· Ejecutamos el test:
$ java -cp /home/alumnado/mirepo/lovillo/tercera/TPs/tp1/*:. org.junit.runner.JUnitCore  MathTest

· El resultado debería ser:

$ java -cp /home/alumnado/mirepo/lovillo/tercera/TPs/tp1/*:. org.junit.runner.JUnitCore  MathTest

...
FAILURES!!!
Tests run: 4,  Failures: 1

TESTING SUITE

· Hemos creado un Test Suite, Que nos permite realizar dos tipos de Test:
MathTest.class y TestPerson.class.

· Compilamos y realizamos el test:
$ javac -cp /home/alumnado/mirepo/lovillo/tercera/TPs/tp1/*:.  MathJunitTestSuite.java

$ java -cp /home/alumnado/mirepo/lovillo/tercera/TPs/tp1/*:. org.junit.runner.JUnitCore  MathJunitTestSuite
JUnit version 4.12
...
FAILURES!!!
Tests run: 5,  Failures: 1

