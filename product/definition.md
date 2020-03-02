# Introduction 

The Jukeberry project is intended to generate beautiful geeky mini-jukeboxes, powered Raspberries for everyone to build.

It was originally inspired by other DIY projects using RFID cards to determine what to play next. I imagined endless possibilities for a gadget like this, and so, I'm creating this repo in an attempt of planning, taking notes, writing ideas down, and finally, start building it.

## First EPICs


### Jukeberry manager

* For identification porpuses, the Jukeberry should count with a unique identifier. The user might want to add an alias too, but unique identifier will prevent devices to connect to an incorrect Jukeberry

### Player

* When a user brings an RFID card close to the jukebox, it will start playing the corresponding song right away. [MVP]
* If the user holds the "add to queue" button while passing the RFID card, the song won't play right away but will be added to a queue.
* There will be another button to toggle a random order on and off.
* By default, Jukebox will use its speakers (connected via Bluetooth, plug, HDMI, etc). However, it will be possible to connect compatible devices to Jukeberry to play the corresponding songs.
  * In case having more than one connected device, a button will let the user choose which one should be reproducing a song.

### Media manager

* To have a card related to a song, we need a UI:
  - Scan the card and upload a song. [MVP]
  - Save the card art with the song
  - Save some information about the song
  - Specify a link to Spotify / Youtube
  - Upload a song and assign the card later (when you are in front of an RFID reader)
  - Pick up a previously uploaded song and scan the card (Media manager directly on the device)

### Devices Manager

* Register a compatible device in Jukeberry: The compatible device should be able to read notifications from a queue (or other mechanisms). 
* The Devices Manager should show all the connected devices and allow unpairing

### Guests mode

* Guests will be able to choose one song associated with a personal card (we could check if it works with cards such as [SUBE](https://www.argentina.gob.ar/sube) or other public ones). 
* When a guest comes home, they will be allowed to play their song by passing the card

