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

Install the english patch in the same path it's showing in the 7zip file (otherwise you will not be able to create new character, if it shows you a little textbox with a green message, see picture below, that's because the english patch is missing), the only file it will replace is the IIPSFileList.lst, it contains all the .ifs files that MHO needs + the english patch.

![Green message](https://private-user-images.githubusercontent.com/23282377/476175299-dea15393-a094-463e-a6a2-f632bd472e63.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ2ODUyMDQsIm5iZiI6MTc1NDY4NDkwNCwicGF0aCI6Ii8yMzI4MjM3Ny80NzYxNzUyOTktZGVhMTUzOTMtYTA5NC00NjNlLWE2YTItZjYzMmJkNDcyZTYzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODA4VDIwMjgyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQwOGQwNmI1NzE5YzJiZmZmYThhZWY5NjUyOTExM2RlNGM4MjFlYzUwYTk4YWIwMjgyZWM0NzMwMDcyZDY1MDcmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.7DXGBf-GkWLHeqsV1zCSfMGETHNInIhYuuuXlt22sJM)

You will have to build the launcher by yourself.

Download the Launcher project and put it where you want (mine is E:\jeux\MONSTER HUNTER ONLINE\mho_launcher).


Launch Visual Studio, select folder and follow theses steps to build it :

- The project need a compiler to build correctly, it should compile in x86-Release :

![Compiler image](https://private-user-images.githubusercontent.com/23282377/476175302-ff3513d6-7690-46f6-a1b7-b1c080e825f1.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ2ODUxNDEsIm5iZiI6MTc1NDY4NDg0MSwicGF0aCI6Ii8yMzI4MjM3Ny80NzYxNzUzMDItZmYzNTEzZDYtNzY5MC00NmY2LWExYjctYjFjMDgwZTgyNWYxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODA4VDIwMjcyMVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU2NTdiZmQzMzc1ODNjOTM3YjlmY2FiZjc4OGFmZWE5ZDI2MDA1NTM2MzY1NjUwMmFhMGI5NzliZDc1YzRkMWYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.BTd6j2Do-CiWYXwU1yxDN9Spp-2zdxSy3ssbhcL4u14)

- Next, build the project with this icon :

![Build image](https://private-user-images.githubusercontent.com/23282377/476175301-7c6db59e-b117-4012-8de0-60416bd38bb9.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ2ODUyMDQsIm5iZiI6MTc1NDY4NDkwNCwicGF0aCI6Ii8yMzI4MjM3Ny80NzYxNzUzMDEtN2M2ZGI1OWUtYjExNy00MDEyLThkZTAtNjA0MTZiZDM4YmI5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODA4VDIwMjgyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTYxZWNhMjU4NjJlNTk2YzY2YTBjMTczMWIwMDBhMjM5ZjhhMzUwODllNWUxMjA1ZGY2YmM4YTcyNDFlZDQzZmYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.p-dCiYNAl9jknJ5DExY4ryKSJv7AwGOKQH8ZuZsNbd0)

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

![Notepad image](https://private-user-images.githubusercontent.com/23282377/476175300-106c1a95-c7ab-40e2-9fd5-ff591b88efa1.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ2ODUyMDQsIm5iZiI6MTc1NDY4NDkwNCwicGF0aCI6Ii8yMzI4MjM3Ny80NzYxNzUzMDAtMTA2YzFhOTUtYzdhYi00MGUyLTlmZDUtZmY1OTFiODhlZmExLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODA4VDIwMjgyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWMyNmM3YTQzOWI2ODNlNzQzZGY2Mzg3MGFmNjlkMjkyMDg0Njc4MmZjZjE1ZmEwNDAyZjI0ODZjNjkwNmEyN2YmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.-eRrq0fYDO3fONAvJLpXRzhRwRJCWyv8Ag4LG8IuBBM)

## Server installation

Download the server files (Server source code) and put it where you want (mine is E:\jeux\MONSTER HUNTER ONLINE\Arrowgene.MonsterHunterOnline)

With Visual Studio, select the project .sln, and configure the debugging properties and put "service start" :

![Service start image](https://private-user-images.githubusercontent.com/23282377/476175298-6572371d-884a-496b-bf67-d8c0ce0dc75d.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ2ODUyMDQsIm5iZiI6MTc1NDY4NDkwNCwicGF0aCI6Ii8yMzI4MjM3Ny80NzYxNzUyOTgtNjU3MjM3MWQtODg0YS00OTZiLWJmNjctZDhjMGNlMGRjNzVkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODA4VDIwMjgyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTJiM2MwM2ZjYjA2MWNhZjU0MmRhMmIzMzE3OGZmZjgzNmQ0MGFjMThhZmMzMjE0NGVjMDBlM2E3NGQ4MjlkNTkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.1wUt9drO6LVSWH9BpfsPdXPb9JfQEP7Jfxy4uXfWyTE)



## Final step, run everything

Run the ArrowGene.MonsterHunterOnline.Cli and you should get that cmd window :

![Cmd window image](https://private-user-images.githubusercontent.com/23282377/476175297-6c7ba234-25a8-46c4-bf99-30e8d57ce4be.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ2ODUyMDQsIm5iZiI6MTc1NDY4NDkwNCwicGF0aCI6Ii8yMzI4MjM3Ny80NzYxNzUyOTctNmM3YmEyMzQtMjVhOC00NmM0LWJmOTktMzBlOGQ1N2NlNGJlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODA4VDIwMjgyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBmOTJlOTlkYTFkMDc3ZDQ3OTEwYzU4Yjg4NTI0NzFmZWFmZTdkYWQ4ZmE3MjhlMDFlZGVkNTQ2MjhiZTU2MmMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.CfjXgP85YrXkrZ4jRRknN4y-pg9d2HukTUHyeENXhqs)

Next you can go inside your game installation (mine is C:\Program Files (x86)\TencentGame\Monster Hunter Online\Bin\Client\Bin32) and launch the mho_launcher.exe

You should get another cmd window, press Enter and it should close the cmd to open another one.
Sometimes the 2nd cmd can crash (sometimes it happened 5-6 times in a row for me), just open the launcher again.

Ta-da, your inside the game, create a caracter and cruise around !


## FAQ

Q: I get a green message in a small box, what is it ? 

![Green message](https://private-user-images.githubusercontent.com/23282377/476175299-dea15393-a094-463e-a6a2-f632bd472e63.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ2ODUyMDQsIm5iZiI6MTc1NDY4NDkwNCwicGF0aCI6Ii8yMzI4MjM3Ny80NzYxNzUyOTktZGVhMTUzOTMtYTA5NC00NjNlLWE2YTItZjYzMmJkNDcyZTYzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODA4VDIwMjgyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQwOGQwNmI1NzE5YzJiZmZmYThhZWY5NjUyOTExM2RlNGM4MjFlYzUwYTk4YWIwMjgyZWM0NzMwMDcyZDY1MDcmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.7DXGBf-GkWLHeqsV1zCSfMGETHNInIhYuuuXlt22sJM)

A: You didn't installed the english patch, check again the first step.
