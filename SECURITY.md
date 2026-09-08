[Magyar verzió](#magyar-verzió) | [English version](#english-version)

---

# Magyar verzió

## Biztonsági Irányelvek (Security Policy)

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

---

# English version

## Security Policy

Secure coding and data protection are especially important in our courses.

---

## 1. Secrets Management

During student assignments and projects, **you must never upload real, active sensitive data** to repositories.

* **What should never be uploaded?**
  * Database passwords, root access credentials (such as credentials for the university's production Oracle or MongoDB systems).
  * API keys (OpenAI, GitHub tokens, Postman keys, and so on).
  * Personal data (Neptun codes, passwords, or private email addresses hardcoded in the source code).
* **Use this instead:** Always use `.env` files for configuration, and make sure `.env` is included in `.gitignore`! Only an `.env.example` template with empty values may be shared in the repository.

---

## 2. Reporting a Vulnerability or Bug

If you find a security vulnerability, incorrect permissions, or sensitive information left in a public location in one of the course assignments or template projects, **do not open a public Issue**, because it would expose the problem to others as well.

Instead, report it directly to an instructor:

* **By email:** [szilvasi.istvan.peter@uni-eszterhazy.hu](mailto:szilvasi.istvan.peter@uni-eszterhazy.hu)
* **On GitHub:** Send a private message or report it during a consultation.

---

## 3. Environment Security (Docker & WSL2)

When using development containers (Docker Dev Containers, WSL2), make sure your local development environment does not unnecessarily expose dangerous ports to the public network, especially when working on the university network or a dormitory Wi-Fi connection.
