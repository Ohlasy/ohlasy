# Vkládání fotografií

Při vkládání článků je úplně jedno, ke je fotografie uložená, jen to musí být někde veřejně a musíte od ní mít URL (adresu). K tomu výborně poslouží například server [imgur](http://imgur.com), kam můžete po registraci nahrát libovolný počet fotek zdarma a dostanete jejich URL.

Když se přihlásím na imgur a najedu myší na své uživatelské jméno vpravo nahoře, objeví se menu:

![screenshot](http://i.imgur.com/tLPbCee.png)

Vyberu položku *images* (obrázky) a dostanu se na přehled všech svých obrázků. Tam už pak můžete novou fotku nahrát snadno tak, že ji do okna prohlížeče přetáhnete myší. (Nebo klikněte na tlačítko *Computer* a objeví se dialog pro výběr souboru.)

Jakmile je fotka úspěšně nahraná, objeví se ve vašem seznamu fotek. Když na ni pak kliknete, zobrazí se její detail a seznam odkazů:

![screenshot](http://i.imgur.com/z8ciVH4.png)

Nejdůležitější je ten odkaz označený zeleně, to je URL obrázku v plné velikosti. (Schválně si ho zkuste zkopírovat do schránky a vložit do adresního řádku prohlížeče, otevře se vám obrázek v plné velikosti.)

Plná velikost obrázku je ale hodně velká, takže například na titulce webu musíme použít menší verzi. Její URL dostaneme snadno tak, že v obrazovce s přehledem odkazů klepneme dole v menu *Sizes* (velikosti) na možnost *Large Thumbnail* (velký náhled). Kýžené URL je opět v políčku *Direct Link* (přímý odkaz).

Pokud si ale porovnáte URL plného obrázku a náhledu, zjistíte, že jsou úplně stejné, jen URL náhledu má na konci názvu malé písmeno L navíc. Takže si můžete zjednodušit práci a URL náhledu vyrobit ručně, prostě přidáte `l`.

Nic dalšího není potřeba dělat. Jednou za čas spouštíme [skript pro migraci obrázků](https://github.com/zoul/demiurge), který námi používané obrázky postahuje z imgur a nahraje je na náš server.