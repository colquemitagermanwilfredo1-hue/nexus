NEXUS v1.0 — Programación II

NEXUS es una aventura de exploración multiversal. El jugador registra un explorador, elige perfil y realidad, investiga anomalías con IRIS, administra energía e inventario, afronta entidades y busca extraerse para completar “LA ANOMALÍA PERDIDA”. Esta solución reúne el prototipo de consola de H3 y una primera aplicación gráfica de escritorio en C# con Windows Forms.

## Contenido y estado

- **Consola:** `nexus 3.csproj` conserva el prototipo y sus reglas.
- **Windows Forms:** `NEXUS-WindowsForms.csproj` aporta registro, selección de personaje y pantallas de exploración. Consulta `LEEME.txt` para controles y uso.
- **Solución:** `nexus v1.0.slnx` incluye ambos proyectos.
- **SQL Server:** está documentado como evolución propuesta; esta entrega no declara persistencia SQL implementada.

## Requisitos y ejecución

Se requiere Windows, Visual Studio con la carga de trabajo **Desarrollo de escritorio de .NET** y el SDK de .NET 10. Abre `nexus v1.0.slnx`. Para iniciar la interfaz, selecciona `NEXUS-WindowsForms` como proyecto de inicio; para la consola, selecciona `nexus 3`.

También se puede usar CLI:

```powershell
dotnet run --project "nexus 3.csproj"
dotnet run --project "NEXUS-WindowsForms.csproj"
```

## Documentación

- [Diseño del juego](docs/diseno-del-juego.md)
- [Arquitectura actual](docs/arquitectura-actual.md)
- [Arquitectura propuesta](docs/arquitectura-propuesta.md)
- [Modelo de datos propuesto](docs/modelo-de-datos-propuesto.md)
- [Análisis técnico](docs/analisis-tecnico.md)
- [Diagramas](docs/evidencias/diagramas.md) y [manual técnico H3](docs/NEXUS-Manual-tecnico-H3.pdf)

La interfaz Windows Forms y el prototipo de consola están presentes como proyectos. La persistencia SQL Server y la arquitectura completamente separada por capas son propuestas para etapas posteriores.
