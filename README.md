# Teams Cheat Sheet


- https://www.microsoft365.com/launch/stream?auth=2



# Transkribieren

<details><summary>Click to expand..</summary>


## Aktivieren
- * Nur bei **echten, geplanten Meetings** (nicht 1:1-Calls oder spontanem Anrufen) greifen die Recording-Optionen. * Muss über Outlook/Teams-Kalender erstellt worden sein.

<details><summary>Click to expand..</summary>
  
Perfekt – wenn du der Admin bist, kannst du das direkt im **Microsoft Teams Admin Center** freischalten. Hier ist dein klarer Fahrplan 🛠️:

---

### 🔓 **Aufzeichnung und Transkription aktivieren**

#### 1. **Teams Admin Center öffnen**

👉 [https://admin.teams.microsoft.com/](https://admin.teams.microsoft.com/)

#### 2. **Links im Menü zu folgendem navigieren:**

`Besprechungen` → `Besprechungsrichtlinien`

#### 3. **Richtlinie auswählen oder neue Richtlinie erstellen:**

* Entweder bearbeitest du die **globale (Standard)** Richtlinie oder du wählst eine bestimmte benutzerdefinierte Richtlinie.
* Klicke auf den Namen der Richtlinie.

#### 4. **Folgende Optionen aktivieren:**

| Einstellung                    | Wert      |
| ------------------------------ | --------- |
| **Cloudaufzeichnung zulassen** | ✅ **Ein** |
| **Transkription zulassen**     | ✅ **Ein** |

#### 5. **Speichern nicht vergessen**

#### 6. **Richtlinie zuweisen (falls notwendig):**

* Wenn du **nicht die globale Richtlinie** geändert hast:

  * Gehe zu `Benutzer` → wähle betroffenen User aus → `Richtlinien` → `Besprechungsrichtlinie` → zuweisen.

---

### 🧠 Hinweis:

Es kann **bis zu 24 Stunden dauern**, bis die Änderungen aktiv werden (meist schneller, aber MS liebt Bürokratie).

Möchtest du's auch via **PowerShell** machen?


<br><br>



Gut, dass du’s bereits gemacht hast – jetzt knöpfen wir uns die üblichen Stolperfallen vor. Hier kommt der Check-up 🕵️‍♂️:

---

### ✅ **Checkliste: Wenn Aufzeichnung & Transkription immer noch gesperrt sind**

#### 1. **Richtlinie wirklich aktiv beim Benutzer?**

Auch wenn du die Richtlinie geändert hast: Ist sie dem Benutzer **wirklich zugewiesen**?

➡️ **Prüfen unter:**
`Teams Admin Center → Benutzer → [User anklicken] → Richtlinien → Besprechungsrichtlinie`

> Muss dort deine geänderte Richtlinie sein (z. B. „Global (Standard)“ oder die, die du angepasst hast).

---

#### 2. **Meeting-Organisator hat die richtige Richtlinie?**

Die Berechtigungen greifen **nur, wenn der Organisator** des Meetings die entsprechende Richtlinie hat – nicht nur die Teilnehmer!

---

#### 3. **Meeting ist ein *geplantes* Teams-Meeting?**

* Nur bei **echten, geplanten Meetings** (nicht 1:1-Calls oder spontanem Anrufen) greifen die Recording-Optionen.
* Muss über Outlook/Teams-Kalender erstellt worden sein.

---

#### 4. **OneDrive/SharePoint aktiviert?**

Teams speichert Aufzeichnungen in OneDrive/SharePoint. Wenn das abgeschaltet ist, geht gar nix.

➡️ Prüfen im **Microsoft 365 Admin Center → Einstellungen → Dienste → OneDrive/SharePoint**

---

#### 5. **Compliance-Richtlinien?**

Hat eure Organisation Microsoft Purview / DLP / Information Protection aktiviert? → Manchmal blockieren diese **Aufzeichnungen und Transkripte automatisch** bei sensiblen Inhalten.

---

#### 6. **Lizenztyp prüfen:**

Für Transkription brauchst du **Teams Premium**, **E5** oder **Microsoft 365 Business Standard/Premium**.

➡️ Prüfen unter:
`Microsoft 365 Admin Center → Benutzer → Aktive Benutzer → [User anklicken] → Lizenzen und Apps`

---

Wenn du willst, schick mir einen Screenshot vom Benutzer + Richtlinie oder sag, welche Lizenz ihr habt – dann entwirre ich’s genau für deinen Fall 🧩

Willst du zusätzlich den PowerShell-Befehl, um alle Richtlinienzuweisungen für einen User abzufragen?





</details>




## Download
- Man kann es auch in **Teams**, in der **Applikation** an sich sehen, unter **Aktivität** zum Beispiel, nachdem das **Gespräch** vorbei ist oder auch dann im **Kalender**, wie du meintest, wenn man nochmal da reingeht, dort ist eine komplette **Übersicht**, wo man es auch **herunterladen** kann.


<details><summary>Click to expand..</summary>


Um eine **Transkription in Microsoft Teams herunterzuladen**, brauchst du:

1. Das Meeting muss **aufgezeichnet** **und** die **Transkription aktiviert** worden sein.
2. Du musst **Organisator oder Teilnehmer** mit Zugriffsrechten sein.

---

### 📥 So lädst du die Transkription herunter:

#### 🔹 **Weg 1: Über den Teams-Meeting-Chat**

1. Geh in **Teams → Chat → wähle den Meeting-Chat**.
2. Dort findest du unter dem Video-Link: **„Transkription anzeigen“** oder **„Meetingprotokoll“**.
3. Öffne die Transkription.
4. Oben rechts auf die **drei Punkte** (⋯) klicken → **Herunterladen**.
5. Wähle Format:

   * **.docx** (Word)
   * **.vtt** (für Untertitel)

#### 🔹 **Weg 2: Über Microsoft Stream (falls verwendet)**

Falls das Meeting in **Stream (classic)** oder **Stream on SharePoint** gespeichert wurde:

1. Geh zu [https://stream.microsoft.com/](https://stream.microsoft.com/)
2. Öffne die Aufzeichnung.
3. Klick auf **„Transkript“** im Seitenbereich.
4. Oben rechts: **⋯ → Transkript herunterladen**.

---

### ❗ Wichtig:

* Funktioniert nur, wenn **Transkription beim Meeting aktiv war**.
* Wenn du nichts findest, wurde **keine Transkription erstellt oder gespeichert**.
* Die **Sprache** muss vor dem Meeting korrekt eingestellt worden sein – sonst wird nichts transkribiert.

Möchtest du ein Script, um Transkripte automatisch zu sichern?


  
</details>



  
</details>





































