# Utilidades 

## Git

* Clonar parte de un repositorio

```
git clone -n --depth=1 --filter=tree:0 \
  <>
cd test-git-partial-clone-big-small-no-bigtree
git sparse-checkout set --no-cone small
git checkout
```

* `git log` pero mas lindo

```
git log --oneline
```

## ffmpeg

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
