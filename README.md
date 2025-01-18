# cloudflare-errors
repository containing cloudflare error pages for archival purposes (or if you want to make fake pages)<br>
<img src="https://github.com/user-attachments/assets/c1abc679-0d1a-4c14-aaed-9391511a30c9" width="710px" />


### current list (feel free to pr more that you find)

[`security blocks` "Sorry, you have been blocked"](indexblocked.html)<br>
[`phishing blocks` "Suspected Phishing"](indexphishing.html)<br>
[`error code  502` "Bad gateway"](index502.html)<br>
[`error code  520` "Web server is returning an unknown error"](index520.html)<br>
[`error code  522` "Connection timed out"](index522.html)<br>
[`error code  525` "SSL handshake failed"](index525.html)<br>
[`error code 1000` "DNS points to prohibited IP"](index1000.html)<br>
[`error code 1003` "Direct IP access not allowed"](index1003.html)<br>
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
Abidjan
Accra
Adelaide
Ahmedabad
Albuquerque
Algiers
Almaty
Americana
Amman
Amsterdam
Anchorage
Annaba
Antananarivo
Aracatuba
Arica
Ashburn
Astara
Asuncion
Athens
Atlanta
Auckland
Austin
Baghdad
Baku
Bandar Seri Begawan
Bangkok
Bangor
Barcelona
Barranquilla
Basra
Beihai
Beijing
Beirut
Belgrade
Belo Horizonte
Belém
Bengaluru
Berlin
Bhubaneshwar
Blumenau
Bogota
Bordeaux
Boston
Brasília
Bratislava
Bridgetown
Brisbane
Brussels
Bucharest
Budapest
Buenos Aires
Buffalo
Cagayan
Cairo
Calgary
Campinas
Campos dos Goytacazes
Canberra
Cape Town
Casablanca
Caçador
Cebu
Chandigarh
Changde
Changsha
Changzhou
Chapeco
Charlotte
Chengmai
Chennai
Chiang Mai
Chicago
Chittagong
Chongqing
Christchurch
Cleveland
Colombo
Columbus
Concepción
Copenhagen
Cordoba
Cork
Cuiabá
Curitiba
Da Nang
Dakar
Dalian
Dallas
Dammam
Dar Es Salaam
Denpasar
Denver
Detroit
Dhaka
Djibouti
Doha
Dubai
Dublin
Durban
Düsseldorf
Edinburgh
Ekaterinburg
Entebbe
Erbil
Florianópolis
Fortaleza
Foshan
Frankfurt
Fukuoka
Fuzhou
Gaborone
Geneva
Georgetown
Goiânia
Gothenburg
Guadalajara
Guam
Guangzhou
Guatemala City
Guayaquil
Guiyang
Haifa
Haikou
Halifax
Hamburg
Hanoi
Harare
Helsinki
Hengshui
Ho Chi Minh City
Hobart
Hong Kong*
Honolulu
Houston
Huainan
Hyderabad
Indianapolis
Islamabad
Istanbul
Itajaí
Izmir
Jacksonville
Jakarta
Jashore
Jeddah
Jinan
Johannesburg
Johor Bahru
Joinville
Juazeiro do Norte
Kannur
Kanpur
Kansas City
Kaohsiung City
Karachi
Kathmandu
Khabarovsk
Kigali
Kingston
Kinshasa
Kochi
Kolkata
Krasnoyarsk
Kuala Lumpur
Kunming
Kuwait City
Kyiv
La Paz
Lagos
Lahore
Langfang
Lanzhou
Las Vegas
Lima
Lisbon
London
Los Angeles
Luanda
Luxembourg City
Lyon
Macau
Madrid
Male
Manama
Manaus
Manchester
Mandalay
Manila
Maputo
Marseille
McAllen
Medellín
Melbourne
Memphis
Mexico City
Miami
Milan
Minneapolis
Minsk
Mombasa
Montgomery
Montréal
Moscow
Mumbai
Munich
Muscat
Nagpur
Naha
Nairobi
Najaf
Nanchang
Nashville
Nasiriyah
Neuquen
New Delhi
Newark
Nicosia
Norfolk
Nouméa
Oklahoma City
Omaha
Oran
Osaka
Oslo
Ottawa
Ouagadougou
Palermo
Palmas
Panama City
Paramaribo
Paris
Patna
Perth
Philadelphia
Phnom Penh
Phoenix
Pittsburgh
Port Louis
Port of Spain
Portland
Porto Alegre
Prague
Qingdao
Queretaro
Quito
Raleigh
Ramallah
Recife
Reykjavík
Ribeirão Preto
Richmond
Riga
Rio de Janeiro
Riyadh
Rome
Sacramento
Saint-Denis
Salt Lake City
Salvador
San Antonio
San Diego
San Francisco
San Jose
San José
San Juan
Santiago
Santiago de los Caballeros
Santo Domingo
Saskatoon
Seattle
Seoul
Shanghai
Shaoxing
Shenzhen
Singapore
Sioux Falls
Skopje
Sofia
Sorocaba
St. George's
St. Louis
St. Petersburg
Stockholm
Stuttgart
Sulaymaniyah
Surat Thani
Suva
Sydney
São José do Rio Preto
São José dos Campos
São Paulo
Tahiti
Taipei*
Taizhou
Tallahassee
Tallinn
Tampa
Tarlac City
Tashkent
Tbilisi
Tegucigalpa
Tel Aviv
Thessaloniki
Thimphu
Tianjin
Timbo
Tirana
Tokyo
Toronto
Tunis
Tver
Uberlândia
Ulaanbaatar
Valparaíso
Vancouver
Vienna
Vientiane
Vilnius
Vitoria
Warsaw
Willemstad
Winnipeg
Wuhu
Xianyang
Yamoussoukro
Yangon
Yangquan
Yerevan
Yogyakarta
Zagreb
Zhengzhou
Zhongshan
Zibo
Zürich
```
