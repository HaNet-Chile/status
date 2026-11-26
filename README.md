# Estado de HaNet

Página de estado de HaNet: **[status.hanet.muxp.art](https://status.hanet.muxp.art)**. La arma [Upptime](https://upptime.js.org) con GitHub Actions (revisa cada sitio cada 5 minutos), Issues (incidentes y mantenciones) y Pages (la página).

## [En vivo](https://status.hanet.muxp.art): <!--live status--> **Esperando el primer chequeo**

<!--start: status pages-->
<!--end: status pages-->

## Cómo se usa

- **Qué se revisa:** `sites` en [`.upptimerc.yml`](./.upptimerc.yml). Servidores es `getAppStatus`, el chequeo público de las funciones en Santiago.
- **Un incidente:** cuando algo no responde, Upptime abre un issue y lo cierra al volver. Si dura menos de 15 minutos lo borra. Se puede renombrar en español y comentar qué pasó: los comentarios salen en la página.
- **HaNet cerrado:** cuando el equipo cierra HaNet desde el Panel HNT (Estado de HaNet), Servidores sale "Con problemas" y la página muestra arriba el aviso con el mensaje y la hora de vuelta, leídos en vivo de `getAppStatus`.
- **Mantención programada:** un issue nuevo con la plantilla "Mantención programada" (etiqueta `maintenance`), con inicio y fin en hora de Chile. Se cierra sola al terminar. Los nombres que van en `expectedDown` o `expectedDegraded` son los `slug`: `app`, `servidores`, `cuenta`, `panel`, `docs`, `sitio`.
- **Diseño:** el tema de HaNet está en [`assets/themes/dark.css`](./assets/themes/dark.css) y reemplaza al oscuro de Upptime al publicar. El script del aviso y de los textos en español va en `js` dentro de `.upptimerc.yml`.
- **No tocar** `.github/workflows/`: Upptime los regenera desde `.upptimerc.yml`.

## Licencia

- Código: [MIT](./LICENSE) © [Anand Chowdhary](https://anandchowdhary.com)
- Datos de `./history`: [Open Database License](https://opendatacommons.org/licenses/odbl/1-0/)
