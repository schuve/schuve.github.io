<h4>VM config</h4>
<p>SRV: 8-6-4GB RAM, 60GB STR, 1J 4V, NAT8, OS later</p>
<p>WIN: 8-6-4GB RAM, 60GB STR, 1J 4V, NAT8, OS later</p>
<p>LNX: 4GB RAM, 30GB STR, 1J 4V, NAT8, OS later</p>
------------------------------------------------------------------------------------------------------------------
<h4>DNS</h4>
<h4>AD</h4>
<p>New Forest (local.lab), DSRM (zdt ps), DNS delegace -> když sub dom (sub.loacl.lab)</p>
<h4>DHCP</h4>
<p>scope...DNS, GW</p>
<h4>AD create</h4>
<p>pray</p>
<h4>IIS-FTP</h4>
<p>AKTIVNÍ REŽIM - v advancet u WinSCP vypnout :)</p>
------------------------------------------------------------------------------------------------------------------
<h4>SAMBA</h4>
<p>
/etc/samba/smb.conf <--- konfig on end, 
samba user create, 
smbd, nmbd,  
\\ip\\share 
</p>
<h4>RMT-HELP</h4>
<p>SSH sudo apt install ssh</p>
<p>VNC W(tightvnc) -> L(x11vnc)</p>
<p>RDP L(Remmina) -> W(ON)</p>
<p>Remmina i pro vnc, i think so <3</p>
------------------------------------------------------------------------------------------------------------------
<h4>conf</h4>
<p>PCPartPicker.com, PassMark, Geekbench, geekboy cz, GPUreport cz, forum zive cz sestavy </p>
<p>srv: smicro.cz</p>
<h4>zanetování</h4>
<p>prvky: RACK, Router (GW), SW (Poe, NEPoE), Patchpanel (konektory Optika/RJ45), AP, UPS, NAS</p>
<p>značky: ubiquity</p>
------------------------------------------------------------------------------------------------------------------
<p>17: https://freshmangojuice.github.io/ ----- https://maturitaop.github.io/</p>
------------------------------------------------------------------------------------------------------------------
<h2>IT vybavení</h2>
<table>
    <tr>
        <th>KOMPONENTA</th>
        <th>CENA</th>
    </tr>
    <tr><td>Router - Ubiquiti EdgeRouter ER-6P, PoE</td><td>5 059 Kč</td></tr>
    <tr><td>Switch - Ubiiquiti USW-24-POE Gen2</td><td>9 590 Kč</td></tr>
    <tr><td>AP - Ubiquiti U7-Pro-XG</td><td>4 989 Kč</td></tr>
    <tr><td>UPC - CyberPower CP2000EIPFCRM2U</td><td>10 790 Kč</td></tr>
    <tr><td>Barevná tiskárna - HP ColorJet Pro MFP 3302fdw</td><td>8 899 Kč</td></tr>
    <tr><td>Černobílá tiskárna - HP LaserJet Enterprise MFP M528dn</td><td>43 223 Kč</td></tr>
    <tr><td>HP Z2 Mini G1i</td><td>33 790 Kč</td></tr>
    <tr><td>Monitor - DELL Pro 27 Plus (P2725D)</td><td>5 999 Kč</td></tr>
    <tr><td>Microsoft 365 Business Standard (rok)</td><td>3 990 Kč</td></tr>
</table>

<h2>PC sestava</h2>
<table>
    <tr>
        <th>KOMPONENTA</th>
        <th>CENA</th>
    </tr>
    <tr><td>AMD Ryzen 9 9950X3D</td><td>14 690 Kč</td></tr>
    <tr><td>ARCTIC Liquid Freezer III 360 Pro Black</td><td>2 499 Kč</td></tr>
    <tr><td>ASROCK X870 PRO RS</td><td>4 999 Kč</td></tr>
    <tr><td>GIGABYTE GeForce RTX 5070 Ti EAGLE OC SFF 16G</td><td>24 990 Kč</td></tr>
    <tr><td>Kingston FURY 32GB DDR5 6000MT/s CL30</td><td>10 890 Kč</td></tr>
    <tr><td>Samsung 990 PRO 2TB</td><td>5 199 Kč</td></tr>
    <tr><td>Montech X5 Black</td><td>1 459 Kč</td></tr>
    <tr><td>Seasonic Focus GX-1000 ATX 3.1</td><td>4 499 Kč</td></tr>
    <tr><td>27" DELL U2724DE UltraSharp</td><td>12 790 Kč</td></tr>
    <tr><td>Logitech G213</td><td>1 299 Kč</td></tr>
    <tr><td>Logitech G502 Hero</td><td>1 199 Kč</td></tr>
    <tr>
        <td><strong>Celkem</strong></td>
        <td><strong>84 513 Kč</strong></td>
    </tr>
</table>

Návrh hardwaru
------------------------------------------------------------------------------------------------------------------

Sklep: Multimediální dílna a jádro
PC1 (Studio): Zaměřeno na ticho a výpočetní výkon pro audio.

CPU: AMD Ryzen 7 7700 (vysoký výkon, nízké teploty).

RAM: 32GB DDR5 (pro náročné pluginy a samply).

Audio: Externí zvuková karta (např. Focusrite Scarlett 4i4) – interní karty jsou dnes kvůli rušení v PC pasé.

Periferie: Multifunkční tiskárna (např. Brother MFC-L2712DN – nezmar).

NAS: Synology DiskStation DS224+ + 2x 4TB WD Red Plus (RAID 1 pro zrcadlení dat). Centrální úložiště pro nahrávky i zálohy programátora.

Přízemí: Pracovna programátora
PC2 (Profi): Priorita je multitasking a spolehlivost.

CPU: Intel Core i7-14700 (skvělé pro kompilaci kódu).

RAM: 64GB DDR5 (Docker, virtuální stroje, 100 tabů v prohlížeči).

Zobrazení: 2x 27" 4K Dell UltraSharp (pivot pro kódování).

TV: 55" LG OLED (skvělá konektivita, AirPlay/Chromecast).

1. Patro: Domácí PC a hry
PC3 a PC4 (Univerzál): Vyvážený poměr cena/výkon.

CPU: AMD Ryzen 5 7600.

GPU: NVIDIA RTX 4060 (perfektní pro 1080p/1440p hraní).

RAM: 16GB DDR5.

Síťová infrastruktura
VDSL Modem/Router: AVM FRITZ!Box 7530 AX (špička pro VDSL linky).

Switch: 8-portový Gigabit switch (TP-Link TL-SG108) umístěný v technickém centru.

Wi-Fi: Mesh systém (např. TP-Link Deco X50, 3 jednotky) pro pokrytí všech pater bez výpadků.

Návrh softwaru a nastavení
------------------------------------------------------------------------------------------------------------------

Operační systémy
PC1 & PC2: Windows 11 Pro (kvůli vzdálené ploše a BitLockeru). PC2 může mít Dual Boot s Linuxem (Ubuntu/Fedora) podle preferencí programátora.

PC3 & PC4: Windows 11 Home.

Síť a NAS
Statické IP adresy: NAS, tiskárna a TV budou mít v routeru rezervované pevné IP adresy (pro snadný přístup).

Sdílení dat: Na NASu vytvoříme síťové disky (SMB):

\\NAS\Studio (přístup pro PC1).

\\NAS\Backup (pro zálohování všech PC přes aplikaci Synology Drive).

\\NAS\Media (pro filmy a hudbu v TV přes DLNA/Plex).

Zabezpečení: Firewall na routeru, WPA3 šifrování na Wi-Fi, na NASu nastavený automatický "Snapshot" proti Ransomware.

Blokové schéma síťového propojení
------------------------------------------------------------------------------------------------------------------

Textový popis zapojení:

Vstup: Telefonní linka -> VDSL Modem (Sklep/Přízemí).

Páteř: Z modemu vede kabel do Switche.

Větve ze Switche:

Kabel -> NAS (Sklep)

Kabel -> PC1 (Sklep)

Kabel -> PC2 (Pracovna)

Kabel -> TV (Přízemí)

Kabel -> Mesh Jednotky (Rozmístěny v patrech jako "backhaul" pro nejrychlejší Wi-Fi).

Bezdrát: PC3 a PC4 se připojují přes Wi-Fi (nebo kabelem do nejbližší Mesh jednotky).

