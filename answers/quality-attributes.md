# 5 ytri + 3 innri gæðaeiginleikar

## Ytri (5)

| Eiginleiki | Krafa | Rök/forsemdir|
|-------------|--------------------|-----------------------------|
| **1. Notendavæni** | Notandi skal geta lokið útláni eða skilum bókar innan 30 sekúndna án aðstoðar starfsmanns. | Kerfið er ætlað fjölbreyttum notendahóp, þar á meðal börnum og eldri borgurum, og þarf því að vera einfalt í notkun. Skýr viðmótsuppbygging og leiðbeinandi hönnun draga úr villum og bæta notendaupplifun. |
| **2. Færanleiki** | Kerfið skal virka á öllum helstu vöfrum og tækjum tölvum, spjaldtölvum og snjallsímum án þess að skerða virkni. | Notendur geta nýtt bókasafnið á mismunandi tækjum, heima eða á ferðinni. Þetta eykur aðgengi og þægindi en krefst erfiðari vefhönnun og prófana á mörgum kerfum. |
| **3. Áreiðanleiki** | Kerfið skal vera uppi ≥ 99% yfir hverjum mánuði. | Notendur þurfa að geta treyst á að sjálfsafgreiðslukerfið sé aðgengilegt á opnunartíma bókasafnsins. Þetta krefst öruggrar nettengingar og trausts gagnagrunns sem endurræsir sig sjálfkrafa við bilanir. |
| **4. Öryggi** | Aðgangur að notendagögnum skal krefjast auðkenningar með lykilorði eða rafrænum skilríkjum. | Kerfið geymir viðkvæmar upplýsingar um notendur og lánasögu. Dulkóðun og örugg auðkenning sem passa upp á persónuupplýsingar. |
| **5. Frammistaða** | Viðbragðstími kerfisins skal ekki fara yfir 1000 millisekúndur í 95% allra notendaaðgerða. | Hraðvirkni er nauðsynleg til að halda biðtíma stuttum og forðast biðraðir við sjálfsafgreiðslutæki. Skilvirk gagnavinnsla stuðlar að markmiðinu. |

---

## Innri (3)

| Eiginleiki | Krafa | Rök/forsemdir |
|-------------|--------------------|-----------------------------|
| **1. Viðhaldshæfni** | Kóðinn skal vera skipulagður í sjálfstæðum einingum með skýrum API-skilum. | Þannig er hægt að bæta nýjum eiginleikum eða laga villur án þess að trufla önnur kerfishluta. Þetta styður við langtímaþróun og minnkar líkur á keðjuvillum. |
| **2. Prófanleiki** | Allar megineiningar kerfisins skulu hafa a.m.k. 80% kóðayfirdekningu í einingaprófum. | Hátt prófunarhlutfall tryggir áreiðanleika og auðveldar viðhald. Forsenda er að kerfið noti sjálfvirkar prófanir og vel skilgreindar prófunareiningar. |
| **3. Viðbætanleiki** | Ný þjónusta eða viðmót skal vera hægt að bæta við án þess að breyta kjarnakerfi. | Þetta auðveldar samþættingu við aðrar bókasafnslausnir eða rafbókasöfn í framtíðinni. Notkun á viðmótum og þjónustulögum styður þessa kröfu. |

# Gæðakrafa 5. Frammistaða lýst í PLanguage

## Merkimiði (TAG)
`Performance.SelfCheckout.ResponseTime`

---

## Tilgangur / Ásetningur (AMBITION)
Kerfið skal tryggja hraðvirka svörun þegar notandi framkvæmir sjálfsafgreiðslu, svo að upplifun notandans verði hnökralaus og biðröð myndist ekki við afgreiðslustöðvarnar. Þetta er lykilatriði í því að auka notkun á sjálfsafgreiðslukerfinu og minnka þörf fyrir aðstoð bókavarða.

---

## Mælikvarði (SCALE)
Tími í millisekúndum sem líður frá því að notandi staðfestir aðgerð þar til kerfið birtir staðfestingu á skjánum.

---

## Mælir / Mæliaðferð (METER)
Mælt með sjálfvirkum tímamæli á 100 mismunandi sjálfsafgreiðsluaðgerðum í prófunarumhverfi sem endurspeglar raunverulegt notkunarumhverfi bókasafnsins.

---

## Markmið (GOAL)
Viðbragðstími skal vera **≤ 1000 ms** í **95%** allra aðgerða.  
*(Hagsmunaaðili: Bókasafnsstjóri / Notendaupplifunarteymi)*

---

## Æskilegt (STRETCH)
Viðbragðstími ≤ **700 ms** í 95% aðgerða.

---

## Óska (WISH)
Viðbragðstími ≤ **500 ms** í 95% aðgerða.

---

## Grunnkerfi (BASE PLATFORM)
Sjálfsafgreiðslustöð með:
- Intel i5 örgjörva  
- 8 GB RAM  
- SSD geymslu  
- Windows 11
- Stöðuga nettengingu ≥ 50 Mbps  
- MySQL gagnagrunn

