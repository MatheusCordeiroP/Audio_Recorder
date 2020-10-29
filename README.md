# Audio_Recorder

Adicionar no android manifest do app para gravar audio
<uses-permission android:name="android.permission.RECORD_AUDIO" />

Adicionar esses 2 também se for salvar o áudio no armazenamento
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.STORAGE"/>

A partir da versão 6.0 do android, a gravação de audio é considerada uma PERMISSÃO PERIGOSA
Dá uma olhada aqui se quiser detalhes:
https://developer.android.com/reference/androidx/core/app/ActivityCompat#requestPermissions(android.app.Activity,%20java.lang.String%5B%5D,%20int)

Aqui tem um aplicativo completo de gravar e ouvir, estou usando muito do código deles de base
https://www.tutorialspoint.com/android/android_audio_capture.htm

pra pegar o endereço de onde vai salvar, aparentemente pode ser usado isso
https://stackoverflow.com/questions/41365042/correct-path-to-save-file-in-android

O mediaRecorder, usado para gravar audios na memória, segue um fluxo que está representado na imagem em:
https://developer.android.com/reference/android/media/MediaRecorder.html

Encontrei esse link interessante de verificar a altura do som, mas ainda não apliquei
https://stackoverflow.com/questions/41798097/android-audiorecord-how-to-get-average-volume-for-a-minute



