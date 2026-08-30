# L4D2 Autoexec — Movimiento, Red y Glows Neón

Config para Left 4 Dead 2 con:

- Script de movimiento nulo (evita frenazos al soltar una tecla con la opuesta presionada).
- Ajustes de red/lerp pensados para conexión estable.
- Pack de glows de colores neón: vida de supervivientes, parpadeos de estado crítico/incapacitado/agarrado, y objetos cercanos/lejanos con ciclo multicolor.
- Mejoras de calidad de vida (cambio de arma rápido, sin auto-cambio de arma, HUD con net_graph).
- Bloque **opcional** de rendimiento para laptops o PCs con GPU integrada.

## Créditos

Config base original por **EITO-TV**. Modificada y ampliada por **[waos-png](https://github.com/waos-png)**.

## Instalación

1. Copia `autoexec.cfg` a la carpeta `left4dead2/cfg/` de tu instalación (Steam → clic derecho en L4D2 → Administrar → Explorar archivos locales → `left4dead2/cfg/`).
2. El juego lo carga automáticamente al iniciar. Para cargarlo manualmente en cualquier momento, abre la consola (por defecto en este config: `F8`) y escribe `exec autoexec.cfg`.
3. **Opcional:** si usas una laptop o GPU integrada (Intel Iris Xe, UHD, etc.), copia también `autoexec_rendimiento_gpu_integrada.cfg` a la misma carpeta y ejecútalo con `exec autoexec_rendimiento_gpu_integrada.cfg`. Si tienes GPU dedicada, sáltate este paso.

## ¿Esto es baneable / detectado por VAC?

No. Todas las convars de glow (`cl_glow_*`) son configuraciones de cliente sin protección de `sv_cheats`, pensadas originalmente para el modo daltónico del juego. No afectan al servidor ni requieren `sv_cheats 1`.

## Nota sobre los valores de red

`rate`, `cl_cmdrate` y `cl_updaterate` están en su máximo (100000 / 100 / 100), pensados para conexión estable. Si tu conexión es inestable o el servidor tiene límites más bajos, el juego los recorta automáticamente — no rompe nada, pero si notas problemas, puedes bajarlos manualmente.

## Licencia

MIT — libre para usar, modificar y redistribuir. Ver [`LICENSE`](./LICENSE).
