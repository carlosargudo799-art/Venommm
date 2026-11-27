# Auditoría del entorno — 2026-11-27

## Sistema
- Ubuntu 24.04.5 LTS, x86_64, kernel 6.18.44. 4 vCPU, 15 GiB RAM.
- Disco: 61 GB disponibles en `/`.

## Herramientas disponibles (verificadas)
| Herramienta | Estado | Versión |
|---|---|---|
| Python | OK | 3.13.18 (pip 24.0) |
| FFmpeg / FFprobe | OK | 6.1.1 |
| Git | OK | 2.43.0 |
| Node / npm | OK | v22.23.5 / 10.9.9 |
| numpy, PIL | OK | (Python) |
| Playwright (Node) | OK | Chromium en /opt/pw-browsers |

## Herramientas que faltan
- yt-dlp — no instalado (no se instala todavía: ver «Bloqueos»).
- Whisper / faster-whisper — no instalado (transcripción pendiente).
- OpenCV, scenedetect — no instalados.
- Tesseract / OCR — no instalado.
- Playwright para Python — no instalado (el de Node sí está).

## Accesos
- Repositorio: `carlosargudo799-art/Venommm` (rama de trabajo `claude/new-session-n6mudi`).
- **kick.com: BLOQUEADO** por la política de red del entorno. `curl https://kick.com/alfredovlza/videos` devuelve `CONNECT tunnel failed, response 403`. El entorno «Default» tiene red limitada y ningún dominio permitido.
- No hay credenciales de Kick ni acceso a las cuentas de Alfredo.
- No hay directos originales en disco: ningún VOD ha sido descargado.

## Instalaciones propuestas
- Pendientes de decisión: `faster-whisper` (transcripción en español), `opencv-python-headless`, `scenedetect`, `tesseract` (OCR), `yt-dlp` (solo si se confirma un método oficial o autorizado para obtener los VOD).

## Qué puede ejecutarse ya
- Estructura de carpetas, briefing copiado, informes y registro de trabajo.
- Procesado de archivos que el usuario aporte manualmente (FFprobe, recortes, 9:16, subtítulos, captions, control de calidad).

## Qué requiere intervención
- Permiso de red para `kick.com` (y, si hace falta, el host de vídeo que use Kick), o bien los archivos originales aportados por el usuario.
