<h1 align="center">Headless Client</h1>
<p align="center">
    <a href="https://github.com/ArmaLife/HC">
        <img src="https://img.shields.io/badge/version-v4.4-green.svg" alt="Life HC Version">
    </a>
    &nbsp;&nbsp;&nbsp;
    <a href="https://github.com/ArmaLife/HC/releases">
        <img src="https://img.shields.io/badge/release-1-yellowgreen.svg" alt="Life HC Release">
    </a>
    &nbsp;&nbsp;&nbsp;
    <a href="http://dev.arma3.com/post/spotrep-00052">
        <img src="https://img.shields.io/badge/arma%203-1.56-orange.svg" alt="Arma 3 Version">
    </a>
    &nbsp;&nbsp;&nbsp;
    <a href="https://gitter.im/ArmaLife/Altis?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge">
        <img src="https://badges.gitter.im/ArmaLife/Altis.svg" alt="Join the chat at https://gitter.im/ArmaLife/Altis">
    </a>
    &nbsp;&nbsp;&nbsp;
    <a href="https://gitter.im/ArmaLife/Altis/Support?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge">
        <img src="https://img.shields.io/badge/support-on%20gitter-blue.svg" alt="Join the support chat at https://gitter.im/ArmaLife/Altis/Support">
    </a>
</p>

<b>Life HC</b> or <b>[Life HC RPG] (http://www.altisliferpg.com)</b> is developed by <b>Tonic</b> AKA <b>[TAW_Tonic] (https://github.com/TAWTonic)</b>.<br/>
This contains primarily the release contain and on-going development changes to the mission.<br/>
<br/>
Life HC RPG by Tonic is licensed under a [Creative Commons Attribution-NonCommercial-NoDerivs 3.0 Unported License] (http://creativecommons.org/licenses/by-nc-nd/3.0/deed.en_US)<br/>
By using the framework and/or code inside the framework, you agree to the [terms of agreement] (README.md/#usage--terms-of-agreement).<br/>
The terms are subjected to be changed over time.<br/>

About Headless Client
----------------------
> Headless Client optimize +80% of arma3server.exe. He takes actually 100% of MySQL request and 80% of ServerSide's scripts.

How to install it
----------------------
> Put in your config.cfg
headlessClients[] = {IP¨of headless}; for exemple if you have your headless in the same computer  : headlessClients[] = {127.0.0.1};

> life_hc.pbo need to be signed if verifysignature=2 !!!

> My Start-HC.bat :

```
@echo off
::timeout 20
:: Modify your folders etc!
set armapath="D:\SteamGames\steamapps\common\Arma 3"
set armaparams=-client -connect=127.0.0.1 -port=2302 -password=dev -name=HC -profiles=HC -mod=@extDB2;@life_hc;
set serverexe=arma3.exe
echo.
echo Restarting
:: start the servers..
cd /d %armapath%
start "" %serverexe% %armaparams%
exit
```
<br/>

---------------------------

[How to configure your server] (https://github.com/ArmaLife/Altis/wiki/Setup-Server)
-------------------------------------
You can found all the steps to have a fully working server in our [github wiki] (https://github.com/ArmaLife/Altis/wiki).

Disclaimer
-----------
>   The vast majority of the code / framework has been written by Tonic.

>   Any additional code / content used is fully credited and owned by it’s author as well as linked to the authors content (Forums,Media,etc).

>   The additional content used within the framework either has the expressed permission of the content creators permission or was automatically used under the GPL (General Public License) from public posting with no usage / TOA / Disclaimer, however they still own the rights to their content.

>   If in any case that content is being used within this mission / framework that the content creator doesn’t wish for it to be used due to my strict TOA / Agreement all you need to do is ask for it to be removed and it will be honored.
<br/>

Usage / Terms of agreement
---------------------------
>   The branding of the mission is to stay ‘XXX Life RPG’. This means you cannot modify it to say something else. i.e Atlis Life by YOURCOMMUNITYNAME/TAG. Everything about the naming / branding is to be left untouched.

>   Naturally all credit is to remain intact on all files. Author cannot be modified via Description.ext but can be extended in briefing.sqf

>   All of my code is not to be used outside of the mission in another ‘Life’ like mission. It is to stay the Life HC RPG Framework / my framework or you don’t use it and direct branding.

>   Some of my code can be used outside of the mission / framework but permission is to be asked first, if no response is received then it is a automatic NO.

>   Core configuration is allowed to be modified (i.e Prices and expansion of items / features).

>   Life-HC RPG Framework is only allowed to be used with the Arma 3 vanilla maps with no extensions or mods (with the exception of server sided mods, and direct permission from author).

>   All edits made inside the framework is fine as long as it stays in the vanilla maps that Bohemia Interactive has released, past, present and future.

>   Features added by you to the mission are to stay to your modification in your server, distribution is not allowed without my permission, if you would like your feature to be added to the Life HC RPG main distribution (by me) you can submit your changes and will be fully credited.

>   This is not be used commercially and is to remain freeware, this includes requiring donations / payment to be able to ‘play’ in your server with this mission. Playability of it is to remain free and open.
