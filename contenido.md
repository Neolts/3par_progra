## Portafolio 3ra Parcial
## Notas

#### *Las instrucciones tanto en erlang como en elixir siempre deben de retornar algo.
#### *Si se ponen multiples instrucciones en la misma linea, retorna el valor de la ultima instruccion.
#### *El comando "h" nos muestra todas las opciones para realizar.
    Si usas el comando "h(pid)" o "h pid" te muestra que es lo que realiza el comando pid.
#### *Al ser de tipado dinamico, ni en elixir o erlang es necesario declarar el tipo de dato, el tipo de dato se determina de acuerdo al contenido, la asignacion se le conoce como fijacion(binding).
#### *El nombre de la variable inicia con un caracter alfabetico en minuscula o _
#### *Cuando se tiene una variable booleana, se debe colocar un signo de interrogacion "?" al final de esta.
### Modulos
    Los modulos constan de varias funciones. 
    Las funciones deben de estar definidas dentro de un modulo.
    Su sintaxis es NombreModulo.nombre_funcion(args).
    Siempre debe tener su primera letra mayuscula. 

## Programacion
![image](https://user-images.githubusercontent.com/111713831/205528530-65c20b72-31c8-447b-81af-9f5e1904b967.png)
![image](https://user-images.githubusercontent.com/111713831/205529180-b94dc46d-2353-4c02-a7f2-f7c7e1c1ac45.png)
![image](https://user-images.githubusercontent.com/111713831/205529466-362959d6-6289-4d67-b9bf-4827089d603b.png)

///////////////////////////// \
defmodule HolaMundo do
  def imprimir_hola_mundo do
    IO.puts("Hola Mundo")
  end
end

//imprime: "Hola mundo" cuando llamamos el modulo HolaMundo.imprimir_hola_mundo \
///////////////////////////// 
defmodule HolaMundo do 
   def saludo(msg) do
     IO.puts(msg)
   end
end
\
HolaMundo.saludo("Este es un mensaje de prueba")
\
// Imprime: "Este es un mensaje de prueba"
///////////////////////////
\
defmodule Geometria do
   def perimetro1(l),do: cuadrado(l)
   def perimetro2(l),do: Geometria.cuadrado(l)
   def cuadrado(l), do: l*l
end
\
Geometria.cuadrado(7)
\
//Imprime "49" 
//Si la funcion fuera "defp" se hace privada y no realiza desde el shell porque es privado.
