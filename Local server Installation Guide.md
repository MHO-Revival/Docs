# Arrowgene.MonsterHunterOnline

## Prerequisites

- Visual Studio Community (https://visualstudio.microsoft.com/downloads/)
- .NET 7 SDK (https://dotnet.microsoft.com/en-us/download/dotnet/7.0)
- Game (https://mega.nz/file/F8hV1AjZ#qh7kYq53p2yKX8sFmrNnvBL5EsScEXzKp_1XF-Upj8k)
- Decompressed MHOClient (https://mega.nz/file/sKNDAZyJ#K6RYgCCvEye9eGGiIBRomkn5zxKCDEEAPiUCi45ZJa8)
- English Patch (https://mega.nz/file/oaFwWKSY#5I5b21AV9F2kWGB2QahA7W6ZKokH5r93o7lIq3bwk9o)
- Launcher (https://github.com/sebastian-heinz/mho_launcher)
- Server source code (https://github.com/sebastian-heinz/Arrowgene.MonsterHunterOnline)

⚠️⚠️⚠️If images doesn't show that means my server is down ⚠️⚠️⚠️

## First steps, the game installation

Install the game to whatever folder you want (mine is C:\Program Files (x86)\TencentGame\Monster Hunter Online\Bin\Client\Bin32)

Install the decompressed MHOClient inside the game installation just freshly installed.

Install the english patch in the same path it's showing in the 7zip file (otherwise you will not be able to create new character, if it shows you a little textbox, that's because the english patch is missing), the only file it will replace is the IIPSFileList.lst, it contains all the .ifs files that MHO needs + the english patch.

You will have to build the launcher by yourself.

Download the Launcher project and put it where you want (mine is E:\jeux\MONSTER HUNTER ONLINE\mho_launcher).


Launch Visual Studio, select folder and follow theses steps to build it :

- The project need a compiler to build correctly, it should compile in x86-Release :
![Compiler image](http://136.243.63.156:10782/images/mho_guide1.png)
- Next, build the project with this icon :
![Build image](http://136.243.63.156:10782/images/mho_guide2.png)
- Find the output files in the folder : LOCATION"\mho_launcher\out\build\x86-Release (mine is E:\jeux\MONSTER HUNTER ONLINE\mho_launcher\out\build\x86-Release)
- Copy mho_launcher.exe + mho_launcher_lib.dll inside your game installation (mine is C:\Program Files (x86)\TencentGame\Monster Hunter Online\Bin\Client\Bin32)

Next part is only to prevent crash report to be send to a unknown host, so it will just send the reports to yourself.

So in the host file (located at C:\Windows\System32\drivers\etc)

Add thoses lines :
```
127.0.0.1 tqos.gamesafe.qq.com
127.0.0.1 down.qq.com
127.0.0.1 stat.iips.qq.com
127.0.0.1 ied-tqos.qq.com
127.0.0.1 apps.game.qq.com
```

Edit the file with notepad to get something similar
![Notepad image](http://136.243.63.156:10782/images/mho_guide5.png)

## Server installation

Download the server files (Server source code) and put it where you want (mine is E:\jeux\MONSTER HUNTER ONLINE\Arrowgene.MonsterHunterOnline)

With Visual Studio, select the project .sln, and configure the debugging properties and put "service start" :
![Service start image](http://136.243.63.156:10782/images/mho_guide3.png)



## Final step, run everything

Run the ArrowGene.MonsterHunterOnline.Cli and you should get that cmd window :
![Cmd window image](http://136.243.63.156:10782/images/mho_guide4.png)

Next you can go inside your game installation (mine is C:\Program Files (x86)\TencentGame\Monster Hunter Online\Bin\Client\Bin32) and launch the mho_launcher.exe

You should get another cmd window, press Enter and it should close the cmd to open another one.
Sometimes the 2nd cmd can crash (sometimes it happened 5-6 times in a row for me), just open the launcher again.

Ta-da, your inside the game, create a caracter and cruise around !
