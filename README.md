![](https://github.com/Audiveris/docs/blob/master/images/SplashLogo.png)

# Audiveris - Open-source Optical Music Recognition

## Installation

```
./gradlew build
```

Within /usr/share/tesseract-ocr/ create the folder structure 3.04/tessdata.
From https://github.com/tesseract-ocr/tessdata/tree/3.04.00 download the eng.traineddata, deu.traineddata and fra.traineddata files and put them in the 3.04 folder.
Set the TESSDATA_PREFIX environment variable to 

```
/usr/share/tesseract-ocr/3.04/
```

## Usage

Now you can run audiveris with

```
./gradlew run
```

With the program, load an image file of the sheet music through File -> Input
To automatically detect the sheet music press Book -> Transcribe Book
Now export the detected notes to an .mxl file through  Book -> Export Book

This .mxl file can be played by a different program. For instance, use MuseScore:

You can download the AppImage from https://musescore.org/en/handbook/3/install-linux#AppImage

Just execute the AppImage file and within the GUI, click File -> open and select the previously created .mxl file.

The notes can be played simply by pressing the Play button on the top right.
