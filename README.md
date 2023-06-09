# Guessing Name Ehanced - POST API

La empresa King.com nos ha contratado para que, en sus juegos Web de adivinar números, enviemos la puntuación del jugador.

Les gustaría recibir 3 datos:

1. El tiempo que ha el jugador ha empleado para adivinar el número
2. El número de intentos que ha necesitado
3. El nombre de la maquina des de donde se envia la puntuación (podríamos pensarlo como un nombre de usuario)

## Arquitectura

King.com nos ofrece un endpoint para enviar peticiones de tipo POST. Esta es la URL:

`https://omiras-reimagined-rotary-phone-rpgp96g5x7fx55x-3000.preview.app.github.dev/score`

Nos comentan que este es el objeto serializado en JSON que tenemos que enviar:

```
{
  "machine": "Oscar",
  "elapsed_time": 30,
  "attempts": 4
}
```

## Tu tarea

Completa adecuadamente la función **sendScoreToServer** para enviar los datos de la partida al endpoint una vez el jugador adivine el número secreto.

Piensa además, en que punto del código tienes que invocar a dicha función.

Puedes ver si has enviado bien tus datos porque la API te responderá con un mensaje de éxito. Además, puedes ver si tu record se ha insertado en esta [Web](https://03i74i.csb.app/)
