# 🏛️ protocolo-rrpp — Skill de Protocolo Oficial y RRPP para Claude

[![Anthropic](https://img.shields.io/badge/Built%20for-Claude%20(Anthropic)-orange)](https://anthropic.com)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-blue)](LICENSE)
[![Protocolo](https://img.shields.io/badge/Marco%20legal-RD%202099%2F1983-green)](https://www.boe.es/buscar/act.php?id=BOE-A-1983-21534)

> Skill profesional para Claude que convierte cualquier consulta de protocolo oficial, empresarial, diplomático o social en tablas de precedencias justificadas, fichas visuales y documentos listos para usar.

---

## ¿Qué hace este skill?

**protocolo-rrpp** transforma a Claude en un experto en protocolo capaz de:

- ✅ Determinar qué artículo del **RD 2099/1983** aplica en cada acto
- ✅ Construir **tablas de precedencias completas y justificadas** cargo por cargo
- ✅ Generar **fichas visuales** — recepción, foto oficial, mesa de trabajo, cena de gala, banderas
- ✅ Resolver **cargos no listados** con criterio académico y profesional
- ✅ Aplicar **protocolo empresarial**, **diplomático** e internacional
- ✅ Explicar teoría de protocolo para **exámenes de RRPP**
- ✅ Producir **documentos Word y PDF** listos para imprimir

---

## Cobertura del skill

| Ámbito | Contenido |
|---|---|
| **Protocolo oficial español** | RD 2099/1983 completo: Art. 10 (Madrid capital), Art. 12 (CCAA), Art. 13 (CCAA orden) |
| **Orden ministerial** | RD 507/2021 — 22 ministerios actualizados |
| **Protocolo diplomático** | Convención de Viena 1961, cumbres OTAN, actos UE |
| **Sistemas de mesas** | Lineal, alternancia, presidencia inglesa/francesa, T, U, redonda, ovalada |
| **Comidas con señoras** | Alternancia de género, sistemas del reloj y cartesiano |
| **Protocolo empresarial** | Jerarquía corporativa, actos de empresa, reuniones bilaterales |
| **Protocolo social** | Bodas, bautizos, actos académicos, etiqueta |
| **Banderas** | Art. 13 CCAA, orden UE (27 países), criterio alfabético |

---

## Instalación

### Opción 1 — Claude.ai (interfaz web)

1. Descarga el archivo `protocolo-rrpp.skill` de la sección [Releases](../../releases)
2. Ve a **claude.ai → Settings → Skills**
3. Haz clic en **"Install skill"** y selecciona el archivo descargado
4. El skill se activará automáticamente cuando hagas consultas de protocolo

### Opción 2 — Claude Code

```bash
# Clona el repositorio
git clone https://github.com/[tu-usuario]/protocolo-rrpp.git

# Instala el skill en Claude Code
claude skill install ./protocolo-rrpp
```

### Opción 3 — Manual (cualquier entorno)

Copia el contenido de `SKILL.md` como system prompt o contexto inicial de tu conversación con Claude.

---

## Ejemplos de uso

### Ejercicio de examen universitario

```
Usuario: Tengo un ejercicio de RRPP. El Rey de España inaugura en Salamanca 
la nueva sede del CSIC. Asisten el Ministro de Ciencia, el Rector de la USAL,
el Presidente de la Junta de CyL y el Alcalde de Salamanca. 
¿Qué artículo aplica y cuál es el orden?

Claude: [Identifica Art. 12, construye tabla completa con justificación 
artículo por artículo, genera ficha de presidencia]
```

### Organización de acto real

```
Usuario: Necesito organizar la foto oficial de nuestra cumbre bilateral 
con 7 participantes: [lista de cargos]. Genera la ficha.

Claude: [Determina sistema de alternancia impar, genera diagrama 
con posición exacta de cada autoridad]
```

### Protocolo empresarial

```
Usuario: Organizo una cena de gala en mi empresa con el CEO, 
3 directivos y 2 clientes importantes con sus parejas (8 personas).
¿Cómo coloco la mesa?

Claude: [Aplica protocolo empresarial, genera mesa presidencia 
francesa con alternancia de género]
```

---

## Estructura del repositorio

```
protocolo-rrpp/
├── SKILL.md                          # Skill principal — punto de entrada
├── README.md                         # Este archivo
├── LICENSE                           # MIT License
├── references/
│   ├── 01-marco-legal.md             # RD 2099/1983, árbol de decisión, principios
│   ├── 02-precedencias-completas.md  # Art. 10, Art. 12, Art. 13 completos + ministerios
│   ├── 03-sistemas-mesas.md          # Todos los sistemas con diagramas
│   └── 04-07-protocolo-empresarial-diplomatico-social-outputs.md
└── evals/
    └── evals.json                    # Casos de prueba
```

---

## Marco legal

Este skill se basa en:

- **Real Decreto 2099/1983**, de 4 de agosto — Ordenamiento General de Precedencias del Estado
- **Real Decreto 507/2021**, de 10 de julio — Estructura ministerial actualizada
- **Real Decreto 508/2021** — Vicepresidencias del Gobierno
- **Real Decreto 372/2020**, de 18 de febrero — Estructura orgánica del Ministerio de Defensa
- **Convención de Viena sobre Relaciones Diplomáticas** (1961)
- **Reglamento 2/2005 del CGPJ**, de 23 de noviembre
- **Libro de Estilo de la Unión Europea** — apartado 7.1 (orden de banderas)

---

## Contribuir

¡Las contribuciones son bienvenidas! Especialmente:

- 📝 Correcciones legales (actualizaciones del RD, nuevos ministerios…)
- 🌍 Protocolo de otras instituciones internacionales (ONU, OSCE, NATO…)
- 🎓 Casos prácticos reales para los evals
- 🌐 Traducciones (inglés, francés, portugués)

### Cómo contribuir

1. Fork del repositorio
2. Crea una rama: `git checkout -b mejora/nombre-de-la-mejora`
3. Commit con mensaje descriptivo: `git commit -m "feat: añade protocolo actos UE"`
4. Push: `git push origin mejora/nombre-de-la-mejora`
5. Abre un Pull Request

---

## Colaboradores

| Colaborador | Rol |
|---|---|
| [Tu nombre] | Autor y mantenedor principal |
| **Anthropic** | Plataforma Claude — colaborador institucional |

---

## Licencia

MIT License — ver [LICENSE](LICENSE)

---

## Agradecimientos

- Al profesorado de RRPP y Protocolo de las universidades españolas
- A los profesionales del protocolo oficial que documentan y actualizan estas normas
- A [carlosfuente.es](https://carlosfuente.es) por la recopilación de precedencias actualizadas
- A Anthropic por la plataforma Claude y el sistema de skills

---

*Desarrollado con ❤️ para estudiantes y profesionales de las Relaciones Públicas y el Protocolo en España*
