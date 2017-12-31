1. Schritt

$ sudo apt remove *pulse*

2. Schritt

$ lsusb
Bus 001 Device 004: ID 0d8c:0014 C-Media Electronics, Inc. 
Bus 001 Device 005: ID 046d:c52e Logitech, Inc. MK260 Wireless Combo Receiver
Bus 001 Device 003: ID 0424:ec00 Standard Microsystems Corp. SMSC9512/9514 Fast Ethernet Adapter
Bus 001 Device 002: ID 0424:9514 Standard Microsystems Corp. SMC9514 Hub
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub

3. Schritt

$ amixer
Simple mixer control 'PCM',0
  Capabilities: pvolume pvolume-joined pswitch pswitch-joined
    Playback channels: Mono
	   Limits: Playback -10239 - 400
		  Mono: Playback -1251 [84%] [-12.51dB] [on]

4. Schritt

$ aplay <irgendeine-audio-datei-wav-ogg-sonstwas>

Das müsste jetzt am Audio-Ausgang der Soundcard zu hören sein!

5. Schritt

$ alsamixer

Da muss jetzt der Mixer zu sehen sein .... (text-util)

6. Schritt

$ sudo mv /etc/rc0.d/K01alsa-utils /etc/rc0.d/k01alsa-utils
$ sudo mv /etc/rc0.d/K06alsa-utils /etc/rc0.d/k06alsa-utils
$ sudo /etc/init.d/alsa-utils reset

JETZT sollte alles Audio von der Soundcard-Input auch auf dem Audio-Output dieser Sound-card zu hören sein.... !!!!!!!

