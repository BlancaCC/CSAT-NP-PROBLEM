# Problema CSAT  

Un circuito lógico es un grafo con entradas binarias, puertas AND, OR y NOT y una salida binaria. El probema CSAT es dado un circuito lógico, determinar si existe una entrada que hace que la salida sea verdad.   

Queremos probar que CSAT es NP-completo.     




## Pasos de la demostración   

1. Prabar que CSAT está en NP.  
2. Cualquier otro lenguaje NP se reduce a él.  

### CSAT está en NP.  

Un problema pertenece a NP si pertece a la clase de complejidad polinóminca no dterminista en tiempo.  

Para ver esto consideremos seleccionaremos de manera no determinista una sucesión de valores de verdad (que serán las entradas del problema), y bastará con comprobar si para este problema la salida es verdadera.  

(Irene revisa esta explicación)  

Este algoritmo es polinímico en tiempo, ya que acotando muy burdamente:   
- Para una entrada de tamaño $x$.  
- Suponiendo que cuente con $n$ nodos nuestro grafo que represente a nuestro circuito lógico.  
- Y que una cota superior de tiempo para evaluar la salida en un nodo de una entrada de tamaño $x$ sea K.  

Entonces el tiempo de ejeción estará mayorado por $xnk$

### Reducción del problema 3-SAT a CSAT  

Necesitamos ver que cualquier otro problema NP-completo se puede reducir a CSAT, 
lo que haremos será probar que 3-SAT se puede reducir a CSAT y
puesto que la reducción es transitiva esto nos garantizará que cualquier otro 
problema NP-completo se pueda reducir a él.  


#### Descripción del problema 3-SAT    

(Me tengo que infomar mejor de cómo va este problema)  
Dado un conjunto de símboloso proposicionales $U={p_1, ..., p_{n-1}}$ y una colección de $C$ de claúsusas sobre estos símbolos. El problema consiste en determinar si son consistentes dicas claúsulas.   



## Fuentes   

(Esto habría que redactarlo según los cánones de referencias)  

- Diapositivas de teoría 
- https://en.wikipedia.org/wiki/Boolean_satisfiability_problem#3-satisfiability  
- https://en.wikipedia.org/wiki/Circuit_satisfiability_problem#Proof_of_NP-Completeness  



