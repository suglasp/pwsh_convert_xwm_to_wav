
*.xwm to *.wav sound converter
-------------------------------

Used for the Fallout sfx conversion kit. See project https://github.com/suglasp/fallout4_fallout76_sfx_conversionkit .

This is a wrapper script that uses xWMAEncode behind the scenes to convert in bulk xmp files to wav.
You can target a folder, and the scripts will convert any xmp file (also in subfolders) to wav.

Setup:
Download convert_xwm_to_wav.ps1 to a folder.
Create a subfolder (in the same root folder where you put convert_xwm_to_wav.ps1) with the name "xWMAEncode".
Download xWMAEncode utility from https://www.nexusmods.com/skyrim/mods/32075/?tab=files and extract to folder "xWMAEncode". (**)

Usage:
Start Powershell (works in Powershell 7 to on Windows).
Run .\convert_xwm_to_wav.ps1 -CustomDir <path_to_target_folder>

If a .xmp file is seen, it will convert it to wav (wave) and place the new file next to the xmp file.
In case a wav file with the same name as the xmp file exists, the script will skip the file and notify you.


(**) You can also get xWMAEncode.exe from the Legacy DirectX SDK from June 2010.
One can install the SDK or just open the original install file with 7-Zip.
It's located under .\DXSDK\Utilities\bin\x86\xWMAEncode.exe
https://www.microsoft.com/en-ca/download/details.aspx?id=6812


Pieter a.k.a. Suglasp
