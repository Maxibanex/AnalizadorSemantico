# AnalizadorSemantico
Creación de un análizador semántico


# Tarea Semana 5

Leer Capítulo 5 del Libro Compiladores, Principios, Técnicas y exponer en clases

# Ejercicios:

1)    Crear un analizador semántico de un compilador. (Utilizar cualquier herramienta) en el Lenguaje de programación de su preferencia.

2)    Subir el código a Github y enviar el código fuente y el ejecutable del proyecto a nube.utesa


# Detecciones actuales del Analizador Semántico
- Si se declara una variable fuera de main.
- Si se declara una variable más de una vez en el mismo ambito.
- Si se le añade un tipo de dato que no le corresponde a una variable (solo funciona int, float o double).
- Si una variable no ha sido declarada.



# Código para prueba
int main() {\n
  int a = 0;\n
  int i = 0.5; // debe dar error porque es entero\n
  float p = 0.5;\n
  int d = 0;\n
  int d=0; //debe dar error porque ya fue declarada\n

  for (a = 0; a < 3; a++) {\n
    i++;\n
    d = i;\n
  }\n
  d=0.5; // debe dar error porque es entera\n
\n
}\n
