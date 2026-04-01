# Sistema de Roles y Rangos de la Plataforma Numinia

> Basado en el sistema de pensamiento sistémico del EEM Institute
> y la estructura de roles del sistema Numinia.

---

## La idea central

En Numinia distinguimos tres cosas que NO son lo mismo:

```
RANGO          Lo que PUEDES hacer (permisos)
GREMIO         Lo que SABES hacer (perfil/cualificación)
ROL            Lo que HACES ahora (función dinámica)
```

Los **Rangos** dan permisos.
Los **Gremios** describen tu conocimiento.
Los **Roles** emergen de tus acciones.

---

## 1. Rangos: La escalera de confianza

Los rangos son acumulativos. Cada nivel incluye todo lo anterior.

```
                    ╔══════════════╗
                    ║   ORACULO    ║  Co-fundador
                    ║  Pythia, sol ║  Configura el sistema
                    ╚══════╤═══════╝
                           │
                    ╔══════╧═══════╗
                    ║   ARCONTE    ║  Administrador
                    ║  Llave + ojo ║  Gestiona todo el catálogo
                    ╚══════╤═══════╝
                           │
                    ╔══════╧═══════╗
                    ║  VERNACULO   ║  Creador de confianza
                    ║  Pluma + ↑   ║  Sube assets, ve stats
                    ╚══════╤═══════╝
                           │
                    ╔══════╧═══════╗
                    ║  PEREGRINO   ║  Aventurero comprometido
                    ║  Brujula     ║  Season Pass, loot, puzzles
                    ╚══════╤═══════╝
                           │
                    ╔══════╧═══════╗
                    ║  CIUDADANO   ║  Miembro con wallet
                    ║  Escudo      ║  Favoritos, perfil, Session Zero
                    ╚══════╤═══════╝
                           │
                    ╔══════╧═══════╗
                    ║    NOMADA    ║  Visitante libre
                    ║  Viento      ║  Navega, descarga CC0
                    ╚══════════════╝
```

### Tabla de permisos

```
Accion                          NOM  CIU  PER  VER  ARC  ORA
─────────────────────────────── ───  ───  ───  ───  ───  ───
Navegar galeria                  x    x    x    x    x    x
Descargar assets CC0             x    x    x    x    x    x
Buscar y filtrar                 x    x    x    x    x    x
                                 │
Conectar wallet                  ·    x    x    x    x    x
Guardar favoritos                ·    x    x    x    x    x
Ver perfil propio                ·    x    x    x    x    x
Ver NFTs propios                 ·    x    x    x    x    x
Participar en Session Zero       ·    x    x    x    x    x
                                 │
Acceder a aventuras premium      ·    ·    x    x    x    x
Reclamar loot exclusivo          ·    ·    x    x    x    x
Participar en burn ritual        ·    ·    x    x    x    x
Ver progreso de temporada        ·    ·    x    x    x    x
                                 │
Subir assets al catalogo         ·    ·    ·    x    x    x
Editar metadatos propios         ·    ·    ·    x    x    x
Ver stats de descargas propias   ·    ·    ·    x    x    x
Acceso al LAP (panel creador)    ·    ·    ·    x    x    x
                                 │
Gestionar TODOS los assets       ·    ·    ·    ·    x    x
Toggle visibilidad               ·    ·    ·    ·    x    x
Sync a R2 / IPFS / Arweave      ·    ·    ·    ·    x    x
Gestionar temporadas             ·    ·    ·    ·    x    x
Ver stats globales               ·    ·    ·    ·    x    x
Audit logs                       ·    ·    ·    ·    x    x
                                 │
Gestionar lista de admins        ·    ·    ·    ·    ·    x
Configuracion del sistema        ·    ·    ·    ·    ·    x
Decisiones arquitectonicas       ·    ·    ·    ·    ·    x
```

### Como se determina el rango

El rango NO se asigna manualmente. Se **infiere** de lo que ya sabemos:

```
┌─────────────────────────────────────────────────────┐
│                                                     │
│   Sin sesion ──────────────────────────► NOMADA     │
│                                                     │
│   Wallet conectada ───────────────────► CIUDADANO   │
│                                                     │
│   Wallet + Season Pass ───────────────► PEREGRINO   │
│                                                     │
│   Wallet + assets subidos / creator ──► VERNACULO   │
│                                                     │
│   Wallet en ADMIN_WALLET_ADDRESSES ───► ARCONTE     │
│                                                     │
│   Wallet fundador ────────────────────► ORACULO     │
│                                                     │
└─────────────────────────────────────────────────────┘
```

---

## 2. Gremios y Facciones: Quien eres en Numinia

Los gremios describen tu **perfil de conocimiento**.
Las facciones describen tu **campo de desarrollo**.
Se asignan al completar la **Session Zero**.

```
          G R E M I O S (vertical: que sabes)
          ═══════════════════════════════════

     Alquimistas       Exegetas       Procuradores     Centinelas
     (crear)           (narrar)       (organizar)      (proteger)
        │                 │                │                │
    ┌───┴───┐         ┌───┴───┐        ┌───┴───┐       ┌───┴───┐
    │       │         │       │        │       │       │       │
 Artesanos Ingenieros Cronistas Eruditos Juristas Sindicos Serafines Arcangeles
    │   │     │   │     │   │    │   │    │   │    │   │    │   │     │    │
    P   E     A   Au    L   B    T   H    LR  He   Te  Co   Ca  Gu    Sa  Gui



          F A C C I O N E S (horizontal: que campo)
          ═════════════════════════════════════════

                    ┌───────────────────────────┐
                    │    Neo-Atlantistas        │
                    │    (Arte - itinerante)    │
                    │    acompana a todas       │
                    └─────────┬─────────────────┘
                              │
    ┌─────────────────────────┼─────────────────────────┐
    │                         │                         │
    ▼                         ▼                         ▼
 Hermeticos           Herederos de Eleusis        Circulo Estelar
 (Educacion)          ★ JUEGO (prototipo) ★       (Framework)
 periferico           siempre se empieza          periferico
                      por jugar
```

### Relacion Gremio x Faccion

No son paralelos. Son **transversales**. Se cruzan:

```
                    Herederos     Circulo      Hermeticos
                    de Eleusis    Estelar
                    (Juego)       (Framework)  (Educacion)
                    ───────────   ──────────   ──────────
 Alquimistas        Crea juegos   Construye    Ensena a
 (crear)            y mundos      sistemas     crear

 Exegetas           Escribe       Documenta    Investiga
 (narrar)           aventuras     procesos     y teoriza

 Procuradores       Gestiona      Organiza     Administra
 (organizar)        torneos       la empresa   la academia

 Centinelas         Modera        Asegura      Acompana
 (proteger)         partidas      calidad      el aprendizaje
```

---

## 3. Roles: Lo que haces AHORA

Los roles son **dinamicos**. No se asignan. **Emergen de tus acciones**.
Una misma persona puede activar distintos roles en distintos momentos.

```
  Pablo (Oraculo, Alquimista-Ingeniero, Herederos de Eleusis)
  ═══════════════════════════════════════════════════════════

  09:00  Sube un asset GLB ──────────────► Rol: ARTESANO
  09:30  Revisa stats ──────────────────► Rol: CURADOR
  10:00  Programa el frontend ──────────► Rol: INGENIERO
  11:00  Escribe lore de temporada ─────► Rol: CRONISTA
  14:00  Prioriza el backlog ───────────► Rol: GESTOR
  16:00  Piensa en monetizacion ────────► Rol: ESTRATEGA
  17:00  Responde en Discord ───────────► Rol: GUIA

  Mismo ejecutor. Mismo rango (Oraculo). Mismo gremio.
  SIETE roles distintos en un dia.
```

### Roles tipicos de la plataforma

```
  ╭──────────────────────────────────────────────────────────╮
  │  ACCION EN LA PLATAFORMA          ROL QUE SE ACTIVA      │
  ├──────────────────────────────────────────────────────────┤
  │                                                          │
  │  Navega y descarga assets    ───►  Explorador             │
  │  Guarda favoritos            ───►  Coleccionista          │
  │  Juega una aventura          ───►  Aventurero             │
  │  Sube un asset               ───►  Artesano               │
  │  Remixa un asset CC0         ───►  Remixer                │
  │  Verifica ownership NFT      ───►  Guardian               │
  │  Construye un mundo .hyp     ───►  Arquitecto             │
  │  Gestiona el catalogo        ───►  Curador                │
  │  Administra la plataforma    ───►  Arconte (rol + rango)  │
  │                                                          │
  ╰──────────────────────────────────────────────────────────╯
```

---

## 4. Como encaja todo junto

```
  ┌─────────────────────────────────────────────────────────────┐
  │                                                             │
  │   EJECUTOR (persona fisica / wallet)                        │
  │   Ejemplo: Pablo, 0x1234...                                 │
  │                                                             │
  │   ┌───────────────────────────────────────────────────────┐ │
  │   │ RANGO: Oraculo                                        │ │
  │   │ Que puede hacer: TODO                                 │ │
  │   │ (permisos acumulativos)                               │ │
  │   └───────────────────────────────────────────────────────┘ │
  │                                                             │
  │   ┌───────────────────────────────────────────────────────┐ │
  │   │ PERFIL (Gremio + Faccion)                             │ │
  │   │ Gremio: Alquimista > Ingeniero > Arquitecto           │ │
  │   │ Faccion: Herederos de Eleusis (Juego)                 │ │
  │   │ Que sabe hacer: disenar sistemas, programar, crear    │ │
  │   └───────────────────────────────────────────────────────┘ │
  │                                                             │
  │   ┌───────────────────────────────────────────────────────┐ │
  │   │ ROLES ACTIVOS (cambian segun la accion)               │ │
  │   │ Ahora mismo: Ingeniero (programando el frontend)      │ │
  │   │ Hace 1 hora: Curador (revisando assets)               │ │
  │   │ Que esta haciendo: funcion concreta en este momento   │ │
  │   └───────────────────────────────────────────────────────┘ │
  │                                                             │
  └─────────────────────────────────────────────────────────────┘
```

---

## 5. Resumen en una frase

> **El Rango dice que PUEDES hacer.**
> **El Gremio dice que SABES hacer.**
> **La Faccion dice DONDE lo haces.**
> **El Rol dice que ESTAS HACIENDO.**

Los cuatro son necesarios. Ninguno sustituye al otro.

```
  RANGO ─── permisos de la plataforma (estatico, acumulativo)
    │
  GREMIO ── perfil de conocimiento (asignado en Session Zero)
    │
  FACCION ─ campo de desarrollo (asignado en Session Zero)
    │
  ROL ───── funcion activa (dinamico, emerge de la accion)
```

---

## 6. Flujo del usuario en la plataforma

```
  Llega a numinia.store
         │
         ▼
  ┌──────────────┐     Navega, descarga
  │   NOMADA     │────────────────────────► usa la plataforma libre
  └──────┬───────┘
         │ conecta wallet
         ▼
  ┌──────────────┐     Favoritos, perfil
  │  CIUDADANO   │────────────────────────► Session Zero disponible
  └──────┬───────┘
         │ completa Session Zero
         │ (elige gremio + faccion)
         ▼
  ┌──────────────┐     Gremio asignado
  │  CIUDADANO   │     Faccion elegida
  │  + perfil    │     Prism Cells ganadas
  └──────┬───────┘
         │ compra Season Pass
         ▼
  ┌──────────────┐     Aventuras premium
  │  PEREGRINO   │────────────────────────► puzzles, loot, burn ritual
  └──────┬───────┘
         │ sube assets / es invitado
         ▼
  ┌──────────────┐     Panel de creador
  │  VERNACULO   │────────────────────────► upload, stats, LAP
  └──────┬───────┘
         │ wallet en whitelist
         ▼
  ┌──────────────┐     Gestion total
  │   ARCONTE    │────────────────────────► admin del catalogo
  └──────┬───────┘
         │ co-fundador
         ▼
  ┌──────────────┐     Configuracion
  │   ORACULO    │────────────────────────► decisiones de sistema
  └──────────────┘
```

---

*Documento basado en el framework STSI del EEM Institute,
los documentos seminales de Numinia,
y la estructura de roles del sistema Numinia.*

*Numinia Digital Goods v0.10.0 — Abril 2026*
