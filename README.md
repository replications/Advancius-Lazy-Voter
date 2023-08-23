# Advancius-Lazy-Voter
Opens all 10 voting websites for Advancius Network. Never vote manually again!







Source code below.
@echo off
setlocal
:menu
cls
title Lazy Voter 1.0 - Made by idolizer
echo Advancius Lazy Voter
echo Created by idolizer
echo [94msoho#1515
echo [37m=================
echo Menu
echo [32m1. Start Vote Sequence
echo [31m2. Exit
echo [37m=================
set /p choice=Menu^> 
if %choice%==1 goto voteseq
if %choice%==2 exit /b
echo Invalid choice
timeout /t 1 /nobreak >nul
goto menu

:voteseq
cls
echo Vote 1
start https://minecraft.buzz/vote/1184
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 2
start https://topminecraftservers.org/vote/16049
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 3
start https://minecraftservers.org/vote/478339
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 4
start https://minecraftpocket-servers.com/server/114787/vote/
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 5
start https://minecraft-mp.com/server/184363/vote/
echo Press any key once done
pause >nul
echo Wait...
echo Vote 6
start https://best-minecraft-servers.co/server-advancius-network.185/vote
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 7
start https://minecraft-server-list.com/server/416425/vote/
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 8
start https://servers-minecraft.net/server-advancius-network.721
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 9
start https://minecraftbestservers.com/server-advancius.53/vote
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo Vote 10 (Final Vote)
start https://www.planetminecraft.com/server/advancius-network/vote/
echo Press any key once done
pause >nul
echo Wait...
timeout /t 1 /nobreak >nul
echo =================
cls
echo Done! Return to your game to enjoy your keys!
echo [0mPress any key to exit.
echo [97mYou[91mTube[0m.com/[96mArislaz
pause >nul
exit /b


:parsejson
set string=%string:"=%
set "string=%string:~2,-2%"
set "string=%string:: ==%"
set "%string:, =" & set "%"
goto :eof
