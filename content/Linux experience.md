#IT #Linux

> Setting ที่เคยปรับไว้ แล้วอาจจะลืม
	> ~~set repeat rate @2000 แก้ terraria input lag ~~ปรับกลับละ [Source](https://forums.terraria.org/index.php?threads/horrible-input-lag-on-tmodloader-ubuntu.103104/)
	> 
# Install & Setup
- Pop!_ OS เอา iso มาลงผ่าน etcher 
- Bios to [[Legacy mode]] instead of UEFI *เพราะคอมเก่าเกิ้น ลง UEFI แล้ว fail 100%*
## First things to do
1. Update & Upgrade `sudo apt update` (optional: change mirror for download speed)
2. Install nvidia driver if needed
3. 


### Language Switching
#### Current setup 2022
- just use CAPLOCK to change language; fast and no delay switching
#### Outdated
- มันจะมี delay ตอน switch เป็น prompt ขึ้นมาหน้าตาแบบนี้ถ้าใช้ grave accent
	![[Pasted image 20211206111807.png|200]]
- ให้ run script ![[graveAccentChangeLanguageScript.sh]]
- ถ้า work ก็ผูก script ไว้กับปุ่ม grave accent ด้วย custom keyboard shortcut (command: whatever the path to file is)
- Sources: https://askubuntu.com/questions/1348051/how-do-i-change-input-language-without-having-to-confirm-it



### Others
- navigating foldername with "space" ใช้ tab autocomplete ของ terminal เลย

# Apps
ลงได้หลายแบบมากๆ
- appimage โหลดมา คลิกขวา set ให้ executable -> run ได้เลย
	- useful software: https://github.com/TheAssassin/AppImageLauncher ช่วยให้เหมือน install appimage ได้เลย (register in applications)
- .deb มีตัวลงให้ง่ายสุด
- flatpak, snap เป็น platform app ใช้ได้เหมือนกัน

| Windows | Linux solution|
| --- | --- |
| Zoom| ✅ |
| Word| ✅ ใช้ libreoffice พอได้ กับ word online|
| Line | ~~WINE พอได้ ตั้ง compat เป็น windows 10~~ ไม่ work แล้วอ่ะ 😭|
| ShareX | Ksnip(manual add to startup), Flameshot |
|  |  |

## Line 
- ~~download installer https://desktop.line-scdn.net/win/new/LineInst.exe
	- ใช้ link นี้แทน https://desktop.line-scdn.net/win/legacy/win7or8/LineInst.exe เพราะมันจะไม่ error win7/8 not supported ใช้ได้เหมือนกัน
- Issues
	- High CPU usage

## Jdownloader2
- install by snap (ไม่รู้ install .sh ให้มันได้ยังไง 555 กด execute แล้วมันเข้า text editor)
- very good at capturing multi-part links download
- set max chunk high and max simultaneous cuz combine speed is better than one fast download

## XDM
- very very fast

## APK extractor
- APK editor studio สามารถเอา icon ออกจาก apk ได้

# Gaming
many ways to play
1. Native ✅
2. Steam proton experimental
3. Lutris
4. Wine

Helpers
- ProtonUp-QT from github ใช้ manage ทุกอย่างเกี่ยวกับ wine/proton ใน steam/lutris 

### Current limitations
- cannot play repack like steam games from fit-girl

### LOL ⭐⭐⭐
- see reddit guide for garena, unreliable but at least no crash during play (need confirmation)
### POE
- ใช้ Steam proton experimental ไปเลย
- Launch option: gamemoderun DXVK_STATE_CACHE=0 %command% --waitforpreload --noasync --nodx9ex --gc2 --nologo
- In game: low setting all นอกนั้นเปลี่ยนแล้ว +/- ลองได้
- Issues
	- Lag and stutter like hell in maps ยังไม่ได้ลอง  proton-ge อาจจะ improve fps ???

### Battlerite
- Steam proton: crash @#$% everytime in multiplayer
- sometimes doesn't even launch

### Wizardry 8
- WINE
- perfect with some number display glitch

### Mutants zero-road to eden
- download from gogs-game
- use lutris gog installer instead of double click
- Profit
- Issues
	- crash every now and then randomly so save every 2-3 minutes

### Sekiro 💪
- download from igg-games (https://igg-games.com/pc-sekiro-443921769-shadows-die-twice-free-download.html) จะมาเป็น folder เลย ไม่ต้องทำอะไร เปิด exe ผ่าน lutris
- ใน lutris ให้ใช้ WINE-GE จาก github

## Wakfu/Dofus
- ง่ายมาก ankama launcher โหลดเป็น appimage มา run เลย แต่ก็ลงเป็น application ไม่ได้ :/

# Theme
- gnome look : nordic theme 

# Misc
- interesting desktop customize: https://ubuntubudgie.org (not yet tried)

# Issues and solutions
- official PPAs เวลาลง program แล้วขึ้นว่า not publicly signed
	- ใช้ command นี้เลย
		``` sudo apt-key adv --recv-keys --keyserver keyserver.ubuntu.com `sudo apt-get update 2>&1 | grep -o '[0-9A-Z]\{16\}$' | xargs` ```
	- แล้วก็ ``` sudo apt update ``` ตามปกติ