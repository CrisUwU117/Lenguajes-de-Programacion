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

<caracter>::-'!'|'@'|'%'|'&'|'*'|'('|')'|'{'|'_'|'}'|'['|']'|':'|';'|'<'|'>'|'?'|<mayusculas>|<minusculas>
<pausa_opcional>::- <milisegundo>
<milisegundo>::-<entero>|<flotante>
<valor>::-<nombre_variable>|<cadena>|<numero>|<caracter>|<booleano>|<pausa_opcional>

<asignar>::- <nombre_variable>'='<valor>

<condicional>::-<si>|<si_sino>

<si>::-'si ('<condicion>') {' <bloque_instrucciones> '}'

<condicion>::-<nombre_variable><operador_relacional><valor>

<operador_relacional>::- '=='|'<'|'=<'|'=>'|'!='|'>'
<si_sino>::- 'si ('<condicion>') {'<bloque_instrucciones>'} sino {'<bloque_instrucciones>'}'

<iteracion>::-<mientras>|<para>

<mientras>::-'mientras ('<condicion>' ) { '<bloque_instrucciones>'}'

<para>::-'para ('<variable_entera>' ; '<condicion_numerica>' ; '<contador>'{ '<bloque_instrucciones>' }'

<variable_entera>::- 'entero '<nombre_variable>'='<numeros>

<condicion_numerica>::-<variable_entera><operador_relacional><numero>

<contador>::- <variable_entera>'+'<digitos>



<operaciones>::-<estado_reflector>|<estado_fuente>| <estado_reflector>::-<encendido>|<apagado>|<intensidad>|<tipo_reflector>| <tipo_reflector>::-<color_luz>|<cantidad_colores> <color_luz>::-'amarillo '|' rojo'|' azul'|'verde'|'naranja'|'violeta'|'blanco'|'negro'| 
<cantidad_colores>::-'1 '|' 2'|' 3'|'4 '|
<intensidad>::-<digitos>

<estado_fuente>::-<encendido>|<apagado>|<intensidad>
<encendido>::-<true>
<apagado>::-<false>

Probando



<flotante>::-<signo><digito>' . '<digito>




