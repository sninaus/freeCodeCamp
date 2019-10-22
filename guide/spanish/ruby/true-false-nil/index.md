---
title: True, False, and Nil
localeTitle: Verdadero, falso y nulo
---
# Verdadero, falso y nulo

`true` , `false` y `nil` son tipos de datos incorporados especiales en Ruby. Cada una de estas palabras clave se evalúa como un objeto que es la única instancia de su clase respectiva.

```ruby
true.class 
 => TrueClass 
 false.class 
 => FalseClass 
 nil.class 
 => NilClass 
 ``` 
 
 `true` y `false` son los valores booleanos nativos de Ruby. Un booleano puede tener solo dos valores: true (verdadero) o false (falso).
Se puede asignar el valor `true` o `false` a una variable, pasarla a métodos, y generalmente se le puede dar un como a cualquier otro objeto nativo de Ruby (Strings, Arrays, Hashes).
 
 `nil` es un valor especial que indica la ausencia de valor: es la manera de Ruby de referirse a "nada". Un ejemplo de cuando se puede encontrar el objeto `nil` es cuando se pregunta por algo que no existe o no puede ser encontrado:
```

sombreros = ["boina", "sombrero", "gorro", "fez", "flatcap"]

sombreros[0] => "boina" # el sombrero en el índice 0 sombreros[2] => "gorro" # el sombrero en el índice 2 sombreros[4] => "flatcap" # el sombrero en el índice 4 sombreros[5] => nil # no hay sombrero en el índice 5, el índice 5 no tiene nada (nulo)
```
Zero no es nada (es un número, que no es nada). Asi también, strings vacíos, arrays vacíos y hashes vacíos no son nada (son objetos, pero que están vacíos). Se puede usar el método `nil?` para chequear si un objeto es nil. 
```

 0.nil? => falso "".nil? => falso [].nil? => falso {}.nil? => falso nil.nil? => verdadero # del ejemplo de arriba gorras[5].nil? => verdadero`

Cada objeto en Ruby tiene un valor booleano, lo que significa que se considera verdadero o falso en un contexto booleano. Aquellos considerados verdaderos en este contexto son "truthy" y aquellos considerados falsos son "falsey". En Ruby, _solo_ `false` y `nil` son "falsey", todo lo demás es "truthy".

### Otros recursos

*   https://ruby-doc.org/core-2.3.0/TrueClass.html
*   https://ruby-doc.org/core-2.3.0/FalseClass.html
*   https://ruby-doc.org/core-2.3.0/NilClass.html
*   https://en.wikipedia.org/wiki/Boolean
