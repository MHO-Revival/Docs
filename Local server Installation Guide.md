#Arrowgene.MonsterHunterOnline

##Prerequisites

- Visual Studio Community (https://visualstudio.microsoft.com/downloads/)
- .NET 7 SDK (https://dotnet.microsoft.com/en-us/download/dotnet/7.0)
- Game (https://mega.nz/file/F8hV1AjZ#qh7kYq53p2yKX8sFmrNnvBL5EsScEXzKp_1XF-Upj8k)
- Launcher (https://github.com/sebastian-heinz/mho_launcher)
- Server source code (https://github.com/sebastian-heinz/Arrowgene.MonsterHunterOnline)
- others ()

## First steps, the game installation

Install the game to whatever folder you want (mine is C:\Program Files (x86)\TencentGame\Monster Hunter Online\Bin\Client\Bin32)

You will have to build the launcher by yourself
Download the Launcher project and put it where you want (mine is E:\jeux\MONSTER HUNTER ONLINE\mho_launcher)


Launch Visual Studio, select folder and follow theses steps to build it :

- The project need a compiler to build correctly, it should compile in x86-Release :
![alt text](https://cdn.discordapp.com/attachments/597845868841795604/1151228212714680431/image.png)
- Next, build the project with this icon :
![alt text](https://cdn.discordapp.com/attachments/597845868841795604/1151229689176797257/image.png)
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
![alt text](https://cdn.discordapp.com/attachments/597845868841795604/1151237180321177711/image.png)

## Server installation

Download the server files (Server source code) and put it where you want (mine is E:\jeux\MONSTER HUNTER ONLINE\Arrowgene.MonsterHunterOnline)

With Visual Studio, select the project .sln, and configure the debugging properties and put "service start" :
![alt text](https://cdn.discordapp.com/attachments/597845868841795604/1151232832581156894/image.png)



## Final step, run everything

Run the ArrowGene.MonsterHunterOnline.Cli and you should get that cmd window :
![alt text](https://cdn.discordapp.com/attachments/597845868841795604/1151233757471326299/image.png)

Next you can go inside your game installation (mine is C:\Program Files (x86)\TencentGame\Monster Hunter Online\Bin\Client\Bin32) and launch the mho_launcher.exe

You should get another cmd window, press Enter and it should close the cmd to open another one.
Sometimes the 2nd cmd can crash (sometimes it happened 5-6 times in a row for me), just open the launcher again.

Ta-da, your inside the game, create a caracter and cruse around !