# Biztonsági Irányelvek (Security Policy)

A kurzusokon kiemelten fontosnak tartom a biztonságos kódolást és az adatok védelmét.

---

## 1. Titkos adatok kezelése (Secrets Management)

A hallgatói feladatok és projektek során **szigorúan tilos** bármilyen éles, valós szenzitív adatot feltölteni a repository-kba.

* **Mit ne tölts fel soha?**
  * Adatbázis jelszavakat, root hozzáféréseket (pl. az egyetemi Oracle vagy MongoDB éles kredenciáljait).
  * API kulcsokat (OpenAI, GitHub tokenek, Postman kulcsok stb.).
  * Személyes adataidat (neptun kód, jelszó, privát email címek a kódban hardkódolva).
* **Helyette használd:** Mindig használj `.env` fájlokat a konfigurációhoz, és győződj meg róla, hogy a `.env` benne van a `.gitignore`-ban! A repóban csak `.env.example` sablont szabad megosztani, üres értékekkel.

---

## 2. Biztonsági rés vagy hiba jelentése

Ha a kurzusokhoz kiadott feladatok valamelyikében (vagy a sablonkódokban) biztonsági rést, elrontott jogosultságot, vagy publikus helyen felejtett érzékeny információt találsz, **ne nyiss róla nyilvános Issue-t**, mert azzal mások is láthatják a problémát!

Ehelyett kérjük, hogy közvetlenül az oktatónak jelezd:
* **E-mailben:** [szilvasi.istvan.peter@uni-eszterhazy.hu](mailto:szilvasi.istvan.peter@uni-eszterhazy.hu)
* **GitHubon:** Küldj egy privát üzenetet vagy jelezd a konzultáción.

---

## 3. Környezetbiztonság (Docker & WSL2)

A fejlesztéshez használt konténerekben (Docker DevContainers, WSL2) mindig ügyelj arra, hogy a helyi fejlesztői környezetedben ne nyiss meg feleslegesen veszélyes portokat a publikus hálózat felé, különösen ha az egyetemi hálózaton vagy kollégiumi Wi-Fi-n dolgozol.
