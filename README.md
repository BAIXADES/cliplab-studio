# ClipLab Studio

ClipLab Studio és un editor web gratuït que processa els vídeos al navegador. No utilitza crèdits, monedes virtuals, subscripcions, pagaments ni marques d'aigua.

## Obrir l'aplicació

https://baixades.github.io/cliplab-studio/

## Funcions disponibles

- Importar fitxers locals de vídeo i arrossegar-los a l'editor.
- Importar una URL directa a un fitxer de vídeo HTTP/HTTPS, sempre que el servidor permeti CORS i el navegador admeti el còdec.
- Reproduir vídeos de YouTube o Vimeo dins del reproductor oficial com a previsualització; aquests reproductors no es poden retallar ni exportar des de ClipLab.
- Seleccionar temps d'inici i final, format 9:16, 1:1 o 16:9 i crear diversos clips.
- Afegir subtítols manuals, triar-ne el color, la mida i la posició.
- Ajustar zoom, brillantor, saturació i desenfocament global.
- Analitzar localment l'energia de l'àudio i proposar fragments al voltant dels pics de volum. Això és una heurística de volum, no una IA que entengui el significat de la conversa.
- Exportar el clip seleccionat a WebM mitjançant MediaRecorder del navegador, amb la pista d'àudio quan el navegador permet capturar-la.

## Importació per URL: limitacions tècniques

Enganxa una URL que apunti directament al fitxer, per exemple a un recurs MP4 o WebM. Un enllaç a una pàgina web, a una pàgina de compartir o a un reproductor no és una URL directa del fitxer.

Per motius de seguretat del navegador, els vídeos allotjats en altres dominis necessiten que el servidor d'origen permeti CORS (per exemple, una capçalera Access-Control-Allow-Origin adequada). Si el servidor no dona aquest permís, el navegador pot impedir la càrrega o la captura per a l'exportació.

Els enllaços de YouTube es mostren amb el reproductor oficial, però no s'extreu ni es descarrega el vídeo. Consulta les condicions de YouTube i les polítiques de la seva API: https://www.youtube.com/t/terms i https://developers.google.com/youtube/terms/developer-policies

## Funcions que no estan activades

Aquesta versió no incorpora encara detecció semàntica de moments amb un model d'IA, transcripció Whisper, subtítols sincronitzats automàticament, seguiment de cares, desenfocament selectiu, millora neuronal de l'àudio, monitoratge de directes, publicació automàtica a xarxes socials ni sincronització de comptes/projectes al núvol. La interfície no simula aquestes funcions.

## Privacitat i gratuïtat

Els vídeos seleccionats o les URL directes són processats pel navegador de l'usuari; ClipLab no els envia a un servidor propi. Els vídeos exportats es creen al dispositiu. La disponibilitat i el rendiment depenen del navegador, del còdec, de la memòria i de les capçaleres CORS del servidor d'origen.
