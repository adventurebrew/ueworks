# Tanslation Proccess

## How we added hebrew fonts to the game

## Creating the font file

- Using an utility called "upkpacker", unpack the package file called "ExampleGame.upk" (on LifeIsStrangeGame\CookedPCConsoleFinal)

- After unpacking the package, open a file called fonts_en.SwfMovie (on SN_Font_EN/) using [JPEXS Free Flash Decompiler](https://github.com/jindrapetrik/jpexs-decompiler)

![alt text](swf_original.JPG 'Original Font File')

- Add hebrew letters to the original font - Dudu Caligraphy (need some more docs here) and saved it as "fonts_he.Swf"

![alt text](swf_after.JPG 'Font File with hebrew letters')

## Creating UPK file with the new fonts

- Download and install [UDK 2015-02 release](https://www.indiedb.com/engines/unreal-development-kit/downloads/february-2015-unreal-development-kit-udk)

- On the installation folder create the folder path "UDKGame/Flash/Fonts_he/SN_Font_HE" (make sure you're creating the folder the same root folder UDK is running from) and copy the font file there.

- Open the UDK editor and select import on the content browser window
- Select the font file and click ok

![import asset](udk_import.JPG 'import asset')
![package file](udk_package_file.JPG 'package file')

- Save the file to same directory you copied "ExampleGame.upk" from (LifeIsStrangeGame\CookedPCConsoleFinal)

![save file](udk_save.JPG 'save file')

## Configuring the game to use new font package

- On the game directory, open file "GFxUI.int" (LifeIsStrangeGame\Localization\INT\)
- Change the first fontLib to use "Fonts_HE.SN_Font_HE.fonts_he" instead of "SN_Font_EN.fonts_en"

![GFxUI](GFxUI.JPG 'GFxUI')

💯 **Congrats! You now have the ability to use hebrew text in the game.
All you have to do is edit the text files on "LifeIsStrangeGame\Localization\INT\"**

![game](game.png 'game')
