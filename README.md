# AI-stödd plananalys – Detaljplan Borrby 58:3 och S:35

Detta projekt innehåller en AI-genererad analys av granskningsyttranden för detaljplanen vid Borrbystrand i Simrishamns kommun.

## 🌐 Webbplats

**Se projektet live:** [https://lundgren9.github.io/Borrby/](https://lundgren9.github.io/Borrby/)

## 📁 Filer i projektet

| Fil | Beskrivning |
|-----|-------------|
| `index.html` | Startsida med översikt, information om planprocessen och länkar |
| `Sammanstallning_granskningsyttranden_Borrby.docx` | Word-dokument med sammanställning i löpande text |
| `Granskningsyttranden_Borrby_tabell.xlsx` | Excel-fil med filtrerbar tabell över alla yttranden |
| `Planillustration_Borrby_markanvandning.html` | Interaktiv karta över markanvändning |
| `Principsnitt_Borrby_tillganglighet.html` | Principsnitt som visar alternativa lösningar |
| `Antagandehandling_Borrby_58_3_Borrby_S_35...pdf` | Ursprunglig antagandehandling (38 sidor) |
| `Yttranden_sammanslaget2.pdf` | Sammanslagna granskningsyttranden |
| `Protokoll SPn april 2024_Bortredigerad.pdf` | Protokoll från samhällsplaneringsnämnden |

## 🛠️ Teknik

- **AI:** Claude (Anthropic) för analys och kodgenerering
- **Word-dokument:** docx.js (JavaScript)
- **Excel-fil:** openpyxl (Python)
- **Illustrationer:** HTML, CSS, SVG

## 📖 Om projektet

Projektet demonstrerar hur generativ AI kan användas för att:
- Sammanställa och kategorisera granskningsyttranden
- Identifiera intressekonflikter mellan sakägare
- Skapa pedagogiska visualiseringar
- Föreslå alternativa lösningar baserat på inkomna synpunkter

---

# 🚀 Guide: Arbeta med GitHub-filer i Cursor eller VS Code

Den här guiden förklarar steg-för-steg hur du laddar ner projektet från GitHub, arbetar med det lokalt på din dator, och sedan laddar upp det till din egen webbplats.

## Innehåll

1. [Vad är vad? (Ordlista)](#-vad-är-vad-ordlista)
2. [Installera programvara](#-steg-1-installera-programvara)
3. [Ladda ner projektet från GitHub](#-steg-2-ladda-ner-projektet-från-github-klona)
4. [Öppna projektet i Cursor/VS Code](#-steg-3-öppna-projektet-i-cursorvs-code)
5. [Göra ändringar och spara](#-steg-4-göra-ändringar-och-spara)
6. [Synka ändringar tillbaka till GitHub](#-steg-5-synka-ändringar-tillbaka-till-github)
7. [Ladda upp till din webbplats](#-steg-6-ladda-upp-till-din-webbplats)
8. [Vanliga problem och lösningar](#-vanliga-problem-och-lösningar)

---

## 📚 Vad är vad? (Ordlista)

Innan vi börjar, här är några begrepp du behöver känna till:

| Begrepp | Förklaring |
|---------|------------|
| **Git** | Ett program som håller reda på alla ändringar i dina filer (versionhantering). Tänk dig att du kan "spara" olika versioner och alltid gå tillbaka. |
| **GitHub** | En webbplats där du lagrar dina Git-projekt online. Som en molnlagring för kod. |
| **Repository (repo)** | En projektmapp på GitHub. Det här projektet ligger i repot "Borrby". |
| **Klona** | Att ladda ner en kopia av ett GitHub-projekt till din dator. |
| **Commit** | Att "spara" dina ändringar med ett meddelande som beskriver vad du gjort. |
| **Push** | Att ladda upp dina sparade ändringar (commits) till GitHub. |
| **Pull** | Att hämta de senaste ändringarna från GitHub till din dator. |
| **Cursor** | Ett modernt IDE (kodredigerare) med inbyggd AI. Baserat på VS Code. |
| **VS Code** | Visual Studio Code – ett populärt, gratis IDE från Microsoft. |
| **IDE** | Integrated Development Environment – ett program för att skriva och redigera kod. |
| **FTP/SFTP** | Protokoll för att ladda upp filer till en webbserver. |

---

## 📥 Steg 1: Installera programvara

Du behöver installera två saker: **Git** och **Cursor** (eller VS Code).

### 1.1 Installera Git

Git är motorn som hanterar versioner och synkronisering.

1. Gå till: **https://git-scm.com/downloads**
2. Klicka på **"Download for Windows"** (eller Mac/Linux)
3. Öppna den nedladdade filen och följ installationen
4. **Viktigt:** Behåll alla standardinställningar – klicka bara "Next" hela vägen

#### ✅ Kontrollera att Git är installerat:
1. Öppna **Kommandotolken** (sök efter "cmd" i Windows startmeny)
2. Skriv: `git --version`
3. Tryck Enter
4. Du ska se något i stil med: `git version 2.43.0`

Om du ser ett versionsnummer är Git installerat! ✓

### 1.2 Installera Cursor (rekommenderas)

Cursor är som VS Code men med inbyggd AI-hjälp.

1. Gå till: **https://cursor.com**
2. Klicka på **"Download"**
3. Öppna den nedladdade filen och följ installationen
4. Starta Cursor när installationen är klar

### 1.3 Alternativ: Installera VS Code

Om du föredrar VS Code:

1. Gå till: **https://code.visualstudio.com**
2. Klicka på **"Download for Windows"**
3. Öppna den nedladdade filen och följ installationen

> 💡 **Tips:** Cursor och VS Code fungerar nästan identiskt. Cursor är baserat på VS Code, så allt du lär dig i det ena fungerar i det andra.

---

## 📂 Steg 2: Ladda ner projektet från GitHub (klona)

Nu ska vi hämta projektfilerna från GitHub till din dator.

### 2.1 Skapa en mapp för dina projekt

Först behöver du en plats att spara projektet:

1. Öppna **Utforskaren** (Windows Explorer)
2. Gå till **Dokument**
3. Högerklicka → **Ny** → **Mapp**
4. Döp mappen till: `GitHub-projekt`

Nu har du mappen: `C:\Users\[DittNamn]\Documents\GitHub-projekt`

### 2.2 Kopiera repository-adressen

1. Gå till: **https://github.com/lundgren9/Borrby**
2. Klicka på den gröna knappen **"<> Code"**
3. Se till att fliken **"HTTPS"** är vald
4. Klicka på **📋-ikonen** för att kopiera adressen

Adressen som kopieras är: `https://github.com/lundgren9/Borrby.git`

### 2.3 Klona projektet via Cursor

1. Öppna **Cursor**
2. Klicka på **"Clone Git Repository..."** på startsidan
   - (Eller gå till menyn: **File** → **Clone Git Repository...**)
3. Klistra in adressen: `https://github.com/lundgren9/Borrby.git`
4. Tryck **Enter**
5. Välj mappen du skapade: `Dokument/GitHub-projekt`
6. Klicka **"Select as Repository Destination"**
7. Vänta medan filerna laddas ner
8. Klicka **"Open"** när det frågas om du vill öppna projektet

🎉 **Klart!** Nu har du alla filer på din dator.

### 2.4 Alternativ: Klona via kommandotolken

Om du föredrar att använda terminalen:

```bash
# 1. Öppna kommandotolken (cmd)

# 2. Gå till din projektmapp
cd Documents\GitHub-projekt

# 3. Klona projektet
git clone https://github.com/lundgren9/Borrby.git

# 4. Gå in i projektmappen
cd Borrby
```

---

## 💻 Steg 3: Öppna projektet i Cursor/VS Code

Om projektet inte redan är öppet:

1. Öppna **Cursor** (eller VS Code)
2. Klicka **File** → **Open Folder...**
3. Navigera till: `Dokument/GitHub-projekt/Borrby`
4. Klicka **"Välj mapp"**

### Så här ser det ut:

```
BORRBY (projektmapp)
├── 📄 index.html                    ← Startsidan
├── 📄 Planillustration_Borrby_markanvandning.html
├── 📄 Principsnitt_Borrby_tillganglighet.html
├── 📄 Sammanstallning_granskningsyttranden_Borrby.docx
├── 📄 Granskningsyttranden_Borrby_tabell.xlsx
├── 📄 Antagandehandling_Borrby_58_3_Borrby_S_35...pdf
├── 📄 Yttranden_sammanslaget2.pdf
├── 📄 Protokoll SPn april 2024_Bortredigerad.pdf
└── 📄 README.md                     ← Den här filen
```

### Förhandsgranska HTML-filer:

1. Högerklicka på `index.html` i fillistan
2. Välj **"Open with Live Server"** (om tillägget är installerat)
   - Eller: Högerklicka → **"Reveal in File Explorer"** → Dubbelklicka på filen

---

## ✏️ Steg 4: Göra ändringar och spara

### 4.1 Redigera en fil

1. Klicka på filen du vill ändra (t.ex. `index.html`)
2. Gör dina ändringar i editorn
3. Spara med **Ctrl + S** (eller **Cmd + S** på Mac)

Du ser en prick (●) vid filnamnet om filen har osparade ändringar.

### 4.2 Se dina ändringar i webbläsaren

1. Öppna **Utforskaren** och navigera till projektmappen
2. Dubbelklicka på `index.html`
3. Filen öppnas i din webbläsare
4. Efter ändringar: Tryck **F5** för att uppdatera sidan

---

## 🔄 Steg 5: Synka ändringar tillbaka till GitHub

När du gjort ändringar och vill spara dem på GitHub:

### 5.1 Öppna Source Control

1. Klicka på **Source Control-ikonen** i vänstermenyn (ser ut som en förgrening: 🔀)
   - Eller tryck **Ctrl + Shift + G**
2. Du ser en lista med ändrade filer

### 5.2 Gör en commit (spara ändringarna)

1. Skriv ett meddelande som beskriver vad du ändrat i textrutan
   - Exempel: `"Uppdaterat kontaktinformation i index.html"`
2. Klicka på **✓ Commit** (bocken)
3. Om det frågas, välj **"Yes"** för att stagea alla ändringar

### 5.3 Pusha till GitHub (ladda upp)

1. Klicka på **"Sync Changes"** eller **"Push"**
   - Du kan också se en ↑-pil med en siffra som visar antal commits att pusha
2. Första gången kan du behöva logga in på GitHub:
   - Klicka **"Allow"** i popup-rutan
   - Logga in med ditt GitHub-konto i webbläsaren som öppnas

🎉 **Klart!** Dina ändringar finns nu på GitHub.

### 5.4 Hämta ändringar från GitHub (pull)

Om någon annan (eller du själv från en annan dator) har gjort ändringar:

1. Klicka på **Source Control-ikonen**
2. Klicka på **"..."** (tre punkter) högst upp
3. Välj **"Pull"**

Eller i terminalen:
```bash
git pull
```

---

## 🌍 Steg 6: Ladda upp till din webbplats

Nu vill du få filerna till din webbplats www.kentlundgren.se. Det finns flera sätt:

### Metod A: Via FTP-program (rekommenderas för nybörjare)

#### Steg 1: Installera FileZilla

1. Gå till: **https://filezilla-project.org**
2. Ladda ner **FileZilla Client** (inte Server)
3. Installera programmet

#### Steg 2: Anslut till din webbserver

Du behöver FTP-uppgifter från ditt webbhotell. Vanligtvis:
- **Värd:** ftp.kentlundgren.se (eller liknande)
- **Användarnamn:** (från ditt webbhotell)
- **Lösenord:** (från ditt webbhotell)
- **Port:** 21 (FTP) eller 22 (SFTP)

1. Öppna **FileZilla**
2. Fyll i uppgifterna högst upp:
   - Värd: `ftp.kentlundgren.se`
   - Användarnamn: `[ditt användarnamn]`
   - Lösenord: `[ditt lösenord]`
   - Port: `21`
3. Klicka **"Snabbanslut"**

#### Steg 3: Ladda upp filerna

FileZilla visar två paneler:
- **Vänster:** Din dator
- **Höger:** Webbservern

1. **Vänster panel:** Navigera till `Dokument/GitHub-projekt/Borrby`
2. **Höger panel:** Navigera till mappen där du vill ha filerna
   - Ofta: `public_html` eller `www` eller en undermapp
3. Markera filerna du vill ladda upp
4. Högerklicka → **"Ladda upp"**
5. Vänta tills överföringen är klar

#### Steg 4: Testa

Gå till din webbplats och kontrollera att filerna syns:
- `www.kentlundgren.se/Borrby/index.html`

### Metod B: Via VS Code-tillägg (SFTP)

Om du vill synka direkt från Cursor/VS Code:

1. Installera tillägget **"SFTP"** av Natizyskunk
2. Tryck **Ctrl + Shift + P**
3. Skriv: `SFTP: Config`
4. En fil `sftp.json` skapas. Fyll i:

```json
{
    "name": "kentlundgren.se",
    "host": "ftp.kentlundgren.se",
    "protocol": "sftp",
    "port": 22,
    "username": "ditt-användarnamn",
    "password": "ditt-lösenord",
    "remotePath": "/public_html/Borrby",
    "uploadOnSave": true
}
```

5. Spara filen
6. Högerklicka på en fil → **"Upload"**

---

## ❓ Vanliga problem och lösningar

### Problem: "git is not recognized"
**Lösning:** Git är inte installerat eller inte tillagt i PATH. Installera om Git och se till att kryssa i "Add to PATH" under installationen.

### Problem: Får inte pusha till GitHub
**Lösning:** 
1. Kontrollera att du är inloggad på GitHub i Cursor/VS Code
2. Gå till **File** → **Preferences** → **Settings**
3. Sök efter "github" och logga in

### Problem: "Permission denied" vid FTP
**Lösning:** Kontrollera att du har rätt användarnamn och lösenord. Kontakta ditt webbhotell om du är osäker.

### Problem: Sidan ser konstig ut på webbplatsen
**Lösning:** Kontrollera att alla filer (HTML, CSS, bilder) har laddats upp och ligger i rätt mappar.

### Problem: Ändringar syns inte på GitHub
**Lösning:** 
1. Kontrollera att du har sparat filen (Ctrl + S)
2. Gör en commit (skriv meddelande + klicka ✓)
3. Pusha (klicka Sync Changes)

---

## 📚 Läs mer

- [Git - officiell dokumentation](https://git-scm.com/doc)
- [GitHub - kom igång](https://docs.github.com/en/get-started)
- [Cursor - dokumentation](https://cursor.sh/docs)
- [VS Code - dokumentation](https://code.visualstudio.com/docs)
- [FileZilla - manual](https://wiki.filezilla-project.org/Documentation)

---

## 📝 Licens

Detta projekt är skapat för utbildnings- och demonstrationssyfte.

---

## 👤 Kontakt

- **GitHub:** [lundgren9](https://github.com/lundgren9)
- **Webbplats:** [www.kentlundgren.se](https://www.kentlundgren.se)

---

*Senast uppdaterad: December 2025*
