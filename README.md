# Lenguajes-de-Programacion 1800  BNF

<programa>::-<bloque_instrucciones>

<bloque_instrucciones>::-<instruccion>|<bloque_instrucciones>

<instruccion>::-<operaciones>|<secuencia>|<declarar_variable>|<asignar>|<condicional>|<iteracion>|<leer>|<bloque_instrucciones>

<secuencia>::-<bloque_instrucciones>
  
  <declarar_variable>::- <nombre_variable>' as '<tipo_dato>'='<valor>| <nombre_variable>' as '<tipo_dato>

<nombre_variable>::- <cadena>

<cadena>::- <letras>|<letras><numeros>
<letras>::- <mayusculas>|<minusculas>  

<mayusculas>::- ' A'| 'B '| 'C '| ' D'| ' E'| ' F'| 'G '| ' H'| 'I '| ' J' |' K'| 'L '| 'M '| ' N'| Ñ' '|' O'| ' P'| ' Q'| ' R'| ' S'| 'T '| 'U '| 'V '| 'W '| ' X'| 'Y
'| ' Z'

<minusculas>::- ' a'| 'b '| 'c '| ' d'| ' e'| ' f'| 'g '| ' h'| 'i '| ' j' |' k'| 'l '| 'm '| ' n'| ñ' '|' o'| ' p'| ' q'| ' r'| ' s'|'t'|'u'|'v'|'w'|'x'|'y'|'z'

<numeros>::- <signo><digitos>
<signo>::- '-'|'+'

<digitos>::- '0'|<numero_validos>

<numero_validos>::-'1 '|' 2'|' 3'|'4 '|' 5'|' 6'|' 7'|' 8'|' 9'

<tipo_dato>::-<caracter>|<cadena>|<entero>|<decimales>|<booleano>

<entero>::-<numeros>

<booleano>::-<true>|<false>

<flotante>::-<signo><digito>' . '<digito>




