# PS5 UMTX Jailbreak — etaHEN 2.3B

Host del exploit **UMTX2** para PS5 (firmware 1.00–5.50) con **etaHEN 2.3B** como payload por defecto.

Sitio desplegado en GitHub Pages: **[https://digitalarmada1-a11y.github.io/umtx2/](https://digitalarmada1-a11y.github.io/umtx2/)**

## Uso en la PS5

1. Abre el navegador de la PS5 y entra a `https://digitalarmada1-a11y.github.io/umtx2/`
2. Pulsa **Jailbreak**
3. El exploit se ejecuta y carga automáticamente el payload **etaHEN 2.3B**

El host detecta el firmware (1.00–5.50) y usa los offsets correspondientes.

> **Nota:** el appcache está desactivado en este host (carga directa por HTTPS). No deberías ver "Downloading new cache..." en el navegador de la PS5.

## Payloads incluidos

- **etaHEN 2.3B** (`etaHEN-2.3B.bin`) — payload por defecto (auto-load)
  - SHA-256: `15159a1e4063068920b7efcee8d4ff814845014d2c574f27528841f608c75404`
  - Fuente oficial: https://github.com/etaHEN/etaHEN/releases/tag/2.3B
- ps5-kstuff, Byepervisor HEN, libhijacker game-patch, websrv, ftpsrv, klogsrv, shsrv, gdbsrv, ps5debug, elfldr y más (menú de payloads en la página)

## Créditos

Este host es un fork de **[idlesauce/umtx2](https://github.com/idlesauce/umtx2)**.

- Exploit basado en la implementación Lua de @shahrilnet y @n0llptr: https://github.com/shahrilnet/remote_lua_loader/blob/main/payloads/umtx.lua
- Setup basado en trabajos previos de @SpecterDev y @ChendoChap: https://github.com/PS5Dev/PS5-UMTX-Jailbreak/
- Usa PSFree 150b por abc
- Auto-carga el ELF loader de @john-tornblom
- Incluye el elf loader 9020 para compatibilidad con payloads antiguos (no disponible en modo webkit-only)
- Modo webkit-only para enviar payloads y limpiar appcache

### Sitio original en CloudFlare Pages: [https://umtx2.pages.dev/](https://umtx2.pages.dev/)
   - Media pkg: [https://umtx2.ps5browser.pages.dev/umtx2.pages.dev.pkg](https://umtx2.ps5browser.pages.dev/umtx2.pages.dev.pkg)

### Sitio original en GitHub Pages: [https://idlesauce.github.io/umtx2/](https://idlesauce.github.io/umtx2/)
   - Media pkg: [https://umtx2.ps5browser.pages.dev/umtx2.github.pkg](https://umtx2.ps5browser.pages.dev/umtx2.github.pkg)
