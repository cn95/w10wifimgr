# netsh wlan show profiles
# netsh wlan show profiles name= key=clear
echo off
goto question

:ShowAllKnownNames
cls
netsh wlan show profiles
pause
goto question

:ShowPasswordByName
cls
set /p name=Set a name of Wi-Fi: 
netsh wlan show profiles name=%name% key=clear
pause
goto question

:ConnetByName
cls
set /p name=Set a name of Wi-Fi: 
netsh wlan connect %name%
pause
goto question

:Disconnet
cls
netsh wlan disconnect
pause
goto question

:ShowAllNames
cls
netsh wlan show networks
pause
goto question

:GetPing
cls
ping google.com
pause
goto question

:question
cls
echo 1. Show Wi-Fi known names
echo 2. Show Wi-Fi password by Wi-Fi name
echo 3. Connect to Wi-Fi by Wi-Fi name
echo 4. Disconnect to Wi-Fi
echo 5. Show all avaible Wi-Fi names
echo ------------------------------------------
echo 6. Get internet connection

set /p case=Set a task: 
if %case% == 1 (goto ShowAllKnownNames)
if %case% == 2 (goto ShowPasswordByName)
if %case% == 3 (goto ConnetByName)
if %case% == 4 (goto Disconnet)
if %case% == 5 (goto ShowAllNames)
if %case% == 6 (goto GetPing)
pause
