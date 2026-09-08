[Magyar verzió](#magyar-verzió) | [English version](#english-version)

---

# Magyar verzió

## Útmutató a kurzusfeladatokhoz és projektekhez (Contributing Guidelines)

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

---

# English version

## Guidelines for Course Assignments and Projects (Contributing Guidelines)

Welcome to the development environment for the Software Engineering courses at Eszterházy Károly Catholic University (EKKE)!

This document summarizes how to work effectively on assignments, the technical requirements for submissions, and the university's expectations regarding the use of artificial intelligence (AI). Please read it carefully at the beginning of every semester!

---

## 1. Workflow (Working on Assignments)

You cannot write directly to the organization's repositories. You must use the standard GitHub workflow to complete assignments:

1. **Fork:** Click the `Fork` button in the upper-right corner of the provided assignment repository to create a copy under your own profile.
2. **Clone:** Always use the URL of *your own* fork when cloning the repository.
3. **Environment:** If the assignment requires a Dev Container or a specific Docker/WSL2 environment, follow the setup steps described in the repository's `README.md` file.
4. **Commit:** Use descriptive commit messages (for example, `feat: add FastAPI endpoint` or `fix: repair database connection`). Messages such as "done", "asd", and "modified" are not acceptable.
5. **Push & Pull Request (PR):** If the assignment is submitted through GitHub, open a Pull Request from your repository to the original (upstream) repository. Summarize what you implemented in the PR description.

---

## 2. Generative AI Usage Policy

AI tools such as Copilot, ChatGPT, and Claude are a normal part of modern software development. Our goal is not to ban them, but to teach responsible use based on the principles of the **Verification Code Paradigm**.

When you use AI, **YOU are the owner of the code**. You are responsible for ensuring that the code is correct, secure, and consistent with the architecture.

### Supported AI Use

* Brainstorming and system design (architecture, database schemas).
* Asking for explanations of concepts, technologies, and error messages.
* Generating boilerplate.
* Debugging based on logs.

### Strictly PROHIBITED and Considered Plagiarism

* **Blind copy-paste:** Adding generated code to a project without checking or understanding it.
* **Concealing a lack of knowledge:** Submitting code that you cannot explain line by line during a defense or assessment. *(If you do not understand memory management or the selected algorithm in your own code, the assignment will be invalidated.)*
* **Disclosing secrets:** Sharing university database passwords, API keys, or other sensitive data with public models.

### AI Usage Statement (Required!)

If you used a generative AI tool to write your code, you must clearly disclose it in the Pull Request description **or** in the source code comments.

*Example in code:*
```python
# [AI GENERATED & MODIFIED] Copilot generated the outline of the vector search function; I modified the thresholds.
```

---

## 3. Asking for Help and Reporting Issues

Are you stuck while coding, or will the Docker container not start? Please do not email screenshots of your code. Instead, use GitHub's built-in tools:

1. Discussions / Issues: Open a new Issue or discussion in the course repository.
2. Environment details: Always describe your operating system (for example, Windows 11 + WSL2 Ubuntu) and the versions of your tools.
3. Exact error message: Paste the exact error message from the terminal as text, rather than providing only a screenshot.
4. Reproduction: Explain what you have tried so far and how we can reproduce the problem.

## 4. Code Quality and Clarity

- Names: Use English for the names of variables, functions, and classes.
- Formatting: Run the formatter or linter required by the course before committing.
- Comments: Do not comment on what the code does (the code should express that); explain why you chose the solution instead.
