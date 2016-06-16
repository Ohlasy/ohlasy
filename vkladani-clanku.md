# Vkládání článků

Každý článek je textový soubor v adresáři [_posts](https://github.com/Ohlasy/web/tree/gh-pages/_posts). Struktura tohoto adresáře může být libovolná, my jsme zvolili rozdělení podle let a měsíců. Článek má dvě hlavní části: samotný text ve formátu [Markdown](https://github.com/Ohlasy/redakce/blob/master/markdown.md) a metadata, tedy informace o článku (autor, rubrika a podobně).

## Metadata

Informace o článku jsou uložené především v záhlaví každého souboru, například takhle:

    ---
    title: „Člověk dokáže i trapno využít ve svůj prospěch.“
    cover-photo: http://i.imgur.com/eYUFoYtl.jpg
    author: Martina Vašková
    category: rozhovory
    tags: kultura, divadlo
    ---

Tímto záhlavím začíná každý článek. Jeho formát je jednoduchý: nejprve tři pomlčky (přesněji řečeno spojovníky) jako oddělovač, pak několik řádků ve tvaru `magické-klíčové-slovo: nějaká hodnota`, a nakonec zase tři spojovníky jako oddělovač.

### Titulek článku

Titulek se nastavuje klíčovým slovem `title`. Skrývá se tady jen jeden čert: Pokud titulek obsahuje dvojtečku, je nutné celý text titulku uzavřít do rovných uvozovek (`"`), aby dvojtečka nezmátla mašinu.

A vlastně ještě jeden čert tu je: Pokud je článek v rubrice *názory a komentáře*, nedávejte do titulku jméno autora, vloží se tam automaticky.

### Titulní fotka

Nastavuje se klíčovým slovem `cover-photo`, hodnotou je URL fotky. K nahrávání fotek [podrobněji samostatný dokument](https://github.com/Ohlasy/redakce/blob/master/vkladani-fotografii.md). Nezapomeňte na to, že titulní fotka nesmí být v plném rozlišení, jinak by se nám na titulce webu sešly desítky megabajtů dat!

### Autor

Nastavuje se klíčovým slovem `author`. Hodnota musí být něco ze [seznamu autorů](https://github.com/Ohlasy/web/blob/gh-pages/_data/autori.yml), jinak by se nenačetla profilovka autora a jeho e-mail.

### Rubrika

Nastavuje se klíčovým slovem `category`. Možné hodnoty jsou `rozhovory`, `názory a komentáře`, `zpravodajství`, `ankety` a `seriály`. Podle rubriky se momentálně pod každým článkem sází seznam dalších článků.

### Témata

Nastavují se klíčovým slovem `tags`, hodnotou je seznam témat oddělených čárkami. K seznamu témat je [stručný návod na Trellu](https://trello.com/c/wzHWMyxX/364-temata), ale celá věc je zatím v plenkách.

### Seriály

Pokud je článek součástí seriálu, mezi ostatní články ze seriálu ho zařadíte klíčovým slovem `serial`. Možné hodnoty jsou `stromy`, `depozitar`, `jazyk`, `krajiny` a `historie`, viz [seznam seriálů ve zdrojovém kódu webu](https://github.com/Ohlasy/web/tree/gh-pages/_includes/serials).

## Text článku

Pro formátování článků používáme jazyk [Markdown](https://github.com/Ohlasy/redakce/blob/master/markdown.md). Jediné, co stojí za další zmínku, je vkládání obrázků. To vypadá takhle:

    <img src="http://i.imgur.com/eYUFoYt.jpg"
        alt="Jenda Nádvorník, Michaela Vymazalová"
        class="img-responsive img-popup"
        data-author="Tomáš Znamenáček">

Do uvozovek za `src` patří URL obrázku. Atribut `alt` určuje textový popisek obrázku, který potřebují například hlasové čtečky pro nevidomé. Atribut `class` je vždycky stejný, atribut `data-author` určuje zdroj obrázku.

Pokud si nejste jisti, jak co zařídit, podívejte se na předchozí články v podobném stylu, máme jich mraky.