# video2mp4

Convierte automáticamente todos los videos de la carpeta actual a formato MP4 usando FFmpeg en Windows.

## Instrucciones

1. Coloca tus videos (de cualquier formato) en la misma carpeta que el script.
2. Ejecuta el archivo `convertir_a_mp4.bat`.
3. Los videos convertidos aparecerán en formato `.mp4`.

### Requisitos

- Windows 10 o superior
- PowerShell (incluido en Windows)
- ffmpeg.exe (ver instrucciones abajo para descargarlo)

### Notas

 Necesitarás `ffmpeg.exe`. Puedes descargarlo manualmente desde [ffmpeg.org](https://ffmpeg.org/download.html) o ejecuta este comando en PowerShell para descargarlo automáticamente:

 ```powershell
 Invoke-WebRequest -Uri "https://www.gyan.dev/ffmpeg/builds/ffmpeg-release-essentials.zip" -OutFile "ffmpeg.zip"
 Expand-Archive -Path "ffmpeg.zip" -DestinationPath "."
 Copy-Item ".\ffmpeg-*-essentials_build\bin\ffmpeg.exe" .
 Remove-Item "ffmpeg.zip"
 ```
 Esto descargará y extraerá `ffmpeg.exe` en la carpeta actual.

## Licencia

MIT