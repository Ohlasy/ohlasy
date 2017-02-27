Pro předplatné se nám hodí mít přesnější statistiky – především vědět, kdo odkud přišel.
Například který post na Facebooku byl úspěšný, jestli čtenáři klikají na naše bannery na
webu a podobně. Abychom tahle data dostali, musíme při odkazování na web předplatného
k běžnému URL (predplatne.ohlasy.info) přidat ještě několik parametrů.

Google má [speciální nástroj](https://ga-dev-tools.appspot.com/campaign-url-builder/), ve
kterém se tyhle parametry dají pohodlně vyplnit. Zadáte základní URL (predplatne.ohlasy.info)
plus parametry pro sledování kampaně a vypadne vám delší URL, na které pak můžete poslat
čtenáře. (Zbytečně to URL neotvírejte sami, zkreslili byste statistiky.)

Parametry, které se dají nastavit:

* _Website URL_ je základní URL, tedy http://predplatne.ohlasy.info.
* _Campaign Source_ je zdroj, ze kterého čtenář přišel. Takže pokud děláte odkaz pro použití
na Facebooku, napište `facebook`, pokud chcete vyrobit odkaz na propagaci mailem, napište `mail`.
V principu sem můžete napsat cokoliv, je to prostě jen identifikátor pro naše potřeby.
* _Campaign Medium_ je podrobnější určení zdroje. Například na Facebooku můžete rozlišit
běžný post a nákupní tlačítko. Když jde o facebookový post, píšu `post`.
* _Campaign Name_ je název kampaně, používáme prostě `predplatne`.
* _Campaign Content_ je další pole pro rozlišení zdroje. Například u Facebooku sem můžete
vložit krátký identifikátor postu, abychom věděli, přes který post čtenáři přišli.

Konkrétní příklad: _Campaign Source_ `facebook`, _Campaign Medium_ `post`, _Campaign Content_
`rozhovor_mazal`.

Výsledné URL je hodně dlouhé. Pokud bude vidět, je lepší ho zkrátit pomocí [goo.gl](https://goo.gl).
