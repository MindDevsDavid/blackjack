# ♠ Blackjack multijugador local

Juego de **blackjack (21)** en un solo archivo HTML, pensado para jugar varias personas reales en el **mismo PC o móvil**, sin instalar nada y sin conexión.

## Cómo jugarlo

1. Descarga `blackjack.html` (o clona este repositorio).
2. Haz **doble clic** en el archivo → se abre en tu navegador. No necesita servidor ni internet.
3. Configura la mesa: nombre y **fichas iniciales de cada jugador** (entre 100 y 100.000; recarga con el mismo monto).
4. Juega por turnos: apostar → reparto → seguro (si aplica) → manos → crupier → liquidación.

## Reglas de la mesa

- **Blackjack natural paga 3:2.** El crupier pide hasta 16 y se planta en 17 (también soft 17).
- **Seguro** cuando el crupier muestra As: paga 2:1.
- **Doblar** con dos cartas; **dividir** pares hasta 4 manos; doblar tras dividir permitido.
- Ases divididos reciben una carta cada uno y se cierran; blackjack tras dividir paga 1:1.
- **6 mazos** con barajado automático al 25%. Apuesta mínima **10**; sin máximo: puedes ir **all-in** con «Todo».
- **1 a 6 jugadores**, todos ven la mesa y se resalta de quién es el turno.

## La banca (la casa)

La banca empieza con **10.000 fichas** y es la que paga los premios: lo que pierdes va a la banca y de ahí salen los pagos. Las fichas **nunca desaparecen ni se inventan** — el total de la mesa se conserva siempre.

- Si un jugador se queda sin fichas: **Recargar** (la banca se las vende por su monto inicial) o **Retirarse** (se lleva sus fichas y su apuesta vuelve a la banca).
- La partida se **guarda sola** en el navegador (`localStorage`); al volver a abrir puedes continuar o empezar de nuevo.

## Controles

| Tecla | Acción |
|---|---|
| `H` | Pedir carta |
| `S` | Plantarse |
| `D` | Doblar |
| `P` | Dividir |
| `Enter` | Apostar / nueva ronda |

También hay botones para todo; el sonido se silencia con 🔊 y «⚙ Mesa» reconfigura la partida.

## Tecnología

HTML + CSS + JavaScript puro en un **archivo único**, sin dependencias ni build. Compatible con navegadores modernos de escritorio y móvil.
