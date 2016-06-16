# Markdown

Všechny články Ohlasů jsou značkované pomocí jazyka Markdown. Ten řeší jeden prastarý problém: jak do textu zanést významové nebo formátovací značky, například *kurzívu*. Pro značkování textu vznikla řada jazyků, například v HTML by se kurzíva označila pomocí značky `<i>`:

    Takto vypadá <i>kurzíva</i>.

Jenže to je pro běžné psaní dost nepohodlné. Proto vznikl jazyk Markdown, který se snaží značkování textu zařídit co možná nejpřirozenějším způsobem, i když je to na úkor jeho možností. (Jinými slovy: Markdown je bastl, ale pohodlný.)

## Základní značkování

*Kurzívu* nebo jiný základní důraz vytvoříte prostě tak, že danou část textu \*uzavřete do hvězdiček\* nebo \_podtržítek\_. **Tučný** řez vyrobíte \*\*dvěma hvězdičkami\*\*. Pokud potřebujete použít hvězdičku v jejím běžném, nespeciálním významu (například 2\*3), vložte před ni zpětné lomítko (`\*`).

Odkaz vyrobíte tak, že klikací část uzavřete do hranatých závorek a těsně za ně uvedete do kulatých závorek URL:

    Viz [náš předchozí text na toto téma](http://ohlasy.info/clanky/2016/06/rozhovor-impro.html).

Pokud odkazujete na články v rámci Ohlasů, můžeme použít takzvané relativní URL:

    Viz [náš předchozí text na toto téma](/clanky/2016/06/rozhovor-impro.html).

Odstavce jsou nejjednodušší, stačí za každým odstavcem udělat volný řádek.

## Seznamy

Číslovaný nebo odrážkovaný seznam vytvoříme jednoduše tím, že každý bod uvedeme číslicí nebo odrážkou:

    1. Jedna
    2. Dva
    3. Tři

Odrážka může být hvězdička nebo pomlčka:

    - Jedna
    - Dvě
    - Tři

Tady číhá nepříjemný detail: Pokud odstavec přirozeně začíná číslem a tečkou (například: „1. dubna se tam a tam bude dít to a to“), Markdown ho považuje za část seznamu. Opět se to dá řešit lomítkem: `1\. dubna se…`. Lomítko ve výsledném dokumentu zmizí a datum zůstane datem.

## Tvrdé konce řádků

Potřebujete-li vyrobit explicitní konec řádku, například kvůli sazbě poezie, můžete na konec řádku přidat dvě mezery, tady naznačené podtržítkem, abyste je viděli:

    ÚPLNĚK STOUPÁ__
    nad krajem.__
    Jak čerstvě__
    přeříznutý__
    kmen.

Kdybyste to neudělali, Markdown by řádky spojil dohromady do jednoho odstavce.