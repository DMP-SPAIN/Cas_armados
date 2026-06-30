# Reforger CAS

Proyecto local para mantener y publicar materiales CAS de Arma Reforger.

## Fuentes Vigentes

- `MANUAL_CAS_ARMADOS.html`: manual del alumno. Es una sola fuente con selector de lectura `PC` / `Móvil`; no dupliques el manual en otro HTML salvo petición expresa.
- `CHULETAS_CAS.html`: tablillas y herramientas de bolsillo.
- `MANUAL_INSTRUCTORES_CAS.html`: manual del instructor.
- `GUIA_DIA1_OPERACION_FORD.html`: guia visual de la primera sesion.
- `GUIA_DIA2_CHECKIN_SITREP.html`: guia del segundo ejercicio, transito de aerodromo, reporte en CP, SITREP, BP, plan de ataque, 5 lineas, DENTRO CALIENTE, RIFLE/Zuni, BDA y RTB.
- `1_MANUAL_CAS_HELICOPTEROS.md`, `2_PROGRAMA_FORMACION_INSTRUCTOR.md` y `FORMACION_CAS_KIOWA_REFORGER.md`: fuentes historicas/soporte.
- `logo_armados.png`: recurso grafico.

## URLs Publicas

- Manual alumno: `https://dmp-spain.github.io/Cas_armados/`
- Chuletas: `https://dmp-spain.github.io/Cas_armados/CHULETAS_CAS.html`
- Manual instructor: `https://dmp-spain.github.io/Cas_armados/MANUAL_INSTRUCTORES_CAS.html`
- Guia Dia 1 FORD: `https://dmp-spain.github.io/Cas_armados/guia-dia1-operacion-ford.html`
- Guia Dia 2 CP/SITREP/Zuni: `https://dmp-spain.github.io/Cas_armados/guia-dia2-checkin-sitrep.html`

## Progresion Del Curso

1. Sesion 1: transito de aerodromo, rodaje/despegue emulado y reporte de entrada en seco.
2. Sesion 2: CP, SITREP, BP, plan de ataque, 5 lineas, DENTRO CALIENTE, RIFLE/Zuni, BDA y RTB.
3. Sesion 3: consolidacion del Dia 2 con rotacion de LINCE y aparato atacante usando el orden 6/5/4/5/4/6.
4. Sesion 4: control terminal, correlacion, ABORT, reataque, correccion y BDA.
5. Sesion 5: 9-line y observaciones solo cuando la 5-line ya sale ordenada.
6. Sesion 6: integracion JTAC con maniobra terrestre y prioridades.
7. Sesion 7: plan CAS, frecuencias, CP/BP, separacion y ventanas.
8. Sesion 8: ejercicio final con evaluacion integrada.

## Fuente CAS rotary

- Video de referencia: `Rotary CAS engagement example` (`VRnjkj377EE`, Dave S, 2018-10-05).
- Video de referencia 9-line: `Fixed Wing CAS Example` (`05Ed_ENSp8k`, Dave S, 2018-10-05).
- Video de referencia para explicar por numeros: `How to Call for Close Air Support (CAS)` (`Qq-ieXBkziE`, HipPocket0341, 2024-11-24).
- Transcripcion automatica extraida: `data/youtube/VRnjkj377EE.transcript.en.txt`.
- Transcripcion automatica 9-line: `data/youtube/05Ed_ENSp8k.transcript.en.txt`.
- Transcripcion automatica de estructura numerica: `data/youtube/Qq-ieXBkziE.en.json3`.
- Uso doctrinal en el material: reporte de entrada completo, SITREP/informe de tierra, HA/BP, CCA 5-line, colacion correcta, avance, visual/BLANCO A LA VISTA, DENTRO CALIENTE del piloto, confirmacion de LINCE, RIFLE/Zuni, BDA y RTB.
- Regla editorial vigente: el manual del alumno debe leerse como un flujo humano: llegar, entender, ordenar, confirmar, entrar y cerrar. Usa listas numeradas solo dentro de transmisiones reales, por ejemplo reporte de entrada de 6 datos, SITREP completo de 10 datos, 5-Line, 9-Line, control terminal o BDA. No meter tablas abstractas tipo `3-6-10` en el manual base. La visualización móvil se resuelve con el selector integrado del propio manual.

## Estructura Operativa

```text
docs/                  Contexto y procedimientos del proyecto.
forum/phpbb/           Instrucciones para publicar en foro.
web/                   Copias HTML locales listas para abrir/enlazar.
exports/github-pages/  Copias auxiliares para Pages.
exports/misiones/      Guias de mision/sesion.
.publish/Cas_armados/  Repo Git real de GitHub Pages.
```

## Arranque Para IA

- Leer primero `docs/ARRANQUE_IA.md`.
- Usar `docs/AGENTS_COMPLETO.md` solo si hace falta el detalle completo.
- No tocar `.publish/Cas_armados/data/evaluacion-cas.json` salvo peticion explicita.

## Sincronizacion

- Manual alumno: `MANUAL_CAS_ARMADOS.html` -> `web/index.html`, `web/manual-cas-armados.html`, `exports/github-pages/index.html`, `.publish/Cas_armados/index.html`.
- Chuletas: `CHULETAS_CAS.html` -> `web/CHULETAS_CAS.html`, `exports/github-pages/CHULETAS_CAS.html`, `.publish/Cas_armados/CHULETAS_CAS.html`.
- Manual instructor: `MANUAL_INSTRUCTORES_CAS.html` -> `exports/github-pages/MANUAL_INSTRUCTORES_CAS.html`, `.publish/Cas_armados/MANUAL_INSTRUCTORES_CAS.html`.
- Guia Dia 1: `GUIA_DIA1_OPERACION_FORD.html` -> `web/guia-dia1-operacion-ford.html`, `exports/misiones/guia-dia1-operacion-ford.html`, `.publish/Cas_armados/guia-dia1-operacion-ford.html`.
- Guia Dia 2: `GUIA_DIA2_CHECKIN_SITREP.html` -> `web/guia-dia2-checkin-sitrep.html`, `exports/misiones/guia-dia2-checkin-sitrep.html`, `.publish/Cas_armados/guia-dia2-checkin-sitrep.html`.

## Publicacion

Publicar solo desde `.publish/Cas_armados`, empujando el mismo commit a `main` y `gh-pages`.

No usar `git push --force`.

Antes de publicar, revisar que no haya rutas locales privadas, IPs, credenciales, tokens o datos internos que no deban ser publicos.

No hay PDF ni ZIP vigentes en la estructura limpia actual.
