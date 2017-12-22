# Ton Weiterleitung zwischen Applikationen in Linux
Wenn das Linux System PulseAudio hat, dann ist es ganz einfach.
Beide Applikationen mit PulseAudio als Ausgabe bzw. Eingabe Schnittstelle
auswählen. Dann mit dem PulseAudio Steuerungsapplikation (z.B. pavucontrol)
in der Recording Reiter als "Capture Source"  "Monitor of Built-in Audio" 
auswählen.
# Erster Versuch heute mit Alsa-Mixer (dk2vh)
"pavucontrol" will nicht mit meinem Alsa auf dem Ubuntu 16.04 LTS zusammenarbeiten. Es lässt sich keine Verbindung von Audio-Ausgang zum Mic-Eingang herstellen. Ich weiß im Moment nicht, ob überhaupt der Audio-Ausgang (egal ob default oder hdmi) auf eine fremde Applikation pipen lässt. Ich habe hoffentlich alle Varianten ausprobiert (aus Aufnahme-App habe ich audacity verwendet, weil ich da hätte sehen können, dass tatsächlich was aufgefangen wird, außerdem lassen sich dann alle Ein-/Ausgänge unter Zuhilfenahme von pulsaudio auswählen), aber ich habe keine Verbindung von Audio zu App herstellen können.
# Mögliche Ursachen: (dk2vh)
Ich nehme an, dass etwas mit den config-Dateien nicht stimmt. Wo kann ich eine Liste der möglichen conf-Einstellungen von Alsa und pulsaudio einsehen? (URL)
