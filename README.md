# Intro till screenscraping

###Länkar du behöver i dag

- Länk till den här sidan: http://bit.ly/sjf-scraping
- [Chrome Scraper-pluginet](https://chrome.google.com/webstore/detail/scraper/mbigbapnjcgaffohmbkdlecaccepngjd)
- [Svenska riksdagsledamöter](http://www.riksdagen.se/sv/ledamoter-partier/Hitta-ledamot/Bokstavsordning/)

###Tutorials på nätet

- https://dataist.wordpress.com/2012/10/12/get-started-with-screenscraping-using-google-chromes-scraper-extension/
- http://schoolofdata.org/handbook/recipes/scraper-extension-for-chrome/

###Övning

Exempelsida: http://jensfinnas.github.io/150922-screen-scraping-workshop

- Hämta alla rubriker: `//h3`
- Hämta alla länkar: `//a`
- Hämta alla kursiverade ord: `//i`
- Hämta alla kursiverade ord med klassen "name": `//i[@class="name"]`
- Hämta det första kursiverade ordet med klassen "name": `//i[@class="name"][1]`

__Bonusövningar:__ 

- Vem har flest bilder på sin startsida: Aftonbladet eller Expressen?
- Vem har flest länkar?
- Vem har flest länkar som innehåller ordet "chock"?

### XPath-grunder

Uttryck|Vad det gör
--- | ---
`//`|Sök igenom hela dokumentet
`//div[2]`|Hämta den n:te taggen
`//div[2]/table[1]/tr[3]`|Hämta den n:te taggen, inuti den n:te taggen, inuti...
`//div[@class="class-name"]`|Hämta tag med klassen "class-name" 
`//div[@id="download"]`|...eller ett annat attribut
`//div/text()`|Hämta textinnehållet i en tagg
`//a/@href`|Hämta ett visst attribut, i det här fallet en länks url
`//div[contains(., "sökord")]`|Hämta alla div-taggar som innehåller ett visst sökord


### Andra scraping-verktyg och länkar

- [Kimono](https://www.kimonolabs.com/)
- [Import.io](https://import.io/)
- [Amerikanska exempel på scrapingbaserad journalistik](https://github.com/amandabee/scraping-for-journalists/blob/master/examples.md)
