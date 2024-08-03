# Utilidades 

## Git

* Clonar solo una carpeta de un repositorio

```
git clone -n --depth=1 --filter=tree:0 <repo>
cd <repo>
git sparse-checkout set --no-cone <folder>
git checkout
```

* `git log` pero mas lindo

```
git log --oneline
```

## FFMPEG

* Recortar video

```
ffmpeg -ss <HH:MM:SS> -to <HH:MM:SS> -i <input> -c copy <output>
```

* Convertir formato de audio o video

```
ffmpeg -i input.m4a output.mp3
ffmpeg -i input.avi output.mp4
```

* Extraer audio de un video

```
ffmpeg -i input-video.avi -vn -acodec copy output-audio.aac
```
