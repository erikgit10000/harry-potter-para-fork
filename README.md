# HARRY POTTER (SOMBRERO SELECCIONADOR)
Esta es una aplicación que te permite ser seleccionado para una de las cuatro casas de Hogwarts:
  * _Slytherin_
  * __Hufflepuff__
  * *Ravenclaw*
  * **Gryffindor**
    
## Funcionamiento de la aplicación
  1. Primero introduce tus datos personales.
  2. Si estos datos son correctos, pasarás a realizar un cuestionario. Cada pregunta otorga puntos a cada casa.
  3. Una vez completado el cuestionario serás elegido para tu casa de Hogwarts.

Por ejemplo un resultado final como el siguiente:  
| Casa       | Puntuación |
|------------|------------|
| Slytherin  | 10         |
| Ravenclaw  | 5          |
| Gryffindor | 11         |
| Hufflepuff | 3          |  

Te asignaría a Gryffindor.

## Estructura de código de las preguntas
Las preguntas del cuestionario se encuentran en un fichero JavaScript ([questions.js](https://github.com/BertoMP/harry-potter-para-fork/blob/main/js/questions.js)) que tiene un formato JSON 
en el que cada pregunta se estructura de la siguiente manera:
```
{
  question: '¿Qué color te gusta más de los siguientes?',
  answers: [
    {
      text: 'Verde',
      house: 'Slytherin',
      points: 10
    },
    {
      text: 'Rojo',
      house: 'Gryffindor',
      points: 10
    },
    {
      text: 'Azul',
      house: 'Ravenclaw',
      points: 10
    },
    {
      text: 'Amarillo',
      house: 'Hufflepuff',
      points: 10
    }
  ]
}
```
