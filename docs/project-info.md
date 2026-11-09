# Información del proyecto

## Qué es
Un juego web de memoria (parejas de cartas) en un tablero 4x4 con estética en tonos rosa pastel e iconos SVG sencillos inspirados en personajes Disney.

## Para quién
Cualquier persona que quiera echar una partida rápida desde el navegador, en una interfaz visual y sin necesidad de registrarse.

## Funciones
- Mostrar un tablero de 4x4 (16 cartas, 8 parejas distintas) boca abajo y barajadas al azar en cada partida.
- Permitir voltear 2 cartas por turno: si coinciden se quedan boca arriba; si no, se vuelven a tapar tras una breve pausa.
- Contar los intentos realizados durante la partida.
- Mostrar un mensaje de victoria al completar las 8 parejas y un botón para reiniciar la partida.

## Fuera de alcance
- Cuentas de usuario, bases de datos, clasificaciones online o modo multijugador.
- Descarga de imágenes externas, librerías de terceros o frameworks complejos.
- Efectos de sonido, animaciones 3D avanzadas o llamadas a APIs externas.

## Tecnología
Una única página web (`index.html`) en HTML, CSS y JavaScript, sin librerías externas ni servidor. Se arranca haciendo doble clic sobre `index.html` para abrirlo directamente en el navegador.

## Datos y claves
Solo usa en memoria el estado temporal de la partida (cartas, parejas acertadas e intentos), que se reinicia al recargar. No utiliza claves ni variables de `.env`.

## Cómo se prueba
Al abrir `index.html` en el navegador se ve la cuadrícula 4x4 en tonos rosa pastel con las 16 cartas boca abajo y el contador de intentos a `0`. Al destapar dos cartas distintas, suman `1` intento y vuelven a taparse; al acertar las 8 parejas, quedan todas visibles y aparece el aviso de victoria con el botón de reiniciar funcionando.
---

<details>
<summary>Ejemplo de referencia: calculadora de hipoteca (no es tu proyecto)</summary>

**Qué es:** una página que calcula la cuota mensual de una hipoteca.

**Para quién:** personas que están comparando hipotecas antes de ir al banco.

**Funciones:**
- Pedir importe, interés anual y años.
- Mostrar la cuota mensual.
- Avisar si falta un dato o no es válido.

**Fuera de alcance:** cuentas de usuario, guardar simulaciones y ofertas de bancos reales.

**Tecnología:** una página HTML con JavaScript que se abre en el navegador.

**Datos y claves:** solo los datos que escribe el usuario, que no se guardan. No necesita claves.

**Cómo se prueba:** 200.000 € al 3 % a 30 años = 843 €/mes.

</details>
