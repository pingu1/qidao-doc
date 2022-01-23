---
description: >-
  In diesem Leitfaden wird eine Strategie vorgestellt, die erstaunliche
  Wechselwirkungen zwischen Mai Finance, QuickSwap und Adamant nach der
  Einführung neuer LP-Pools auf Mai Finance und QuickSwap aufz
---

# Farmen oder Staken? Oder doch beides?

![](../../.gitbook/assets/screen-shot-2021-09-03-at-9.24.12-am.png)

## Intro

Wenn du DeFi (**De**centralize **Fi**nance)-Anwendungen verwendest, vor allem wenn du Yields farmst, hast du am Ende einen Haufen nativer Token, die von der Farm vergeben werden. Wenn die meisten Leute diese Token einfach verkaufen, um mehr oder ihre Lieblingsmünzen zu kaufen, werden wir versuchen, einige Möglichkeiten aufzuzeigen, wie du sie tatsächlich behalten und einsetzen kannst, um deine Einnahmen zu steigern.

Dazu nutzen wir die neuen LP-Pools (**L**iquiditätspools), die Anfang September 2021 auf QuickSwap gestartet sind und den Qi-Token von Mai Finance verwenden. Wenn du eine gute Vorstellung davon bekommen möchtest, was QuickSwap und Adamant-Anwendungen sind, lies bitte den [Stacking DApps guide](stack-dapps-like-lego-bricks.md).

## Anwendungen & Pools

### Farming&#x20;

Um unsere Gewinne zu maximieren, werden wir 3 verschiedene Anwendungen nutzen

* Mai Finance
* QuickSwap
* Adamant

Außerdem werden wir die folgenden LP-Pools nutzen

* Qi/MATIC auf Mai Finance, um Qi zu verdienen.
* Qi/WETH auf QuickSwap, um QUICK und ADDY zu verdienen.
* Qi/QUICK auf Adamant, um ADDY und MATIC zu verdienen.

Du kannst bereits sehen, dass jede Anwendung Token generiert, die die anderen Pools der anderen Anwendungen speisen können. Die Idee ist, die Qi-Token von Mai Finance mit den QUICK-Tokens von QuickSwap zu kombinieren und die beiden auf Adamant zu verwenden. Adamant wird ADDY-Token generieren, mit denen du MATIC-Dividenden einfordern kannst. Die MATIC-Token kannst du auf Mai Finance im WMATIC Vault sperren, um MAI zu leihen und dann MATIC und WETH zu kaufen, die du dann mit Qi-Token verwenden kannst, um deine Positionen auf Mai Finance und QuickSwap zu erhöhen.

### Staking&#x20;

Du musst auch wissen, dass Token, die bei Mai Finance und QuickSwap im Überschuss generiert werden, gestaked werden können:

* Qi auf Mai Finance **und** QuickSwap können verwendet werden, um über QIP (**Q**iDAO **I**Verbesserungsvorschläge **P**Vorschläge) abzustimmen.
* Qi auf Mai Finance können gesperrt werden. Wenn du deine Qis sperrst, bist du berechtigt, Dividenden zu erhalten, die in Qi gezahlt und jeden Mittwoch ausgeschüttet werden. Mehr Details zum Qi staken in Kürze.
* QUICK auf QuickSwap kann auch gestaked werden, um zusätzliche QUICK-Token in der Dragon's Lair zu generieren.
* Gesperrte QUICK (dQUICK) können auch auf QuickSwap eingesetzt werden, um weitere Token im Drachensirup zu generieren. Die Farm, die wir verwenden werden, generiert ADDY-Token.
* ADDY auf Adamant sind automatisch unverfallbar (für 90 Tage gesperrt), generieren aber WMATIC-Dividenden.
* ADDYs auf Adamant können auch gesperrt werden, um deine APRs/APYs (**A**nual **P**ercentage **R**ewards / **A**nual **P**ercentage **Y**ield) auf den Pools zu erhöhen, die du auf der Seite eingegeben hast, und um mehr ADDYs zu generieren und deine MATIC-Dividenden zu erhöhen.

## Lass uns das System starten

![](../../.gitbook/assets/screen-shot-2021-09-08-at-6.54.08-am.png)

Es folgt eine Simulation, die mit einer Anfangsinvestition von 1.000 US-Dollar in Qi/MATIC- und Qi/WETH-LP-Token und den aktuellen effektiven Jahreszinsen der verschiedenen Plattformen am 9. September 2021 erzeugt wurde. Dies ist keine reale Anwendung dessen, was wir oben beschrieben haben. Die Zinssätze werden schwanken, die Tokenpreise werden variieren, einige Programme werden auslaufen usw. Die Endergebnisse sind also nur eine Schätzung dessen, was du bekommen könntest, wenn alles stabil bliebe, was nie der Fall sein wird.

### Tag 1

{% hint style="info" %}
**Achtung:** Die Pools, die in diesem Leitfaden verwendet werden, wurden ein paar Stunden vor der Veröffentlichung live geschaltet. Die effektiven Jahreszinsen werden natürlich nicht unverändert bleiben, und in den nächsten Tagen werden wir einige Änderungen an dem Dokument erzeugen. Bitte sei vorsichtig und nimm den Leitfaden mit Vorsicht.
{% endhint %}

Da wir Qi/MATIC-LP-Token im Wert von 500 $ und Qi/WETH-LP-Token im Wert von 500 $ haben, werden wir sie auf Mai Finance und QuickSwap einzahlen. Nebenbei bemerkt: Wenn du Qi oder QuickSwap bevorzugst, kannst du einfach mehr LP-Token auf die eine oder andere Plattform legen, um mehr von deinem Lieblings-Token zu generieren und mehr zu staken. Für unser Beispiel halten wir uns an eine strikte Aufteilung von 50 %.

* 500 $ von Qi/MATIC werden auf Mai Finance mit einem APR von 1160,65% angelegt.
* 500 $ Qi/WETH werden bei QuickSwap mit einem effektiven Jahreszins von 1817,44% angelegt.

Für den Rest der Simulation werden wir die folgenden effektiven Jahreszinsen verwenden

* dQUICK APR von Dragon's Lair ist 17,28%
* ADDY APR von Dragon's Syrup beträgt 17,08%.
* Qi/QUICK APR auf Adamant für automatisch zusammengesetzte LP-Token beträgt 133%.
* Qi/QUICK APR von Adamant für ADDY-Token beträgt 131%.
* Der WMATIC APR bei Adamant beträgt 35% der gesperrten ADDY-Token

Da der effektive Jahreszins auf Mai Finance niedriger ist als auf QuickSwap, verwenden wir 100% der auf Mai Finance generierten Qi, um zusätzliche Qi/QUICK-Token zu generieren (nicht verkaufen, sondern mit den auf QuickSwap erhaltenen QUICK-Token kombinieren), was bedeutet, dass wir am Ende des Tages 0 Qi übrig haben. Wenn du deine anfängliche Investition anders aufrechnest, kannst du natürlich auch noch Qi und 0 QUICK übrig haben.

Am Ende von Tag 1 haben wir also in unserem Portfolio

| Belohnungstyp        | Wert in Dollar |
| -------------------- | -------------- |
| dQUICK auf QuickSwap | 8.997          |
| ADDY auf QuickSwap   | 0              |
| Qi/QUICK auf Adamant | 31.799         |
| ADDY auf Adamant     | 0              |
| WMATIC auf Adamant   | 0              |

### Tag 2

An Tag 2 beginnt der dQUICK, der auf QuickSwaps Drachensirup hinterlegt ist, ADDY-Token zu generieren, ebenso wie das Qi/QUICK LP-Paar auf Adamant. Am Ende von Tag 2 würden wir Folgendes erhalten

| Belohnungstyp        | Wert in Dollar |
| -------------------- | -------------- |
| dQUICK auf QuickSwap | 17.998         |
| ADDY auf QuickSwap   | 0.0042         |
| Qi/QUICK auf Adamant | 63.713         |
| ADDY auf Adamant     | 0.114          |
| WMATIC auf Adamant   | 0              |

Vergiss nicht, deine Belohnungen täglich auf Adamant einzufordern, um WMATIC-Dividenden zu erhalten!

### Tag 3

Am 3. Tag beginnen die auf Adamant gesammelten ADDY-Token, WMATIC-Dividenden zu generieren. Das bedeutet, dass wir am Ende von Tag 3 in unserem Portfolio Folgendes erhalten würden

| Belohnungstyp        | Werte in Dollar |
| -------------------- | --------------- |
| dQUICK auf QuickSwap | 27.004          |
| ADDY auf QuickSwap   | 0.025           |
| Qi/QUICK auf Adamant | 95.743          |
| ADDY auf Adamant     | 0.343           |
| WMATIC auf Adamant   | 0.0001          |

Ab dem 4. Tag werden wir in der Lage sein

* die WMATIC-Dividenden zu kassieren
* einen Teil der WMATIC auf Mai Finance einzuzahlen und MAI dafür zu leihen
* MAI zu verkaufen, um mehr WETH zu kaufen
* die verbleibende MATIC mit Qi und das WETH mit mehr Qi auf Mai Finance zu paaren
* das zusätzliche Qi/WMATIC-Paar auf Mai Finance und das Qi/WETH-Paar auf QuickSwap zu hinterlegen

Zu diesem Zeitpunkt ist das Farming-System vollständig vorbereitet, und wir können mit der Schätzung der Einnahmen beginnen.

## Farming-Ergebnisse

### Tägliche Routine



Der Tagesablauf setzt sich aus den folgenden Vorgängen zusammen

* Qi ernten auf Mai Finance
* WMATIC bei Adamant ernten
* Einzahlung von 66% der WMATIC bei Mai Finance
* Leih dir MAI für 50% der Einlage
* Tausche MAI gegen WETH
* Erstelle ein Qi/WMATIC-Paar auf QuickSwap
* Qi/WMATIC auf Mai Finance einzahlen
* Erstelle ein Qi/WETH-Paar bei QuickSwap
* Hinterlege Qi/WETH bei QuickSwap
* Quick ernten auf QuickSwap
* Erstelle ein Qi/QUICK-Paar bei QuickSwap
* Restliches QUICK auf Dragon's Lair einzahlen
* Lege dQUICK auf Dragon's Syrup ab
* ADDY-Münze aus Drachensirup ernten
* Sammle ADDY-Münzen von Adamant ein
* Neue Qi/QUICK auf Adamant einzahlen
* Geerntetes ADDY auf Adamant ablegen (sperren)

### Ergebnisse über mehrere Monate

| Monat | dQUICK    | Qi/QUICK   | ADDY       | Qi/MATIC  Qi/WETH |
| ----- | --------- | ---------- | ---------- | ----------------- |
| 1     | $280.96   | $1,040.78  | $54.97     | $0.91             |
| 2     | $557.79   | $2,162.98  | $224.36    | $7.89             |
| 3     | $842.08   | $3,413.73  | $521.09    | $27.85            |
| 4     | $1,138.60 | $4,816.62  | $960.17    | $68.48            |
| 5     | $1,454.30 | $6,405.18  | $1,559.60  | $138.44           |
| 6     | $1,798.77 | $8,224.86  | $2,341.64  | $247.49           |
| 7     | $2,184.58 | $10,335.38 | $3,334.13  | $406.84           |
| 8     | $2,627.76 | $12,813.60 | $4,572.23  | $629.47           |
| 9     | $3,148.40 | $15,757.01 | $6,100.39  | $930.60           |
| 10    | $3,771.42 | $19,288.05 | $7,974.83  | $1,328.32         |
| 11    | $4,527.47 | $23,559.40 | $10,266.47 | $1,844.31         |
| 12    | $5,454,16 | $28,760.60 | $13,064.51 | $2,504.79         |

### Tag 365

| Belohnungstyp                  | Wert in Dollar |
| ------------------------------ | -------------- |
| dQUICK auf QuickSwap           | 5,628.29       |
| ADDY auf QuickSwap             | 365.25         |
| Qi/QUICK auf Adamant           | 29,733.58      |
| ADDY auf Adamant               | 13,587.56      |
| Zusätzliche Qi/MATIC + Qi/WETH | 2,631.07       |

Beachte, dass die ADDY, die über die QuickSwap-Farm generiert wurden, in dieser Simulation nicht täglich geerntet und zur Erhöhung der ADDY-Belohnungen auf Adamant hinzugefügt wurden (es ist bereits komplex genug). Außerdem berücksichtigen wir nur unverfallbare ADDY. Wenn du nach der anfänglichen Sperrfrist von 90 Tagen die ADDY-Token einforderst und sperrst, werden deine ADDY-Belohnungen noch mehr steigen und du wirst mehr WMATIC generieren.

Nach einem Jahr sind die generierten Einnahmen schließlich 51.580,50 $ wert. Wenn wir davon ausgehen, dass die anfängliche Investition 1.000 $ in Qi/MATIC und Qi/WETH betrug, ergibt sich ein APY von 5.087,39 %.

## Haftungsausschluss

Dieser Leitfaden ist definitiv keine Finanzberatung, sondern wurde mit einem pädagogischen Ziel erzeugt. Du musst auf Preisschwankungen, Angebot und Nachfrage, Endtermine von Belohnungsprogrammen, impermanente Verluste usw. achten ... Das Ziel war nicht, Rezepte vorzuschlagen, die man blind befolgen kann. Mach also bitte deine Hausaufgaben und deine eigenen Simulationen und investiere nur so viel, wie du bereit bist, möglicherweise zu verlieren.

{% hint style="info" %}
Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geldverluste erzeugen) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
