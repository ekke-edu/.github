# Útmutató a kurzusfeladatokhoz és projektekhez (Contributing Guidelines)

Üdvözlünk az Eszterházy Károly Katolikus Egyetem (EKKE) Software Engineering kurzusainak fejlesztői felületén! 

Ez a dokumentum összefoglalja, hogyan tudsz a leghatékonyabban dolgozni a feladatokon, mik a beadás technikai feltételei, és mik az egyetem elvárásai a mesterséges intelligencia (AI) használatával kapcsolatban. Kérjük, minden félév elején olvasd el figyelmesen!

---

## 1. Munkafolyamat (A feladatok megoldása)

A szervezet repóiba közvetlenül nem tudsz írni. A feladatok megoldásához a standard GitHub munkafolyamatot kell használnod:

1. **Fork:** A kiadott feladat repository-jának jobb felső sarkában kattints a `Fork` gombra, hogy létrehozz egy másolatot a saját profilod alatt.
2. **Clone:** A klónozáshoz mindig a *saját* forkolt repód URL-jét használd!
3. **Környezet:** Ha a feladat DevContainert vagy specifikus Docker/WSL2 környezetet igényel, kövesd a repó `README.md` fájljában leírt beállítási lépéseket.
4. **Commit:** Használj beszédes commit üzeneteket (pl. `feat: hozzáadva a FastAPI végpont` vagy `fix: adatbázis kapcsolat javítása`). A "kész", "asd" és "módosítva" nem elfogadható üzenetek.
5. **Push & Pull Request (PR):** Ha a feladat beadása GitHubon keresztül történik, a saját repódból nyiss egy Pull Requestet az eredeti (upstream) repó felé. A PR leírásában foglald össze, mit valósítottál meg.

---

## 2. Generatív AI Használati Szabályzat

A modern szoftverfejlesztésben az AI (Copilot, ChatGPT, Claude) használata mindennapos. Célunk nem a tiltás, hanem a tudatos használat megtanítása, a **Verification Code Paradigm** elvei alapján.

Amikor AI-t használsz, **TE vagy a kód gazdája**. A te felelősséged, hogy a kód helyes, biztonságos és az architektúrába illeszkedő legyen.

### ✅ Támogatott AI használat:
* Ötletelés, rendszerek megtervezése (architektúra, adatbázis sémák).
* Fogalmak, technológiák és hibaüzenetek elmagyaráztatása.
* Alapvázak (boilerplate) generálása.
* Hibakeresés logok alapján.

### 🚫 Szigorúan TILOS és plágiumnak minősül:
* **Vak másolás (Copy-Paste):** Generált kódok ellenőrzés és megértés nélküli bemásolása a projektbe.
* **Tudás elrejtése:** Olyan kód leadása, amit nem tudsz sorról sorra elmagyarázni a védés/számonkérés során. *(Ha nem érted a memóriakezelést vagy a kiválasztott algoritmust a saját kódodban, a feladat érvénytelenítésre kerül.)*
* **Titkos adatok kiadása:** Egyetemi adatbázis jelszavak, API kulcsok vagy más szenzitív adatok megosztása a publikus modellekkel.

### AI Használati Nyilatkozat (Kötelező!)
Ha a kódod megírásához generatív AI eszközt használtál, azt a Pull Request leírásában **vagy** a forráskód kommentjeiben egyértelműen jelezned kell.

*Példa a kódba:*
```python
# [AI GENERATED & MODIFIED] A vektor-kereső függvény vázlatát a Copilot generálta, a küszöbértékeket módosítottam.
```

---

## 3. Segítségkérés és Hibajelentés
Elakadtál a kódolásban vagy nem indul a Docker konténer? Kérjük, ne e-mailben küldj képernyőfotókat a kódodról, hanem használd a GitHub beépített eszközeit:

1. Discussions / Issues: Nyiss egy új Issue-t vagy témát a kurzus repójában.
2. Környezet megadása: Mindig írd le az operációs rendszeredet (pl. Windows 11 + WSL2 Ubuntu) és az eszközök verzióját.
3. Pontos hibaüzenet: Másold be a terminálban kapott pontos hibaüzenetet szövegként (ne csak képernyőfotót).
4. Reprodukció: Írd le, mit próbáltál eddig, és hogyan tudjuk mi is reprodukálni a hibát.

## 4. Kódminőség és Tisztaság

- Nevek: Változók, függvények és osztályok elnevezésére használj angol nyelvet.
- Formázás: Használd a kurzusban előírt formázó (linter/formatter) eszközöket mielőtt commitolsz.
- Kommentek: Ne azt kommenteld, hogy mit csinál a kód (azt a kódnak kell elmondania), hanem azt, hogy miért azt a megoldást választottad!
