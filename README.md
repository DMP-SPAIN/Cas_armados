# Reforger CAS

Proyecto local para mantener y publicar materiales CAS de Arma Reforger.

## Fuentes Vigentes

- `MANUAL_CAS_ARMADOS.html`: manual del alumno.
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

## Fuente CAS rotary

- Video de referencia: `Rotary CAS engagement example` (`VRnjkj377EE`, Dave S, 2018-10-05).
- Video de referencia 9-line: `Fixed Wing CAS Example` (`05Ed_ENSp8k`, Dave S, 2018-10-05).
- Transcripcion automatica extraida: `data/youtube/VRnjkj377EE.transcript.en.txt`.
- Transcripcion automatica 9-line: `data/youtube/05Ed_ENSp8k.transcript.en.txt`.
- Uso doctrinal en el material: reporte de entrada completo, SITREP/informe de tierra, HA/BP, CCA 5-line, colacion correcta, avance, visual/BLANCO A LA VISTA, DENTRO CALIENTE del piloto, confirmacion de LINCE, RIFLE/Zuni, BDA y RTB.

## Estructura Operativa

```text
docs/                  Contexto y procedimientos del proyecto.
forum/phpbb/           Instrucciones para publicar en foro.
web/                   Copias HTML locales listas para abrir/enlazar.
exports/github-pages/  Copias auxiliares para Pages.
exports/misiones/      Guias de mision/sesion.
.publish/Cas_armados/  Repo Git real de GitHub Pages.
```

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
