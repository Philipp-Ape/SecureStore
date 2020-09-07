# FAQ

  

## <span style="color:dodgerblue">Allgemeine Fragen</span>

  

[//]: #  (Port- & Adressfreigaben)

<details>

<summary><b>Port- & Adressfreigaben</b></summary>

  

### Ports und Protokolle

|Protokoll|Richtung |Ports |Bemerkung |

|:-------:|:--------:|:-----------------------------------------:|:------------------------------------------:|

|**HTTPS**|📶 Extern|**443**/*TCP* | |

|**HTTP** |📶 Extern|**80**/*TCP* |**Nicht für Live-Betrieb geeignet!** |

|**SMTP** |📶 Extern|**25**/*TCP*; **465**/*TCP*; **587**/*TCP* |*Nur, wenn HTTPS absolut nicht möglich ist!*|

|**SNMP** |🔗 Intern|**160**/*UDP*; **161**/*UDP*; **162**/*UDP*|*162 nur, wenn benötigt (Trap)* |

|**ECHO** |🔗 Intern|**7**/*TCP* | |

|**TCP** |🔗 Intern|**9148**/*TCP* | |

  

### Adressen

|Adresse |IP-Adresse |

|:------------------------------|:----------------:|

|https://fm.bissinger.de/ |**128.65.147.76** |

|https://update.simpleclicks.de/|**212.227.72.212**|

  

---

</details>

  

[//]: #  (Limitierung bei Erstellung von Zugängen)

<details>

<summary><b>Sonderzeichen in Zugängen</b></summary>

  

Ein Zugang darf nur einen gewissen Zeichensatz verwenden, damit dieser einwandfrei funktioniert! Im Passwort dürfen beispielsweise **keine** doppelten Anführungszeichen (``"``) vorkommen, die Anmeldung funktioniert ansonsten nicht.

Gleiches gilt beim Vergeben von Benutzernamen. Hier darf z.B. auch kein ``@`` verwendet werden.

Aufgrund der speziellen Behandlung von Passwörtern, dürfen für Passwörter keine Umlaute, wie ``Ä, Ö, Ü, ß`` verwendet werden.

Dies gilt für alle Logins in SimpleClicks, egal wo diese angelegt werden können.

  

### Auflistung von Zeichen, die für **Benutzernamen** verwendet werden können:

- Buchstaben von ``a bis z`` und von ``A bis Z``

- Umlaute (``ä, ö, ü, Ä, Ö, Ü, ß``)

- Zahlen von ``0 bis 9``

-  ``Leerzeichen``, ``!``, ``?``, ``-``, ``+``, ``.``, ``,``, ``/``, ``&``

  

### Auflistung von Zeichen, die für **Passwörter** verwendet werden können:

- Buchstaben von ``a bis z`` und von ``A bis Z``

- Zahlen von ``0 bis 9``

-  ``Leerzeichen``, ``!``, ``?``

  

> Möglicherweise sind noch einige weitere Zeichen möglich - hierzu bitte einfach testen und nachtragen.

  

---

</details>

  

[//]: #  (Gleichzeitiges Anlegen von Zugängen im Server)

<details>

<summary><b>Gleichzeitiges Anlegen von Zugängen im Server (<code>Datenschutzrelevant</code>)</b></summary>

  

Sollten mehrere Benutzer zeitgleich einen Zugang anlegen, kommt es zu **Datenverlust**!

  

<img  src="../.media/image001.png">

  

Sobald ein neuer Zugang angelegt wird, wird die Ansicht in anderen Browsersitzungen nicht aktualisiert. Speichert ein zweiter Benutzer seinen neuen Zugang, bevor seine Ansicht aktualisiert worden ist, wird der erste Zugang verworfen, da dieser in der Ansicht des zweiten Benutzers nicht vorhanden war.

Dies passiert auch, wenn ein Nutzer mit einer noch nicht aktualisierten Ansicht auf ``Speichern`` klickt - dann werden neue Daten mit dem Stand des Benutzers überschrieben. Es empfiehlt sich daher, Zugänge koordiniert einzutragen, sowie die Webseite gelegentlich zu aktualisieren (insbesondere, bevor Änderungen vorgenommen werden).

  

---

</details>

  

[//]: #  (Wo finde ich den 32-Bit Agent?)

<details>

<summary><b>Wo finde ich den 32-Bit Agent?</b></summary>

  

Der 32-Bit Agent ist zur Zeit auf der <a  href="https://www.simpleclicks.de/download">SimpleClicks-Website</a> zum Download verfügbar.

Alternativ sind sowohl die Installationsdateien des 64-Bit als auch 32-Bit Agents in der Bissinger Cloud unter

``SHB-Technik\SimpleClicks\Installationsdateien`` zu finden.

*Der Support des 32-Bit Agents läuft nach und nach aus, da Oracle den 32-Bit Support für Java 9 abgekündigt hat und es daher keine 32-Bit Versionen vom JRE mehr geben wird.*

  

---

</details>

  

[//]: #  (Wo finde ich die aktuellste Master Konfiguration?)

<details>

<summary><b>Wo finde ich die aktuellste Master Konfiguration?</b></summary>

  

Die aktuellsten Konfigurationsdateien sind in der Kategorie **SimpleClicks** im ``OneNote`` oder im Ordner:

``G:\SHB-Technik\SimpleClicks\Konfigurationen`` zu finden.

  

---

</details>

  

[//]: #  (Woher kann ich Kundennummern entnehmen?)

<details>

<summary><b>Woher kann ich Kundennummern entnehmen?</b></summary>

  

### Serviceschein

Als Kundennummer sollte die Nummer über dem Kundennamen auf dem Auftrag hinterlegt werden:

  

<img  src="../.media/image002.png">

  

Falls es sich hierbei um Grenke-/ABC-Nummern handelt, können diese Nummern von den Rollout Technikern ebenfalls verwendet werden.

  

> @Fleet-Team:

In regelmäßigen Abständen sollten die Grenke-/ABC-Nummern durch die jeweiligen Debitorennummern ersetzt werden. Nummern sind folgende:

>- 346374

>- 332846

>- 324144

  

### Auftrag

Den jeweiligen Auftrag öffnen (*``Shift`` + ``F5``*), im Reiter ``Allgemein`` steht dies im Feld ``Verk. an Deb.-Nr.``:

  

<img  src="../.media/image003.png">

  

### Callerfassung

<img  src="../.media/image004.png">

<img  src="../.media/image005.png">

<img  src="../.media/image006.png">

  

Mit ``Strg`` + ``F`` nach Kundennamen suchen und Debitorennummer kopieren:

  

<img  src="../.media/image007.png">

  

---

</details>

  

## <span style="color:dodgerblue">Installation & Einrichtung</span>

  

## <span style="color:dodgerblue">Probleme</span>

<details>

<summary><b>Mein Leben?</b></summary>

  

❗❌ Diese Sektion wird gelöscht!

  

---

</details>
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc4MDk1MTIwNF19
-->