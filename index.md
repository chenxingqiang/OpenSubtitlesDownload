Introduction
------------

**OpenSubtitlesDownload.py** is a small Linux software written in python, built to help you **quickly find and download subtitles for your favorite videos**. It can be used as a nautilus script, or as a regular application working under GNOME or KDE desktop environments. You can also use it in full CLI mode (Command Line Interface) on your NAS, Raspberry Pi or wherever you want to bundle it really!

The subtitles search is done by precisly **identifying your video files** by computing unique movie hash sums. This way, you have more chance to find the **exact subtitles for your videos**, avoiding synchronization problems between the subtitles and the soundtrack. But what if that doesn't work? Well, a search with the filename will be performed, but be aware: results are a bit more... unpredictable (don't worry, you will be warned! and you can even disable this feature if you want).

The subtitles search and download service is powered by [opensubtitles.org](http://www.opensubtitles.org). Big thanks to their hard work on this amazing project! Be sure to [give them your support](http://www.opensubtitles.org/en/support) if you appreciate the service provided, they sure need donations for handling the ever growing hosting costs!

Features
--------

- Use a GNOME/GTK or KDE/Qt GUI depending on your favorite desktop environment.
- Or just use the CLI! Great for automation, and it works on Linux and Mac OS.
- Query subtitles in more than 60 different languages for documentaries, movies, TV shows and more...
- Query subtitles in multiple languages at once.
- Query subtitles for multiple video files at once.
- Detect valid video files (using mime types and file extensions).
- Detect correct video titles by computing unique movie hash sums in order to download the right subtitles for the right file!
- If the video detection fails, search by filename will be performed as backup method.
- Download subtitles automatically if only one is available, choose the one you want otherwise.
- Rename downloaded subtitles to match source video file. Possibility to append the language code to the file name (ex: movie_en.srt).

Screenshots!
------------

![Start subtitles search](https://raw.githubusercontent.com/emericg/OpenSubtitlesDownload/screenshots/osd_screenshot_launch.png)

![Download selected subtitles](https://raw.githubusercontent.com/emericg/OpenSubtitlesDownload/screenshots/osd_screenshot_autodownload.png)

Enjoy your subtitled video!
![Enjoy your subtitled video!](https://raw.githubusercontent.com/emericg/OpenSubtitlesDownload/screenshots/enjoy-sintel.jpg)

If multiple subtitles are available, just pick one from the list!
![Multiple subtitles selection](https://raw.githubusercontent.com/emericg/OpenSubtitlesDownload/screenshots/osd_screenshot_selection.png)

You can even enables more infos on the selection windows:
![Custom subtitles selection](https://raw.githubusercontent.com/emericg/OpenSubtitlesDownload/screenshots/osd_screenshot_selection_custom.png)

Use OpenSubtitlesDownload to search for subtitles in different languages simultaneously:
![Multiple languages](https://raw.githubusercontent.com/emericg/OpenSubtitlesDownload/screenshots/osd_screenshot_selection_language.png)

Installation
------------

### Requirements
- python (version 2 or 3)
- zenity (only for GNOME based desktop environments)
- kdialog (only for KDE based desktop environments)
- basic unix tools: wget & gzip (subtitles downloading), ps & grep (GUI autodetection)

### Download
You can download the latest developer version with the downloads buttons on the header of this page, or you can find various versions and release note of OpenSubtitlesDownload on [the releases page](https://github.com/emericg/OpenSubtitlesDownload/releases)!

### Quick installation
Quick installation as a nautilus script, under GNOME 3 desktop environment:

> $ git clone https://github.com/emericg/OpenSubtitlesDownload.git  
> $ mkdir -p ~/.local/share/nautilus/scripts/  
> $ cp OpenSubtitlesDownload/OpenSubtitlesDownload.py ~/.local/share/nautilus/scripts/OpenSubtitlesDownload.py  
> $ chmod u+x ~/.local/share/nautilus/scripts/OpenSubtitlesDownload.py  

### Installation
* [Usage as a regular CLI script](https://github.com/emericg/OpenSubtitlesDownload/wiki/Usage-as-a-regular-CLI-script)
* [Usage as a nautilus script](https://github.com/emericg/OpenSubtitlesDownload/wiki/Usage-as-a-nautilus-script) (preferred method)
* [Installation under GNOME desktop environment](https://github.com/emericg/OpenSubtitlesDownload/wiki/Installation-under-GNOME-desktop-environment)
* [Installation under KDE desktop environment](https://github.com/emericg/OpenSubtitlesDownload/wiki/Installation-under-KDE-desktop-environment)

### Adjust various settings

After the installation you can **adjust several settings** to make OpenSubtitlesDownload.py an even **better experience** suiting your every needs! Learn more on the [Adjust settings](https://github.com/emericg/OpenSubtitlesDownload/wiki/Adjust-settings) wiki page.

Available **settings** includes:

- Language selection
- Full automatic mode
- GUI window size
- Additionnal columns for the subtitles selection window
- Language codes embedded into the subtitles files names
- And more!

Contributors
------------

- Emeric Grange <emeric.grange@gmail.com> maintainer
- jeroenvdw for his work on the 'subtitles automatic selection' and the 'search by filename' features
- Gui13 for his work on the arguments parsing
- Tomáš Hnyk <tomashnyk@gmail.com> for his work on the 'multiple language' feature
- Carlos Acedo <carlos@linux-labs.net> for his work on the original script

License
-------

OpenSubtitlesDownload.py is a free software released under the GPL v3 license <http://www.gnu.org/licenses/gpl-3.0.txt>