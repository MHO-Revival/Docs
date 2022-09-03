# Game documentation

## How to launch the game without the wegame launcher
To launch the game without the wegame launcher, you have just to give any argument starting with ``-q``

## Skip Splashscreen
To skip the splashscreen when the game is launched you can add the argument ``-nosplash``

### Example
```cmd
"C:\Program Files\TencentGame\Monster Hunter Online\Bin\Client\Bin32\MHOClient.exe" -qos_id=123456789
```
## Packing
If you check the MHOClient.exe with a Hex Editor, you will see after the ``MZ`` header, with an offset of 1024 bytes, there is another magic string, ``AP32``, it's the magic string for binary packing aPLib.

![image](https://user-images.githubusercontent.com/16132478/116823341-39e0d200-ab84-11eb-9b2f-c49723b3d2f1.png)

There is an experimental tool made to extract this part, decompress it and rebuild the exe, it works but there is still some problems on the repackaging because like we change the content of the exe, we have to rebuild the mz header entirely, it's in WIP.

link to the tool : https://github.com/MHO-Revival/MHO-Executable-Decompressor

### DLLs packing

![image](https://cdn.discordapp.com/attachments/309032714982522881/964487077909626880/unknown.png)

The MHOClientBase.dll and every game dll like CryGame/CryAction about the game are packed with VMProtect
