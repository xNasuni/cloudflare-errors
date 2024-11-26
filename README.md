# cloudflare-errors
repository containing cloudflare error pages for archival purposes (or if you want to make fake pages)<br>
<img src="https://github.com/user-attachments/assets/c1abc679-0d1a-4c14-aaed-9391511a30c9" width="710px" />


### current list (feel free to pr more that you find)

[`error code  520` "Web server is returning an unknown error"](index520.html)<br>
[`error code  522` "Connection timed out"](index522.html)<br>
[`error code 1000` "DNS points to prohibited IP"](index1000.html)<br>
---
[`id ray generator preview`](rayid.html)

### generating fake ray ids
```js
const base = ((((new Date().getTime()/1000 + 657696208)).toString(16)).replace(".", ""))
const extra = Math.random().toString(16).substring(2, 2 + (16 - base.length))
return base + extra
```
> cloudflare's ray id's aren't actually fully random, and they are actually a timestamp, this can generate something that sort of looks like them but it's just meant to look real, not actually functional
> 
> i.e. "8e78f376c4dd324d"

### possible cloudflare server region names

```
Ad Dawhah
Al 'Asimah
Al Basrah
Al Qahirah
Alaska
Alberta
Alger
Almaty
Amazonas
An Najaf
Annaba
Antananarivo
Antioquia
Ar Riyad
Arbil
Arica y Parinacota
Arizona
Ash Sharqiyah
Astara
Asuncion
Attiki
Auckland
Australian Capital Territory
Auvergne-Rhone-Alpes
Baden-Wurttemberg
Baghdad
Bagmati
Bahia
Baki
Bali
Bayern
Beograd
Berlin
Beyrouth
Bihar
Biobio
Bratislavsky kraj
British Columbia
Brunei-Muara
Brussels Hoofdstedelijk Gewest
Bucuresti
Budapest
California
Canterbury
Casablanca-Settat
Catalunya
Ceara
Cebu
Centar
Central
Chandigarh
Chattogram
Chiang Mai
Chisinau
Ciudad Autonoma de Buenos Aires
Ciudad de Mexico
Colorado
Cordoba
Cork
Curacao
Dakar
Dar es Salaam
Delhi
Demerara-Mahaica
Dhaka
Distrito Capital de Bogota
Distrito Federal
Distrito Nacional (Santo Domingo)
Djibouti
Dubayy
Dublin
England
Erevan
Esch-sur-Alzette
Espirito Santo
Florida
Francisco Morazan
Fukuoka
Gauteng
Geneve
Georgia
Goias
Grad Zagreb
Greater Accra
Guatemala
Guayas
Gujarat
Ha Noi
Hagatna
Hamburg
Harare
Harjumaa
Hawaii
Hefa
Hessen
Ho Chi Minh
Hofudborgarsvaedi
Hong Kong
Hovedstaden
Ile-de-France
Illinois
Indiana
Islamabad
Istanbul
Izmir
Jakarta Raya
Jalisco
Johor
Kadiogo
Kaohsiung
Karbala'
Karnataka
Kentriki Makedonia
Kerala
Khabarovskiy kray
Khulna
Kingston
Kinshasa
Krasnoyarskiy kray
Krung Thep Maha Nakhon
Kwazulu-Natal
Kyiv
La Paz
Lagos
Lazio
Lefkosia
Lima
Lisboa
Littoral
Lombardia
Luanda
Luxembourg
Macao
Madrid, Comunidad de
Maharashtra
Maine
Makkah al Mukarramah
Male
Mandalay
Manitoba
Maputo
Masqat
Massachusetts
Mato Grosso
Mazowieckie
Michigan
Minas Gerais
Minnesota
Minskaya voblasts'
Misamis Oriental
Missouri
Mombasa
Montserrado
Moskva
Nairobi City
National Capital Region
Nebraska
Neuquen
Nevada
New Jersey
New Mexico
New South Wales
New York
Noord-Holland
Nordrhein-Westfalen
North Carolina
Nouvelle-Aquitaine
Nova Scotia
Odisha
Ohio
Okinawa
Oklahoma
Ontario
Oran
Oregon
Osaka
Oslo
Ouest
Panama
Para
Paramaribo
Parana
Pennsylvania
Pernambuco
Phnom Penh
Pichincha
Port Louis
Praha, Hlavni mesto
Provence-Alpes-Cote-d'Azur
Province Sud
Punjab
Quebec
Queensland
Queretaro
Ramallah
Region Metropolitana de Santiago
Reunion
Riga
Rio Grande do Sul
Rio de Janeiro
Saint George
Saint Michael
San Jose
Sankt-Peterburg
Santa Catarina
Santiago
Sao Paulo
Saskatchewan
Scotland
Seoul-teukbyeolsi
Sicilia
Sindh
Singapore
Sofia (stolitsa)
South Australia
South Dakota
South East
Stockholms lan
Surat Thani
Sverdlovskaya oblast'
Taipei
Tamil Nadu
Tasmania
Tbilisi
Tel Aviv
Telangana
Tennessee
Texas
Thimphu
Tirane
Tokyo
Toshkent
Tunis
Tverskaya oblast'
Ulaanbaatar
Utah
Uttar Pradesh
Uusimaa
Vastra Gotalands lan
Viangchan
Victoria
Ville de Kigali
Vilniaus apskritis
Virginia
Washington
West Bengal
Western Australia
Western Cape
Western Province
Wien
Wilayah Persekutuan Kuala Lumpur
Yangon
Yogyakarta
Zurich
```