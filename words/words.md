<div class="section">
    <div>
    	<iframe id="splash" width="960" height="480" src="banners/splash.html"></iframe>
        <div style="top: 70px;font-size: 75px;font-weight: bold;">
        	Wie geht es weiter?
       	</div>
		<div style="font-weight: 500;top: 140px;left: 10px;font-size: 29px;">
			Zukunftsszenarien von COVID-19: eine spielbare Simulation
		</div>
		<div style="font-weight: 100;top: 189px;left: 10px;font-size: 19px;line-height: 21px;">
			<b>
				🕐 Lese-/Spielzeit: 30 Min.
				&nbsp;&middot;&nbsp;
			</b>
			von 
			<a href="https://scholar.google.com/citations?user=_wHMGkUAAAAJ&amp;hl=en">Marcel Salathé</a>
			(Epidemiologe)
			&
			<a href="https://ncase.me/">Nicky Case</a>
			(Kunst/Code)
		</div>
	</div>
</div>

"Das Einzige, was man fürchten muss, ist die Angst selbst" (siehe Fußnote!→[^roosevelt]), war ein dummer Ratschlag.

[^roosevelt]: Die Fußnoten in dieser Simulation enthalten Quellen, Links oder zusätzliche Kommentare. Wie dieser erste Kommentar!

	"The only thing to fear is fear itself" ist ein Zitat Franklin D. Roosevelts aus der Rede zu seiner Amtseinführung 1933 in Zeiten der Weltwirtschaftskrise.

Sicher hortest du kein Toilettenpapier - aber wenn Politiker die Angst selbst fürchten, werden sie echte Gefahren herunterspielen, um eine "Massenpanik" zu vermeiden. Die Angst ist nicht das Problem, sondern die Art und Weise, wie wir unsere Angst *kanalisieren*. Angst gibt uns die Energie mit den jetzigen Gefahren umzugehen und uns auf kommende Gefahren vorzubereiten.

Wir (Marcel, Epidemiologe + Nicky, Kunst / Code) sind ehrlich gesagt auch besorgt. Und wir wetten, dass du es auch bist! Deshalb haben wir unsere Angst dazu genutzt, um diese **spielbaren Simulationen** zu erstellen. Unser Ziel ist, dass du nicht in Panik verharrst, sondern versuchst zu verstehen und zu lernen:

* **Über die letzten paar Monate** (1x1 der Epidemiologie, SEIR-Modell, R & R<sub>0</sub>)
* **Über die nächsten paar Monate** (Lockdown, Contact Tracing, Masken)
* **Über die nächsten paar Jahre** (Verlust der Immunität? Kein Impfstoff?)

Dieser Wegweiser (veröffentlicht am 1. Mai 2020[^timestamp]) soll dir zugleich Hoffnung geben und Angst machen. Denn um COVID-19 auf eine Weise zu schlagen, die auch **unsere geistige Gesundheit und unsere finanzielle Situation schützt**, brauchen wir zum einen Optimismus, um Pläne zu machen, zum anderen Pessimismus, um Backup-Pläne zu erstellen. Wie Gladys Bronwyn Stern einmal sagte: *"Der Optimist erfindet das Flugzeug und der Pessimist den Fallschirm."*

[^timestamp]: **Dieser Wegweiser wurde am 1. Mai 2020 publiziert.** Viele Details werden obsolet werden, aber wir sind zuversichtlich, dass er 95% aller möglichen zukünftigen Szenarien abdeckt, und dass das 1x1 der Epidemiologie ohne Verfallsdatum nützlich bleiben wird.

Also schnall dich an: Wir erwarten einige Turbulenzen. 

<div class="section chapter">
    <div>
		<img src="banners/curve.png" height=480 style="position: absolute;"/>
        <div>Die letzten paar Monate</div>
    </div>
</div>

Pilotinnen und Piloten trainieren mit Flugsimulatoren, um künftige Abstürze zu verhindern.

**Epidemiologinnen und Epidemiologen trainieren in Epidemiesimulatoren, den Absturz der Menschheit zu verhindern.**

Also, nehmen wir uns einen sehr, *sehr* einfachen "Epidemie-Flugsimulator"! In dieser Simulation können <icon i></icon> ansteckende Menschen <icon s></icon> ungeschütze Menschen in <icon i></icon> ansteckende Menschen verwandeln:

![](pics/spread.png)

Es wird angenommen, dass *zu Beginn* eines COVID-19-Ausbruchs das Virus *im Durchschnitt* alle 4 Tage von einem <icon i></icon> ansteckenden Menschen zu einem <icon s></icon> ungeschützten Menschen springt.[^serial_interval] (bedenke, dass es viele Variationen gibt)

[^serial_interval]: "Das mittlere \[serielle\] Intervall war 3.96 Tage (95% CI 3.53–4.39 Tage)" (“The mean [serial] interval was 3.96 days (95% CI 3.53–4.39 days)”) [Du Z, Xu X, Wu Y, Wang L, Cowling BJ, Ancel Meyers L](https://wwwnc.cdc.gov/eid/article/26/6/20-0357_article) (Hinweis: Vorabveröffentlichungen können nicht als endgültige Version von Artikeln angesehen werden)

Wenn wir "eine Verdoppelung alle 4 Tage", bei einer Bevölkerung, die mit nur 0,001 % <icon i></icon> beginnt, und *nichts anderes* simulieren was passiert dann?

**Klicke auf Start, um die Simulation zu starten! Später kannst du sie mit verschiedenen Einstellungen erneut starten:** (technische Vorbehalte: [^caveats])

[^caveats]: **Beachte: alle diese Simulationen sind für Ausbildungszwecke sehr vereinfacht.**
    
    Eine Vereinfachung: Wenn man bei dieser Simulation folgendes einstellt: "Alle X Tage einen neuen Menschen infizieren", steigt die Zahl der Infizierten tatsächlich um 1/X pro Tag. Dasselbe gilt für zukünftige Einstellungen in diesen Simulationen - "Alle X Tage erholen" bedeutet tatsächlich, dass die Zahl der Infizierten jeden Tag um 1/X abnimmt.
    
    Diese sind *nicht* identisch, aber ähnlich genug und zu Lernzwecken ist es leichter zu durchschauen als die direkte Festlegung der Übertragungs-/Wiederherstellungsraten.

<div class="sim">
		<iframe src="sim?stage=epi-1" width="800" height="540"></iframe>
</div>

Dies ist die **exponentielle Wachstumskurve.** Sie fängt klein an und explodiert dann. Von "Ach, es ist nur eine Grippe" bis "Oh richtig, eine Grippe schafft keine *Massengräber in reichen Städten*". 

![](pics/exponential.png)

Diese Simulation ist aber falsch. Exponentielles Wachstum kann glücklicherweise nicht ewig anhalten. Die Ausbreitung eines Virus wird zum Beispiel dadurch gestoppt, dass andere es *bereits* haben:

![](pics/susceptibles.png)

Je mehr <icon i></icon> es gibt, desto schneller werden <icon s></icon> zu <icon i></icon>, **aber je weniger <icon s></icon> es gibt, desto *langsamer* werden <icon s></icon> zu <icon i></icon>.**

Wie verändert dies das Wachstum einer Epidemie? Lass es uns herausfinden:

<div class="sim">
		<iframe src="sim?stage=epi-2" width="800" height="540"></iframe>
</div>

Dies ist eine "S-förmige" **logistische Wachstumskurve.** Sie fängt klein an, explodiert und verlangsamt sich dann wieder.

Aber auch diese Simulation ist *immer noch* falsch. Wir übersehen die Tatsache, dass <icon i></icon> ansteckende Menschen schließlich aufhören, ansteckend zu sein, entweder indem sie 1) sich erholen, 2) sich mit Lungenschäden "erholen" oder 3) sterben.

Der Einfachheit halber wollen wir so tun, als ob alle <icon i></icon> ansteckenden Menschen wieder genesen <icon r></icon> würden. (Denkt aber daran, dass in Wirklichkeit einige von ihnen sterben.) <icon r></icon> können nicht wieder infiziert werden, lasst uns - *vorläufig!* - so tun, als ob sie ein Leben lang immun bleiben.

Es wird angenommen, dass Personen mit COVID-19 *im Durchschnitt* 10 Tage lang ansteckend sind.[^infectiousness] Das bedeutet, dass manche <icon i></icon> Menschen sich früher als nach 10 Tagen erholen, andere später. **So sieht das bei einer Simulation aus, die mit 100 % <icon i></icon> *beginnt*:**

[^infectiousness]: “Der Median der Zeitspanne, in der Infizierte ansteckend waren \[...\] war 9.5 Tage.” (“The median communicable period \[...\] was 9.5 days.”) [Hu, Z., Song, C., Xu, C. et al](https://link.springer.com/article/10.1007/s11427-020-1661-4) Ja, wir wissen, dass "Median" und "Durchschnitt" nicht das Gleiche sind. Für didaktische Zwecke sind sie aber ähnlich genug.

<div class="sim">
		<iframe src="sim?stage=epi-3" width="800" height="540"></iframe>
</div>

Dies ist das Gegenteil von exponentiellem Wachstum, die **exponentielle Zerfallskurve.**

Nun, was passiert, wenn wir S-förmiges logistisches Wachstum *mit* Erholung simulieren?

![](pics/graphs_q.png)

Lass es uns herausfinden:

die <b style='color:#ff4040'>Rote Kurve</b> gibt die *aktuellen* Fälle <icon i></icon> wieder,    
die <b style='color:#999999'>Graue Kurve</b> gibt die *gesamten* Fälle (aktuelle + genesene) wieder <icon r></icon>) und
beginnt bei nur 0,001 %. <icon i></icon>:

<div class="sim">
		<iframe src="sim?stage=epi-4" width="800" height="540"></iframe>
</div>

Und *so* kommt diese berühmte Kurve zustande! Es ist keine Glockenkurve, es ist nicht einmal eine "log-normale" Kurve. Sie hat keinen Namen. Aber du hast sie schon zigmal gesehen und wurdest inständig gebeten, sie abzuflachen.

Das hier ist das **SIR-Modell**,[^sir]    
(<icon s></icon> **S**usceptible *anfällig/ungeschützt* <icon i></icon> **I**nfectious *ansteckend/infektiös* <icon r></icon> **R**ecovered *erholt/genesen*),      
die *zweit*-wichtigste Idee im 1x1 der Epidemiologie:

[^sir]: Für weitere technische Erläuterungen zum SIR-Modell, siehe [the Institute for Disease Modeling](https://www.idmod.org/docs/hiv/model-sir.html#) und [Wikipedia](https://de.wikipedia.org/wiki/SIR-Modell)

![](pics/sir.png)

**ANMERKUNG: Die Simulationen, auf deren Basis die Politik entscheidet, sind *wesentlich* ausgefeilter als das hier!** Das SIR-Modell kann aber trotzem die gleichen allgemeinen Ergebnisse erklären, auch wenn die Nuancen fehlen.

Eigentlich sollten wir noch eine weitere Nuance hinzufügen: Bevor ein <icon s></icon> zu einem <icon i></icon> wird, wird es zunächst <icon e></icon> exponiert. Das ist, wenn sie oder er das Virus bereits hat, es aber noch nicht weitergeben kann - *infiziert*, aber noch nicht *infektiös*.

![](pics/seir.png)

(Diese Variante wird das **SEIR-Modell**[^seir] genannt, wobei das "E" für <Icon e></icon> **E**xposed (*exponiert*) steht. Bitte beachte, dass dies *nicht* die Alltagsbedeutung von "exponiert" ist, welche da wäre: Man kann das Virus haben oder nicht. In dieser technischen Definition bedeutet "exponiert", dass man das Virus definitiv hat. Wissenschaftliche Terminologie ist eine schwierige Sache).

[^seir]: Weitere technische Erläuterungen zum SEIR-Modell findest du unter [the Institute for Disease Modeling](https://www.idmod.org/docs/hiv/model-seir.html) und [Wikipedia](https://de.wikipedia.org/wiki/SEIR-Modell)

Für COVID-19 wird angenommen, dass <icon e></icon> 3 Tage lang infiziert, aber noch nicht infektiös ist, *im Durchschnitt*. [^latent] Was passiert, wenn wir das zur Simulation hinzufügen?

[^latent]: “Ausgehend von einer Verteilung der Inkubationszeitspanne von im Mittel über 5,2 Tage aus einer anderen Studie über frühe COVID-19 Fälle schlossen wir, dass die Ansteckungsfähigkeit 2,3 Tage (95% CI, 0,8–3,0 Tage) vor dem Auftreten von Symptomen auftrat.” Übersetzung: Angenommen die Symptome fangen am 5. Tag an, dann fängt die Ansteckungsfähigkeit 2 Tage davor an (also am 3. Tag). (“Assuming an incubation period distribution of mean 5.2 days from a separate study of early COVID-19 cases, we inferred that infectiousness started from 2.3 days (95% CI, 0.8–3.0 days) before symptom onset”) [He, X., Lau, E.H.Y., Wu, P. et al.](https://www.nature.com/articles/s41591-020-0869-5)

Die <b style='color:#ff4040'>Rote <b style='color:#FF9393'>+ Pinke</b> Kurve</b> geben die *aktuellen* Fälle (infektiös <icon i></icon> + exponiert <icon e></icon>) wieder,    
die <b style='color:#888'>Graue Kurve</b> gibt die *gesamten* Fälle (aktuell + genesen <icon r></icon>) wieder:

<div class="sim">
		<iframe src="sim?stage=epi-5" width="800" height="540"></iframe>
</div>

Es ändert sich nicht viel! Wie lange ein <icon e></icon> exponiert bleibt, ändert zwar das Verhältnis von <icon e></icon> zu <icon i></icon> und *wann* die aktuellen Fälle ihren Höhepunkt erreichen... aber die *Höhe* dieser Spitze und die Gesamtzahl der Fälle bleibt am Ende gleich.

Warum das? Wegen der *wichtigsten* Idee im 1x1 der Epidemiologie:

![](pics/r.png)

Kurz für Reproduktionszahl. Sie beschreibt die *durchschnittliche* Anzahl an Menschen, die ein <icon i></icon> infiziert *bevor* er sich erholt (oder stirbt).

![](pics/r2.png)

**R** verändert sich im Laufe des Ausbruchsgeschehens durch gesteigerte Immunität und Maßnahmen. 

**R<sub>0</sub>** (gesprochen R-Null, auch "Basisreproduktionszahl") ist die Reproduktionszahl zu *Beginn eines Ausbruchs, also vor einer Immunität und vor Interventionen*. R<sub>0</sub> spiegelt damit die Stärke des Virus wider, jedoch schwankt diese Zahl von Ort zu Ort. Beispielsweise ist sie in dicht besiedelten Städten höher als in ländlichen Gegenden. 

(Die meisten Zeitungsartikel - und teilweise sogar wissenschaftliche Veröffentlichungen! - verwechseln R und R<sub>0</sub>. Wie gesagt - wissenschaftliche Terminologie ist ein schwieriges Feld.)

Die Basisreproduktionszahl R<sub>0</sub> der saisonalen Grippe liegt bei ungefähr 1,28[^r0_flu]. Das bedeutet, dass zu Beginn eines Grippeausbruchs jeder <icon i></icon> *im Durchschnitt* 1,28 andere ansteckt. (Falls du dich wunderst, dass 1,28 keine ganze Zahl ist: Eine "durchschnittliche" Mutter hat 2,4 Kinder. Das bedeutet ja auch nicht, dass irgendwo halbe Kinder herumlaufen.)

[^r0_flu]: “Der Median des R-Werts der saisonalen Grippe lag bei 1,28 (IQR: 1,19–1,37)” (übersetzt): “The median R value for seasonal influenza was 1.28 (IQR: 1.19–1.37)” [Biggerstaff, M., Cauchemez, S., Reed, C. et al.](https://bmcinfectdis.biomedcentral.com/articles/10.1186/1471-2334-14-480)

Der R<sub>0</sub>-Wert für COVID-19 wird auf etwa 2,2 geschätzt[^r0_covid], obwohl es eine *noch nicht fertiggestellte* Studie gibt, die einen Wert von 5,7(!) für Wuhan schätzt.[^r0_wuhan]

[^r0_covid]: “Wir schätzen die Basisreproduktionszahl R<sub>0</sub> von 2019-nCoV auf etwa 2,2 (übersetzt):“We estimated the basic reproduction number R0 of 2019-nCoV to be around 2.2 (90% high density interval: 1.4–3.8)”  [Riou J, Althaus CL.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7001239/)

[^r0_wuhan]: “wir berechneten den Median des R0-Werts als 5,7 (95% CI 3,8–8,9)” (übersetzt): “we calculated a median R0 value of 5.7 (95% CI 3.8–8.9)” [Sanche S, Lin YT, Xu C, Romero-Severson E, Hengartner N, Ke R.](https://wwwnc.cdc.gov/eid/article/26/7/20-0282_article)

In unseren Simulationen infiziert - *zu Beginn und durchschnittlich* - ein <icon i></icon> im Laufe von 10 Tagen alle 4 Tage eine andere Person. Das Verhältnis 10 zu 4 Tage beträgt genau 2,5, das heißt, dass - *zu Beginn und durchschnittlich* - jede und jeder <icon i></icon> 2,5 weitere Personen infiziert. Es gilt hier also R<sub>0</sub> = 2,5. (Vorbehalte:[^r0_caveats_sim])


[^r0_caveats_sim]: Wir nehmen hier an, dass man in seiner "infektiösen Phase" immer gleichbleibend infektiös ist. Auch hier wurden die Vereinfachungen zum besseren Verständnis gemacht. 

**Spiele an R<sub>0</sub> im Rechner unten, um zu sehen, wie R<sub>0</sub> von der Genesungszeit und der Neuinfektionsrate abhängt:**

<div class="sim">
		<iframe src="sim?stage=epi-6a&format=calc" width="285" height="255"></iframe>
</div>

Zur Erinnerung: je weniger <icon s></icon> es gibt, desto *langsamer* werden <icon s></icon> zu <icon i></icon>. Die *aktuelle* Reproduktionszahl R hängt nicht nur von der *Basisreproduktionszahl* (R<sub>0</sub>) ab, sondern auch von der Anzahl der potentiell infizierbaren Menschen. (Beispielsweise durch Genesung und natürliche Immunität.)

<div class="sim">
		<iframe src="sim?stage=epi-6b&format=calc" width="285" height="390"></iframe>
</div>

Sobald genügend Menschen eine Immunität erworben haben und R < 1 ist, hat man das Virus im Griff. Dies nennt man *Herdenimmunität*. 
Für Grippeviren wird Herdenimmunität mittels eines *Impfstoffs* erreicht. Die Idee, "natürliche Herdenimmunität" durch gezielte Infizierungen zu erreichen ist denkbar schlecht! (Aber nicht aus dem Grund, den du vielleicht annimmst - wir werden das später erklären!)

Lass uns jetzt das SEIR-Modell betrachten, das nun R<sub>0</sub> zeigt, R über die Zeit, sowie den Schwellenwert der Herdenimmunität zeigt: 

<div class="sim">
		<iframe src="sim?stage=epi-7" width="800" height="540"></iframe>
</div>

**HINWEIS: Die Gesamtzahl der Infizierten *stoppt nicht* an der Grenze der Herdenimmunität, sondern geht darüber hinaus!** Zudem überschreitet die Gesamtzahl der Infizierten den Schwellenwert der Herdenimmunität *genau* zum Zeitpunkt der höchsten aktuellen Fallzahl. (Dies ist unabhängig von der Wahl der Parameter - teste es selbst!) 

Warum ist das so? Wenn es mehr Nicht-<icon s></icon> als die Schwelle der Herdenimmunität gibt, so wird R < 1. Und wenn R < 1 ist, stoppt das Wachstum neuer Fälle: ein Hochpunkt ist erreicht. 

**Wenn du dir nur eine Sache aus dieser Anleitung merken solltest, dann die folgende** - es ist ein extrem komplexes Diagramm, also nimm dir Zeit, um es zu verinnerlichen: 

![](pics/r3.png)


**Es bedeutet: Wir müssen NICHT alle Übertragungen abfangen, auch nicht fast alle, um COVID-19 zu stoppen!**

Dies scheint paradox! COVID-19 ist eine extrem ansteckende Krankheit, jedoch reicht es aus, "nur" mehr als 60% der Infektionen zu verhindern, um sie einzudämmen. 60%?! Als Schulnote wäre das "befriedigend". Aber wenn R<sub>0</sub> = 2,5 und man 61% davon abzieht, erhält man R = 0,975. Da dann R < 1 ist, wäre das Virus eingedämmt! (exakte Formel: [^exact_formula])) 

[^exact_formula]: Zur Erinnerung R = R<sub>0</sub> * Anteil der zugelassenen Übertragungen. Dabei ist der Anteil der zugelassenen Übertragungen = 1 - Anteil der *vereitelten* Übertragungen.

    Um dann R < 1 zu erhalten, muss R<sub>0</sub> * ZugelasseneInfektionen < 1. 
    
    Also, ZugelasseneInfektionen < 1/R<sub>0</sub>
    
    Also, 1 - VereitelteInfektionen < 1/R<sub>0</sub>
    
    Therefore, VereitelteInfektionen > 1 - 1/R<sub>0</sub>
    
    Also müssen mehr als **1-1/R<sub>0</sub>** der Übertragungen vereitelt werden, um  R < 1 zu erreichen und das Virus einzudämmen!

![](pics/r4.png)

(Falls du glaubst, dass R<sub>0</sub> oder einige der anderen Zahlen unserer Simulationen zu klein oder groß sind - super! Damit hinterfragst du unsere Annahmen. Am Ende gibt es einen "Sandkasten-Modus", bei dem du deine *eigenen* Zahlen auswählen und simulieren kannst, was dann passiert.)

*Jede* COVID-19 Maßnahme, von der du gehört hast - sei es Händewaschen, Abstand halten, "Lockdown", Selbstisolationen, "Contact Tracing", Quarantäne, Gesichtsmasken oder Herdenimmunität - machen *alle* das selbe: 

Sie sollen erreichen, dass R < 1 wird. 

**Starten wir nun unseren "epidemischen Flugsimulator", um folgende Frage beantworten zu können: Wie erreichen wir unter Berücksichtigung unserer Gesundheit und finanziellen Interessen, dass R < 1 wird?**

Bereite dich auf eine Notlandung vor... 

<div class="section chapter">
    <div>
		<img src="banners/curve.png" height=480 style="position: absolute;"/>
        <div>Die nächsten paar Monate</div>
    </div>
</div>

... hätten deutlich schlimmer sein können. Hier ist ein Paralleluniversum, das wir vermieden haben:

###Szenario 0: Überhaupt nichts tun

Etwa 1 von 20 Menschen, die sich mit COVID-19 infiziert haben, benötigen eine intensivmedizinische Behandlung.[^icu_covid] In einem reichen Land wie den USA steht ein Intensivplatz pro 3.400 Menschen zur Verfügung.[^icu_us] Daher können die USA damit umgehen, dass 20 von 3400 Menschen *gleichzeitig* infiziert sind - oder 0,6% der Bevölkerung.

[^icu_covid]: [Prozentualer Anteil der COVID-19-Fälle in den USA vom 12. Februar bis 16. März 2020, die eine intensivmedizinische Behandlung benötigten, nach Altersgruppe](https://www.statista.com/statistics/1105420/covid-icu-admission-rates-us-by-age-group/)(übersetzt):"Percentage of COVID-19 cases in the United States from February 12 to March 16, 2020 that required intensive care unit (ICU) admission, by age group". Zwischen 4,9 % und 11,5 % *aller* COVID-19-Fälle benötigten eine intensivmedizinische Behandlung. Wenn man die unterste Schätzung wählt, sind das 5 % oder 1 von 20. Diese Gesamtzahl ist spezifisch für die Altersstruktur der USA. In Ländern mit älterer Bevölkerung wird sie höher und in Ländern mit jüngerer Bevölkerung niedriger sein.

[^icu_us]: Anzahl der Betten auf der Intensivstation = 96.596. Von [der _Society of Critical Care Medicine_ (Gesellschaft für Intensivmedizin)](https://sccm.org/Blog/March-2020/United-States-Resource-Availability-for-COVID-19) Die Bevölkerung der USA betrug im Jahr 2019 rund 328.200.000 Personen. 96.596 von 328.200.000 macht ungefähr 1 von 3400.  

Selbst wenn wir diese Kapazität auf 2% *mehr als verdreifacht* hätten, wäre Folgendes passiert, *wenn wir absolut nichts getan hätten:*

<div class="sim">
		<iframe src="sim?stage=int-1&format=lines" width="800" height="540"></iframe>
</div>

Gar nicht gut.

Eben das hat [der Bericht des Imperial College vom 16. März](http://www.imperial.ac.uk/mrc-global-infectious-disease-analysis/covid-19/report-9-impact-of-npis-on-covid-19/) herausgefunden: Wenn wir nichts tun, gehen uns die Betten auf den Intensivstationen aus und mehr als 80% der Bevölkerung werden infiziert. 
(zur Erinnerung: die Gesamtzahl der Fälle *überschreitet* die Herdenimmunität)

Selbst wenn nur 0,5% der Infizierten sterben - eine sehr optimistische Annahme, wenn es keine Betten auf Intensivstationen mehr gibt - dann sterben in einem großen Land wie den USA mit 300 Millionen Menschen 0,5% von 80% der 300 Millionen. Also immer noch 1,2 Millionen Menschen ... *FALLS wir nichts tun*.

(In vielen Nachrichten und sozialen Medien wurde berichtet: "80% werden infiziert" *ohne* den Beisatz "FALLS WIR NICHTS TUN". Die Angst kanalisierte sich auf diese Weise in Klicks, nicht in Verständnis. *Seufz.*)

###Szenario 1: "Flatten the Curve" / Herdenimmunität

Der Plan "Flatten The Curve" (Abflachen der Kurve) wurde von allen Gesundheitsorganisationen angepriesen, während der ursprüngliche britische Plan der "Herdenimmunität" allgemein ausgepfiffen wurde. Allerdings handelte es sich dabei eigentlich um *denselben Plan.* Großbritannien kommunizierte ihn nur schlecht.[^yong]

[^yong]: Übersetztes Zitat: Er sagt, dass das eigentliche Ziel dasselbe ist wie in anderen Ländern: die Kurve abflachen, indem der Ausbruch von Infektionen zeitlich versetzt wird. Als Folge davon kann die Nation Herdenimmunität erreichen; das ist ein Nebeneffekt, kein Ziel. [...] Der aktuelle Coronavirus-Aktionsplan der Regierung, der online verfügbar ist, erwähnt die Herdenimmunität überhaupt nicht. (Aus einem [The Atlantic-Artikel von Ed Yong](https://www.theatlantic.com/health/archive/2020/03/coronavirus-pandemic-herd-immunity-uk-boris-johnson/608065/)) (übersetzt):“He says that the actual goal is the same as that of other countries: flatten the curve by staggering the onset of infections. As a consequence, the nation may achieve herd immunity; it’s a side effect, not an aim. [...] The government’s actual coronavirus action plan, available online, doesn’t mention herd immunity at all.” From a The Atlantic article by Ed Yong

Beide Pläne hatten jedoch einen fatalen Fehler.

Betrachten wir zunächst die beiden Hauptmöglichkeiten, mit denen sich die Kurve abflachen lässt: Händewaschen und soziale Distanzierung.

Durch vermehrtes Händewaschen werden Grippen und Erkältungskrankeiten in Ländern mit hohem Einkommen um ~25%[^handwashing] reduziert, während die stadtweite Abriegelung in London enge Kontakte um ~70%[^london] einschränkt. Nehmen wir also an, durch Händewaschen kann R um *bis zu* 25% reduziert werden und durch Distanzierung kann R um *bis zu* 70% reduziert werden:

[^handwashing]: Alle acht in Frage kommenden Studien berichteten, dass das Händewaschen das Risiko einer Atemwegsinfektion senkt, wobei die Risikominderung zwischen 6% und 44% liegt. Gepoolter Wert 24% (95% CI 6-40%). (Der Einfachheit halber haben wir in diesen Simulationen den gepoolten Wert auf 25% aufgerundet.) [Rabie, T. und Curtis, V.](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1365-3156.2006.01568.x) Anmerkung: Wie diese Meta-Analyse aufzeigt, ist die Qualität der Studien zum Händewaschen (zumindest in Ländern mit hohem Einkommen) miserabel.

[^london]: Wir fanden eine 73%ige Verringerung der durchschnittlichen täglichen Anzahl der beobachteten Kontakte pro Teilnehmer. Dies würde ausreichen, um R<sub>0</sub> von einem Wert von 2,6 vor dem Lockdown auf 0,62 (0,37 - 0,89) während des Lockdowns zu reduzieren. (Der Einfachheit halber haben wir in diesen Simulationen auf 70% abgerundet.) [Jarvis und Zandvoort et al](https://cmmid.github.io/topics/covid19/comix-impact-of-physical-distance-measures-on-transmission-in-the-UK.html)

**Probiere mit diesem Rechner aus, um mit unterschiedlichen % von Nicht-<icon s></icon> zu sehen, wie Händewaschen und Distanzierung R reduzieren:** (dieser Rechner visualisiert ihre *relativen* Effekte, weshalb die Erhöhung des einen Merkmals so *aussieht*, als ob es die Wirkung des anderen verringert.[^log_caveat])

[^log_caveat]: Diese Verzerrung würde verschwinden, wenn wir R auf einer logarithmischen Skala auftragen würden... aber dann müssten wir *logarithmische Skalen* erklären

<div class="sim">
		<iframe src="sim?stage=int-2a&format=calc" width="285" height="260"></iframe>
</div>

Lass uns nun simulieren, was mit einer COVID-19-Epidemie passiert, wenn wir ab März 2020 das Händewaschen verstärkt hätten, aber nur *wenig* Abstand gehalten hätten - so dass R niedriger, aber immer noch größer als 1 ist:

<div class="sim">
		<iframe src="sim?stage=int-2&format=lines" width="800" height="540"></iframe>
</div>

Drei Anmerkungen:

1. Dies *verringert* die Gesamtzahl der Fälle! **Selbst wenn R < 1 nicht erreicht wird, rettet die Reduzierung von R immer noch Leben, indem sie den 'Überschuss' bis zur Herdenimmunität reduziert.** Viele Menschen denken, dass mit dem Abflachen der Kurve die Fälle zeitlich gestreckt werden, ohne aber die Gesamtzahl zu reduzieren. Doch das steht im Widerspruch zu *jedem* grundlegenden Epidemiologie-Modell. Aber weil in den Nachrichten "80%+ werden infiziert" als unvermeidlich dargestellt wurde, kam es zu der weitläufigen Annahme, dass die Gesamtzahl der Fälle in jedem Fall gleich bleiben würde. *Seufz.*

2. Aufgrund der zusätzlichen Maßnahmen erreichen die aktuellen Fallzahlen ihren Höhepunkt *bevor* die Herdenimmunität erreicht wird. Tatsächlich schießt in dieser Simulation die Gesamtzahl der Fälle nur *ein kleines bisschen* über die Herdenimmunität hinaus - der Plan des Vereinigten Königreichs! An diesem Punkt, R < 1, kann man alle anderen Maßnahmen loslassen, und COVID-19 bleibt eingedämmt! Es gibt nur ein Problem ...

3. Es fehlen die Betten auf den Intensivstationen. Und das über mehrere Monate. (und dabei haben wir die Betten auf den Intensivstationen für diese Simulation ja *bereits verdreifacht*)

Das war das andere Ergebnis des Imperial-College-Berichts vom 16. März, der Großbritannien davon überzeugte, seinen ursprünglichen Plan aufzugeben. Jeder Versuch einer **Abschwächung** (R reduzieren, aber R > 1) wird scheitern. Der einzige Ausweg ist **Eindämmung** (R reduzieren, so dass R < 1).
![](pics/mitigation_vs_suppression.png)

Das heißt: Es reicht nicht, die Kurve einfach "abzuflachen". Die Kurve muss *zerstampft* werden. Zum Beispiel mit ...

###Szenario 2: Monatelanger Lockdown

Mal sehen, was passiert, wenn wir die Kurve mit einen 5-monatigen Lockdown *drücken*, die <icon i></icon> auf fast null reduzieren und dann endlich – *endlich* – wieder zu unserem normalen Leben zurückkehren:

<div class="sim">
		<iframe src="sim?stage=int-3&format=lines" width="800" height="540"></iframe>
</div>

Oh.

Das ist die "zweite Welle", über die alle sprechen. Sobald wir den Lockdown aufheben, erhalten wir wieder R > 1. Ein einzelner verbliebener <icon i></icon> (oder ein importierter <icon i></icon>) kann also einen Ausschlag der Fallzahlen verursachen, der fast so schlimm ist, als hätten wir Szenario 0 verfolgt: Absolut nichts getan.

**Ein Lockdown ist keine Heilung, es ist nur ein Neustart.**

Was also tun? Einen Lockdown nach dem anderen?

###Szenario 3: Periodischer Lockdown

Diese Option wurde zuerst im Bericht des Imperial College vom 16. März und später erneut in einem Harvard-Papier vorgeschlagen [^lockdown_harvard].

[^lockdown_harvard]: In Abwesenheit anderer Maßnahmen ist eine Schlüsselmetrik für den Erfolg der sozialen Distanzierung, ob die Kapazitäten der Intensivstationen überschritten werden. Um dies zu vermeiden, kann eine längere oder periodische räumliche Distanzierung bis ins Jahr 2022 erforderlich sein. (übersetzt): “Absent other interventions, a key metric for the success of social distancing is whether critical care capacities are exceeded. To avoid this, prolonged or intermittent social distancing may be necessary into 2022.” [Kissler und Tedijanto et al] (https://science.sciencemag.org/content/early/2020/04/14/science.abb5793)

**Hier ist eine Simulation für diese Option:** (Spiele zunächst die Aufzeichnung ab. Danach kannst du versuchen, deinen *eigenen* Lockdown-Plan zu simulieren, indem du den Schieberegler änderst *während* die Simulation läuft! Du kannst dabei die Simulation unterbrechen, fortsetzen und die Simulationsgeschwindigkeit ändern)

<div class="sim">
		<iframe src="sim?stage=int-4&format=lines" width="800" height="540"></iframe>
</div>

Dies *würde* die Fallzahlen unter der Kapazität der Intensivstationen halten! Und es ist *viel* besser als ein 18-monatiger Lockdown, bis ein Impfstoff zur Verfügung steht. Wir müssten also nur... für ein paar Monate einen Lockdown machen, für ein paar Monate öffnen und das so lange wiederholen, bis ein Impfstoff verfügbar ist. (Und wenn es keinen Impfstoff gibt, wiederholen wir es, bis die Herdenimmunität erreicht ist... im Jahr 2022).

Es scheint zunächst sinnvoll, solch einen Plan anhand der Kapazitäten der Intensivstationen zu machen, aber dabei übersehen wir zahlreiche wesentliche Dinge, die wir hier *nicht* simulieren können. Zum Beispiel:

**Psychische Gesundheit:** Einsamkeit ist einer der größten Risikofaktoren für Depressionen, Angstzustände und Selbstmord. Und sie führt statistisch gesehen genauso häufig zu einem frühen Tod, wie das Rauchen von 15 Zigaretten am Tag [^loneliness].

[^loneliness]: Siehe [Abbildung 6 aus Holt-Lunstad & Smith 2010](https://journals.sagepub.com/doi/abs/10.1177/1745691614568352). Natürlich müssen wir einschränkend darauf hinweisen, dass sie lediglich eine *Korrelation* gefunden haben. Aber so lange wir nicht nach dem Zufallsprinzip für einzelne Menschen lebenslange Einsamkeit anordnen wollen, müssen wir für unsere Annahmen auf solche Beobachtungen zurückgreifen.

**Wirtschaftliche Aspekte:** Die Frage nach der Wirtschaft klingt so, als ob man sich mehr ums Geld als um das Leben kümmert, aber "die Wirtschaft" besteht nicht nur aus Aktien: Es geht um die Fähigkeit der Menschen, sich um ihre Liebsten zu kümmern, in die Zukunft ihrer Kinder zu investieren und Kunst, Essen und Videospiele zu genießen. All das also, was das Leben lebenswert macht. Dazu kommt, dass Armut *an sich* gravierende Auswirkungen auf die geistige und körperliche Gesundheit hat.

Dies ist kein Plädoyer gegen erneute Lockdowns! Wir werden uns später mit möglichen Vorgehensweisen dazu befassen. Trotzdem ist es nicht ideal.

Warte mal... haben Taiwan und Südkorea nicht *bereits* COVID-19 in den Griff bekommen? Für vier ganze Monate und *ohne* längerfristige Lockdowns?

Wie ist das möglich?

###Szenario 4: Testen, Verfolgen, Isolieren

"*Sicherlich *hätten* wir das tun können, was Taiwan und Südkorea am Anfang getan haben. Aber dazu ist es jetzt zu spät. Wir haben den Anfang verpasst."*

Doch genau das ist es! "Ein Lockdown ist keine Heilung, es ist nur ein Neustart"... **und ein Neustart ist das, was wir brauchen.**

Um zu verstehen, wie Taiwan und Südkorea COVID-19 in den Griff bekommen haben, müssen wir den genauen zeitlichen Ablauf einer typischen COVID-19-Infektion verstehen[^timeline]:

[^timeline]: **durchschnittlich 3 Tage bis eine Person infektiös wird:** "Unter der Annahme einer Verteilung der Inkubationszeit von durchschnittlich 5,2 Tagen aus einer separaten Studie über frühe COVID-19-Fälle folgerten wir, dass die Ansteckung 2,3 Tage (95% CI, 0,8-3,0 Tage) vor Symptombeginn lag" (Übersetzung: "Assuming an incubation period distribution of mean 5.2 days from a separate study of early COVID-19 cases, we inferred that infectiousness started from 2.3 days (95% CI, 0.8–3.0 days) before symptom onset") (Das bedeutet: Wenn die Symptome nach 5 Tagen beginnen, ist man schon 2 Tage vorher ansteckend = Ansteckungsgefahr 3 Tage nach der Ansteckung) [He, X., Lau, E.H.Y., Wu, P. et al.] (https://www.nature.com/articles/s41591-020-0869-5)
    
    ** durchschnittlich 4 Tage bis zur Ansteckung einer anderen Person:** "Das durchschnittliche [serielle] Intervall betrug 3,96 Tage (95% CI 3,53-4,39 Tage)" [Du Z, Xu X, Wu Y, Wang L, Cowling BJ, Ancel Meyers L](https://wwwnc.cdc.gov/eid/article/26/6/20-0357_article)
 
     ** durchschnittlich 5 Tage bis zum Auftreten von Symptomen:** "Die mediane Inkubationszeit wurde auf 5,1 Tage geschätzt (95% CI, 4,5 bis 5,8 Tage)" [Lauer SA, Grantz KH, Bi Q, et al](https://annals.org/AIM/FULLARTICLE/2762808/INCUBATION-PERIOD-CORONAVIRUS-DISEASE-2019-COVID-19-FROM-PUBLICLY-REPORTED)

![](pics/timeline1.png)

Wenn sich die Personen erst dann selbst isolieren, wenn sie wissen, dass sie krank sind (d.h. wenn sie Symptome spüren), kann sich das Virus trotzdem ausbreiten:

![](pics/timeline2.png)

Und in der Tat verlaufen 44% aller Übertragungen so: Sie finden *vor* dem Auftreten der Symptome statt![^pre_symp]

[^pre_symp]: Wir schätzten, dass 44% (95% Konfidenzintervall, 25-69%) der sekundären Fälle während des präsymptomatischen Stadiums der Indexfälle infiziert wurden. (Übersetzung: "We estimated that 44% (95% confidence interval, 25–69%) of secondary cases were infected during the index cases’ presymptomatic stage”) [He, X., Lau, E.H.Y., Wu, P. et al](https://www.nature.com/articles/s41591-020-0869-5)

Aber, wenn wir die letzten engen Kontakte einer Person, die Symptome hat, finden *und unter Quarantäne stellen* ... stoppen wir die Ausbreitung, indem wir ihr einen Schritt voraus bleiben!

![](pics/timeline3.png)

Diese Idee wird als **contact tracing** (Kontaktverfolgung) bezeichnet. Es ist eine alte Idee, die im großen Maßstab erstmals zur Eindämmung von Ebola[^ebola] verwendet wurde. Jetzt ist sie zentraler Bestandteil der Eindämmungsstrategie von COVID-19 in Taiwan & Südkorea!

[^ebola]: "Contact tracing war eine entscheidende Maßnahme in Liberia und stellte eine der größten Kontaktverfolgungsbemühungen während einer Epidemie in der Geschichte dar." (Übersetzung: “Contact tracing was a critical intervention in Liberia and represented one of the largest contact tracing efforts during an epidemic in history.”) [Swanson KC, Altare C, Wesseh CS, et al.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6152989/)

(Dies ermöglicht uns auch, unsere begrenzten Test-Kapazitäten effizienter zu nutzen, um <icon i></icon> vor dem Ausbruch von Symptomen zu finden, ohne so fast alle Leute testen zu müssen.)

Normalerweise werden Kontakte durch persönliche Interviews gefunden, aber das *alleine* geht zu langsam für das ~48-Stunden-Fenster von COVID-19. Deshalb brauchen die Suchenden Hilfe und werden unterstützt von - *NICHT* ersetzt durch - Contact-tracing-Apps.

(Diese Idee stammt nicht von "Nerds": Die Verwendung einer App zur Bekämpfung von COVID-19 wurde zuerst von [einem Team von Epidemiolog\*innen aus Oxford](https://science.sciencemag.org/content/early/2020/04/09/science.abb6936) vorgeschlagen.)

Warte mal, Apps, die zurückverfolgen, mit wem du Kontakt hattest?... Bedeutet das, deine Privatsphäre aufzugeben und sie Big Brother zu opfern?

Nein verdammt! **[DP-3T](https://github.com/DP-3T/documents#decentralized-privacy-preserving-proximity-tracing)**, ein Team von Epidemiolog\*innen & Verschlüsselungsexpert\*innen (darunter einer von uns, Marcel Salathé), entwickelt *bereits* eine Anwendung zur Kontaktverfolgung - mit einem für die Öffentlichkeit zugänglichen Code -, die **keine Informationen preisgibt über deine Identität, deinen Standort, wer deine Kontakte sind und nicht einmal darüber, *wie viele Kontakte* du hattest.**

Das funktioniert folgendermaßen:

![](pics/dp3t.png)

([Hier findest du den vollständigen Comic](https://ncase.me/contact-tracing/). Details zu "pranking" / Fehlalarme / etc. in der Fußnote:[^dp3t_details])

Zusammen mit ähnlichen Teams wie TCN Protocol[^tcn] und MIT PACT[^pact] haben sie Apple & Google dazu gebracht, Kontaktverfolgung bei Wahrung der Privatsphäre direkt in Android/iOS zu implementieren.[^gapple] (Du traust Google/Apple nicht? Gut! Das Schöne an diesem System ist, dass es kein Vertrauen *benötigt*). Bald wird deine örtliche Gesundheitsbehörde dich vielleicht bitten, eine App herunterzuladen. Wenn der Schutz der Privatsphäre dabei gesichert und der Code öffentlich zugänglich ist, dann mach das bitte!

[^dp3t_details]: Um "pranking" (Leute geben fälschlicherweise an, infiziert zu sein) vorzubeugen, setzt das DP-3T-Protokoll voraus, dass dir das Krankenhaus zunächst einen einmaligen Zugangscode schickt, mit dem du deine Nachrichten hochladen kannst.
    
    Fehlalarme sind ein Problem sowohl beim manuellen wie beim digitalen contact tracing. Doch wir können sie auf zwei Arten reduzieren: 1) Indem Bob nur benachrichtigt wird, wenn die App, sagen wir einmal, 30 oder mehr Minuten lang Nachrichten erhalten hat, nicht bloß eine Nachricht im Vorübergehen. Und 2) Wenn die App *wirklich* denkt, dass Bob exponiert war, kann sie ihn an eine\*n *manuelle\*n* Kontaktverfolger\*in verweisen, um ein ausführliches Folgegespräch zu führen.
    
    Zu anderen Themen wie Datenbandbreite, Quellenintegrität und weiteren Sicherheitsfragen, lest euch die [open-source DP-3T whitepapers](https://github.com/DP-3T/documents#decentralized-privacy-preserving-proximity-tracing) durch!

[^tcn]: [Temporary Contact Numbers, ein dezentralisiertes Contact-tracing-Protokoll zur Kontaktverfolgung unter Wahrung der Privatsphäre](https://github.com/TCNCoalition/TCN#tcn-protocol)

[^pact]: [PACT: Private Automated Contact Tracing](https://pact.mit.edu/)

[^gapple]: [Apple und Google partner on COVID-19 contact tracing technology](https://www.apple.com/ca/newsroom/2020/04/apple-and-google-partner-on-covid-19-contact-tracing-technology/). Bitte beachte: Sie entwickeln diese Apps nicht *selbst*, sondern nur die Systemumgebungen, die diese Apps *unterstützen*.

Aber was ist mit den Menschen ohne Smartphones? Oder Infektionen durch Türklinken? Oder "echte" asymptomatische Fälle? Contact-tracing-Apps können nicht alle Übertragungen erfassen... *und das ist okay!* Wir müssen nicht *alle* Übertragungen erfassen, nur über 60%, um R < 1 zu erreichen.

(Dazu ein Rant über die Verwirrung zwischen präsymptomatisch und "echt" asymptomatisch - "echte" Asymptomatiken sind selten:[^rant])

[^rant]: Viele Nachrichtenbeiträge - und ehrlich gesagt auch viele wissenschaftliche Arbeiten - unterscheiden nicht zwischen "Fällen, die keine Symptome zeigten, als wir sie getestet haben" (präsymptomatisch) und "Fällen, die *immer* keine Symptome zeigten". (echt asymptomatisch). Der Unterschied könnte nur dann festgestellt werden, wenn sie die Fälle später nachverfolgen würden.

	Genau das hat [diese Studie] (https://wwwnc.cdc.gov/eid/article/26/8/20-1274_article) getan. (Disclaimer: "Vorzeitige Veröffentlichungen von Artikeln gelten nicht als endgültige Versionen.") In einem Callcenter in Südkorea, das einen COVID-19-Ausbruch erlebte, blieben nur 4 (1,9%) Fälle innerhalb von 14 Tagen nach der Quarantäne asymptomatisch, und keiner ihrer Haushaltskontakte hatte Sekundärinfektionen. 
	
	Das bedeutet also, dass "echte Asymptomatik" selten ist, und die Ansteckung bei einer echten Asymptomatik kann sogar noch seltener sein!

Die Isolierung *symptomatischer* Fälle würde R um bis zu 40% reduzieren, und die Quarantäne ihrer *prä- bzw. asymptomatischen* Kontakte würde R um bis zu 50% reduzieren[^oxford]:

[^oxford]: Von derselben Oxford-Studie, die zuerst Apps im Kampf gegen COVID-19 empfohlen hat: [Luca Ferretti & Chris Wymant et al.](https://science.sciencemag.org/content/early/2020/04/09/science.abb6936/tab-figures-data) Siehe Abbildung 2. Angenommen R<sub>0</sub> = 2.0, fanden sie heraus:    
    
    * Beitrag der symptomatischen Fälle zu R = 0.8 (40%)
    * Beitrag der präsymptomatischen Fälle zu R = 0.9 (45%)
    * Beitrag der asymptomatischen Fälle zu R = 0.1 (5%, obwohl ihr Modell Ungewissheiten beinhaltet und der Beitrag viel niedriger sein könnte)
    * Beitrag von Umwelteinflüssen wie z.B. Türklinken zu R = 0.2 (10%)

    Zählt man die prä- und asymptomatischen Kontakte (45% + 5%) zusammen, kommt man auf 50% von R!

<div class="sim">
		<iframe src="sim?stage=int-4a&format=calc" width="285" height="340"></iframe>
</div>

Das bedeutet, dass wir auch ohne 100%ige Kontaktquarantäne R < 1 bekommen können, und das *ohne Lockdown!* Und somit viel besser für unsere psychische und wirtschaftliche Lage. (Menschen, die sich selbst isolieren, *sollten von ihren Regierungen Unterstützung erhalten* - Kostenübernahme der Tests, Sicherung des Arbeitsplatzes, Subventionierung des bezahlten Urlaubs usw. Das ist immer noch deutlich billiger als periodische Lockdowns).

Wir behalten dann R < 1 bis wir einen Impfstoff haben, der gefährdete <icon s></icon>s zu immunisierten <icon r></icon> macht. Herdenimmunität auf die *richtige* Art:

<div class="sim">
		<iframe src="sim?stage=int-4b&format=calc" width="285" height="230"></iframe>
</div>

(Hinweis: Dieser Rechner simuliert zu 100% wirksame Impfstoffe. In der Realität müssten *über* die "Herdenimmunität" hinweg geimpft werden, um *tatsächlich* Herdenimmunität zu erhalten)

Okay, genug der Worte. Das hier ist eine Simulation von ...

1. ... einem Lockdown über wenige Monate, bis wir...
2. umschalten auf "Testen, Verfolgen, Isolieren", bis wir...
3. genug Leute impfen können, was bedeutet, dass...
4. wir gewinnen.

<div class="sim">
		<iframe src="sim?stage=int-5&format=lines" width="800" height="540"></iframe>
</div>

Das war's also! So machen wir eine Notlandung mit unserem Flugzeug.

So schlagen wir COVID-19.

...

Aber was ist, wenn die Dinge *immer noch* schief gehen? Die Dinge sind ja bereits furchtbar schief gelaufen. Hier spricht die Angst - und das ist gut so! Angst gibt uns Energie, um *Backup-Pläne* zu erstellen.

Der Pessimist erfindet den Fallschirm.

###Szenario 4+: Masken für alle, Sommer, Kurzschluss-Lockdown!
<!-- circuit breaker als Lockdown?! Übersetzung fehlt-->

Was wäre, wenn R<sub>0</sub> viel größer wäre als wir glauben und wir es trotz der Maßnahmen nicht schaffen würden, R auf unter 1 zu drücken? 

Selbst wenn wir es nicht schaffen, R < 1 zu erreichen, reduziert das Senken der Reproduktionszahl die Anzahl der Fälle und rettet damit Leben. R < 1 bleibt aber dennoch unser Ziel und hier sind ein paar weitere Möglichkeiten, wie wir das schaffen können:  

**Masken für alle:**

Vielleicht fragst du dich: *"Moment, ich dachte, Gesichtsmasken schützen gar nicht vor einer Infizierung?"* 
Das stimmt. Alltagsmasken schützen dich nicht vor einer Infektion.[^incoming]... sie reduzieren das Risiko, dass du *andere* infizierst.

[^incoming]: “Keine dieser chirurgischen Masken zeigen eine adäquate Filterleistung, um einen Schutz vor Infektion für den Träger/die Trägerin zu gewährleisten." (übersetzt): “None of these surgical masks exhibited adequate filter performance and facial fit characteristics to be considered respiratory protection devices.” [Tara Oberg & Lisa M. Brosseau](https://www.sciencedirect.com/science/article/pii/S0196655307007742)

[^outgoing]: “The overall 3.4 fold reduction [70% reduction] in aerosol copy numbers we observed combined with a nearly complete elimination of large droplet spray demonstrated by Johnson et al. suggests that surgical masks worn by infected persons could have a clinically significant impact on transmission.” [Milton DK, Fabian MP, Cowling BJ, Grantham ML, McDevitt JJ](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3591312/)

![](pics/masks.png)

Um es mit Zahlen zu untermauern: Trägt eine *infizierte Person* eine chirurgische Gesichtsmaske, reduziert das die Anzahl der Erkältungs- und Grippeviren der Aerosole um 70%.[^outgoing] Eine Reduktion der Ansteckung um 70% entspricht in etwa der Auswirkung eines *Lockdowns*!  

Trotzdem kennen wir weiterhin nicht den *spezifischen* Einfluss von Masken auf das Infektionsgeschehen von COVID-19. Als wissenschaftlich valide gilt ein Ergebnis erst, wenn es zu 95% sicher ist. Auch erst dann sollte es publiziert werden. (...sollte.)[^replication] Alltagsmasken sind zum Zeitpunkt 1. Mai 2020 zu weniger als "95% sicher".  

[^replication]: Echte Wissenschaftler*innen haben den letzten Satz wahrscheinlich mit einem lachenden und einem weinenden Auge gelesen. Siehe auch: [p-hacking](https://de.wikipedia.org/wiki/P-Hacking), [the replication crisis (Englisch)](https://en.wikipedia.org/wiki/Replication_crisis)

Pandemien sind wie Poker: **Wette nur, wenn du dir zu 95% sicher bist und du sonst alles verlieren wirst.** Wie aus einem aktuellen Artikel[^precautionary] über Masken im British Medical Journal hervorgeht, *müssen* unsere Kosten/Nutzen-Analysen mit einem Unsicherheitsfaktor berechnet werden. In etwa so:

[^precautionary]: "Es ist Zeit, das Vorsorgeprinzip anzuwenden" (übersetzt): "It is time to apply the precautionary principle"" [Trisha Greenhalgh et al \[PDF\]](https://www.bmj.com/content/bmj/369/bmj.m1435.full.pdf)

Kosten: Handelt es sich um selbstgemachte Stoffmasken (die etwa ~2/3 so effektiv wie chirurgische Masken[^homemade]) sind), dann ist das superbillig. Wenn es sich um chirurgische Masken handelt, wird es teurer, aber immer noch ziemlich billig.

[^homemade]: [Davies, A., Thompson, K., Giri, K., Kafatos, G., Walker, J., & Bennett, A](https://www.cambridge.org/core/journals/disaster-medicine-and-public-health-preparedness/article/testing-the-efficacy-of-homemade-masks-would-they-protect-in-an-influenza-pandemic/0921A05A69A9419C862FA2F35F819D55) Siehe Tabelle 1: Bei den beiden getesteten bakteriellen Aerosolen hat ein 100%-Baumwoll-T-Shirt ungefähr 2/3 der Filterwirkungsleistung einer chirurgischen Maske.

Nutzen: Selbst wenn es eine 50:50-Chance gibt, dass chirurgische Masken die Übertragung entweder um 0% oder 70% reduzieren, so liegt der Erwartungswert bei 35% und entspricht damit der Hälfte eines *Lockdowns*. Also schätzen wir mit unserem Unsicherheitsfaktor, dass chirurgische Masken R um bis zu 35% reduzieren. (Auch hier können die Annahmen durch Veränderung der Schieberegler hinterfragt und überprüft werden.) 

<div class="sim">
		<iframe src="sim?stage=int-6a&format=calc" width="285" height="380"></iframe>
</div>

(weitere Argumente für/gegen Masken:[^mask_args])

[^mask_args]: **"Wir müssen unsere Vorräte für unsere Krankenhäuser sichern."** *Auf jeden Fall.* Aber das ist eher ein Argument dafür, die Produktion von Masken zu erhöhen, nicht, sie zu rationieren. In der Zwischenzeit können wir Stoffmasken machen.

**"Es ist schwer, sie korrekt zu tragen."** Es ist genauso schwer, die Hände gemäß der WHO-Richtlinien zu waschen - ernsthaft, "Schritt 3) die rechte Handfläche über den Handrücken"?! - und trotzdem empfehlen wir Händewaschen, denn es ist besser, es nicht perfekt zu machen, als gar nicht. 


**"Das Tragen einer Maske macht die Menschen sorgloser im Umgang mit dem Händewaschen &  Abstandhalten."** Klar, Sicherheitsgurte verleiten einige Menschen dazu, Stop-Schilder zu missachten, und dank Zahnseide können die Menschen Steine essen. Wir sollten ernsthaft mit dem Gegenteil argumentieren: Masken sind eine *dauerhafte physische Mahnung* zur Umsicht - und in Ostasien zudem ein Symbol von Solidarität! 
    


Masken *allein* werden nicht dafür sorgen, dass R < 1 erreicht wird. Aber wenn regelmäßiges Händewaschen sowie "Testen - Nachverfolgen - Isolieren" uns zu R = 1,10 bringt, und dann nur ein Drittel der Menschen Masken tragen würde, würde es zu R < 1 kippen. Virus eingedämmt! 

**Sommer:**

Okay, das ist keine "Maßnahme", die wir kontrollieren können, aber sie wird helfen! Es gibt einige Berichte, die behaupten, dass der Sommer nichts an COVID-19 ändert. Sie sind nur zum Teil korrekt: Der Sommer wird R nicht auf unter 1 senken, aber er *wird* ihn reduzieren.  

Für COVID-19 führt ein Temperaturanstieg von jedem 1° Celsius (1,8° Fahrenheit) zu einer Reduktion des R-Werts um 1,2%.[^heat] Der Temperaturunterschied zwischen Sommer und Winter beträgt in New York City etwa 26°C (47°F), sodass der Sommer eine Reduktion des R-Wertes um etwa 31% bewirkt.  

[^heat]: “One-degree Celsius increase in temperature [...] lower[s] R by 0.0225” and “The average R-value of these 100 cities is 1.83”. 0.0225 ÷ 1.83 = ~1.2%. [Wang, Jingyuan and Tang, Ke and Feng, Kai and Lv, Weifeng](https://papers.ssrn.com/sol3/Papers.cfm?abstract_id=3551767)

<div class="sim">
		<iframe src="sim?stage=int-6b&format=calc" width="285" height="220"></iframe>
</div>

Der Sommer allein wird R nicht unter 1 senken, aber wenn wir eingeschränkte Mittel haben, können wir einige Maßnahmen im Sommer lockern und im Winter wieder *stärker* anziehen. 

**Ein "Kurzschluss"-*Lockdown*:**

Und wenn das alles *immer noch* nicht genug ist, R auf unter 1 zu bringen, können wir einen anderen Lockdown versuchen. 

Aber wir müssten nicht immer wieder 2-Monate schließen und einen Monat öffnen. Weil R reduziert wäre, genügten nur ein oder zwei weitere "Kurzschluss"-Lockdowns, bis ein Impfstoff verfügbar ist. (Singapur musste dies "trotz" der 4-monatigen Kontrolle von COVID-19 machen. Das ist kein Versagen, ganz im Gegenteil: dadurch *wird* es zum Erfolg.)

Hier ist eine Simulation eines "lazy case"-Szenarios: 

1. Lockdown, danach
2. Ein moderater Mix von Hygiene, "Testen, Nachverfolgen & Isolieren" sowie annehmbarer Maskenpflicht, danach ...
3. ein "Kurzschluss"-Lockdown, bevor ein Impfstoff entwickelt wird.  

<div class="sim">
		<iframe src="sim?stage=int-7&format=lines&height=620" width="800" height="620"></iframe>
</div>

Und dann sind da noch die *weiteren* Maßnahmen, die wir ergreifen könnten, um R weiter zu senken: 

* Reiseeinschränkungen / Quarantäne
* Fieber-Checks in Einkaufsmärkten & Schulen 
* Professionelle Desinfektion öffentlicher Plätze 
* [Begrüßung per Fuß anstelle eines Handschlags](https://twitter.com/V_actually/status/1233785527788285953)
* Und alle anderen Dinge, die Menschen einfallen werden

Wir hoffen, dass diese Pläne etwas Hoffnung schaffen. 

**Selbst bei einem pessimistischen Szenario *ist* es möglich COVID-19 zu bekämpfen und unsere Gesundheit und Wirtschaft zu schützen. ** Durch den *Lockdown* als "Neustart", das gleichzeitige Senken des Reproduktionsfaktors (R < 1), der Fallisolierung sowie einer breiten Verwendung einer datenschutzkonformen App zur Nachverfolgung der Kontakte und der Maskenpflicht... kann es gelingen, dass das Leben wieder in eine neue Normalität zurückkehrt.  

Klar, deine Hände werden wahrscheinlich ganz spröde sein. Aber du kannst dich wieder zu einem Date im Comicladen verabreden. Du kannst dir mit Freunden einen neuen Hollywood-Streifen im Kino ansehen. Du kannst wieder Leute in der Bücherei beobachten oder dich einfach mit anderen daran erfreuen, *am Leben* zu sein.

Selbst wenn es zum Worst-Case-Szenario kommt ... das Leben geht weiter.

Also machen wir uns bereit für ein paar wirklich *üble* Worst-Case-Szenarien. Notwasserung! Nimm deine Rettungsweste und begib dich zu den Notausgängen:  
<!-- Ende Übersetzung von Julian @herr_hundt -->
<!-- "The next few years" übersetzt von jan.koelling -->
<div class="section chapter">
    <div>
		<img src="banners/curve.png" height=480 style="position: absolute;"/>
        <div>Die nächsten paar Jahre</div>
    </div>
</div>

Du bekommst COVID-19 und erholst dich. Oder du bekommst die COVID-19-Impfung. So oder so bist du jetzt immun ...

...*für wie lange?*


* COVID-19 ist am engsten mit SARS verwandt, welches die Überlebenden für 2 Jahre immun machte.[^SARSimmunity]
* Die Coronaviren, die normale Erklältungen auslösen, machen dich für 8 Monate immun.[^coldimmunity]
* Es gibt Berichte von Leuten, die sich von COVID-19 erholt haben, dann aber wieder positiv gestestet wurden. Es ist noch unklar, ob diese falsch postiv waren.[^unclear]
* Eine *noch nicht fachlich begutachtete* Studie an Affen zeigte Immunität gegen COVID-19-Coronaviren für mindestens 28 Tage.[^monkeys]

Aber für COVID-19 *beim Menschen* ist, Stand 1. Mai 2020, "für wie lange" die große Unbekannte.

[^SARSimmunity]: SARS-spezifische Antikörper wurden für durchschnittlich 2 Jahre erhalten [...] Daher könnten SARS-Patienten ≥3 Jahre nach ursprünglichem Kontakt für eine Neuinfektion anfällig sein. [Wu LP, Wang NC, Chang YH, et al.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2851497/) 
"Leider" werden wir niemals wissen wie lange SARS-Immunität wirklich erhalten geblieben wäre, da wir es so schnell ausgerottet haben.

<!-- Read paper to check what 'enrollment' stands for in this context. I guessed enrollment of a patient for the study. -->
[^coldimmunity]: Wir konnten keinen signifikaten Unterschied zwischen der Wahrscheinlichkeit für wenigsten einen positiven Test und der Wahrscheinlichkeit eines Wiederauftretens für die Beta-Coronaviren HKU1 und OC43 34 Wochen nach Registrierung für die Studienteilnahme/der Erstinfektion feststellen. [Marta Galanti & Jeffrey Shaman (PDF)](http://www.columbia.edu/~jls106/galanti_shaman_ms_supp.pdf)

[^unclear]: Nachdem eine Person einen Virus abgewehrt hat, neigen Viruspartikel dazu, eine Weile zu verbleiben. Diese Partikel können keine Infektion auslösen, aber sie können zu einem positiven Testergebnis führen. [aus STAT News von Andrew Joseph](https://www.statnews.com/2020/04/20/everything-we-know-about-coronavirus-immunity-and-antibodies-and-plenty-we-still-dont/)

[^monkeys]: Aus [Bao et al.](https://www.biorxiv.org/content/10.1101/2020.03.13.990226v1.abstract) *Hinweis: Dieser Artikel ist ein Preprint und wurde (noch) nicht wissenschaftliche begutachtet.* 
Außerdem, um es hervorzuheben: es wurde nur eine erneute Infektion nach 28 Tagen getestet.

Für die folgenden Simulationen, lass uns annehmen dass es 1 Jahr ist. 
**Hier ist eine Simulation, die mit 100% <icon r></icon> anfängt** und exponentiell zerfällt, mit im Mittel nach einem Jahr nicht mehr immunen, wieder anfälligen <icon s></icon>s mit Abweichungen:

<div class="sim">
		<iframe src="sim?stage=yrs-1&format=lines&height=600" width="800" height="600"></iframe>
</div>

Rückkehr des exponentiellen Zerfalls!

Das ist das **SEIRS Modell**. Das letzte "S" steht wieder für <icon s></icon> "Susceptible" (anfällig).

![](pics/seirs.png)

Lass uns jetzt einen COVID-19 Ausbruch über 10 Jahre, ohne Maßnahmen simulieren... *wenn Immunität nur ein Jahr anhält:*

<div class="sim">
		<iframe src="sim?stage=yrs-2&format=lines&height=600" width="800" height="600"></iframe>
</div>

In vorangegangen Simulationen hatten wir nur *eine* die Intensivstationen überfordernde Spitze. Jetzt haben wir mehrere und die <icon i></icon> Fälle pendeln sich *dauerhaft* bei der Kapazität der Intensivstationen ein.
(Denk dran, diese hatten wir für diese Simulationen *verdreifacht*.)

R = 1, es ist **endemisch.**

Zum Glück reduziert der Sommer R, was die Situation verbessert:

<div class="sim">
		<iframe src="sim?stage=yrs-3&format=lines&height=640" width="800" height="640"></iframe>
</div>

Oh.


Überraschenderweise macht der Sommer die Spitzen schlimmer *und* regelmäßig! Das liegt daran, dass der Sommer die neuen <icon i></icon>s absenkt, was aber wiederum die neuen imunen <icon r></icon>s absenkt. Das bedeutet, Immunität stürzt im Sommer ab was eine große, wiederkehrende Spitze im Winter *erzeugt*.

Zum Glück ist die Lösung hierfür recht klar – impft die Menschen jeden Herbst/Winter, so wie es auch mit den Grippeimpfungen gemacht wird:

**(Nachdem du die Aufnahme abgespielt hast, versuche deine eigenen Impfkampagnen zu simulieren! Denk dran, dass du die Simulation jederzeit pausieren/fortsetzen kannst.)**

<div class="sim">
		<iframe src="sim?stage=yrs-4&format=lines" width="800" height="540"></iframe>
</div>

Aber hier ist die erschreckendere Frage:

Was ist, wenn es über *Jahre* keinen Impfstoff gibt? Oder *niemals*?

**Zur Klarstellung: das ist unwahrscheinlich.** Die meisten Epidemiologinnen und Epidemiologen rechnen mit einem Impfstoff in 1 bis 2 Jahren. Ja, es gab noch nie einen Impfstoff für eines der anderen Coronaviren, aber das liegt daran, dass SARS schnell ausgelöscht wurde und die "normale" Erkältung die Investition nicht gerechtfertigt hat. 

Dennoch haben Forscherinnen und Forscher für Infektionskrankheiten Besorgnis geäußert: Was ist, wenn wir nicht genug herstellen können?[^vax_enough] Was, wenn wir es überstürzen und es nicht sicher ist?[^vax_safe]

[^vax_enough]: "Falls ein Impfstoff für das Coronavirus erscheint, kann die Welt genug davon herstellen?" (übersetzt): “If a coronavirus vaccine arrives, can the world make enough?” [von Roxanne Khamsi, auf Nature](https://www.nature.com/articles/d41586-020-01063-8)

[^vax_safe]: "Drängt nicht auf die Herausgabe von COVID-19 Impfstoffen und Medikamenten ohne ausreichende Sicherheitsgarantien" (übersetzt): “Don’t rush to deploy COVID-19 vaccines and drugs without sufficient safety guarantees” [von Shibo Jiang, auf Nature](https://www.nature.com/articles/d41586-020-00751-9)

Selbst im Albtraumszenario "kein Impfstoff" haben wir noch 3 Auswege. Vom allerschlimmsten zum am wenigsten schlimmen:

1) Mach' periodische Lockdowns oder lockere R < 1 Maßnahmen, um "natürliche Herdenimmunität" zu erreichen. (Warnung: Das würde zu vielen Todesfällen & beschädigten Lungen führen. *Und* es wird nicht funktionieren, falls die Immunität nicht anhält.)

2) Mach' die R < 1 Maßnahmen für immer. Kontaktverfolgung & das Tragen von Masken werden zur neuen Normalität in der Welt nach COVID-19, so wie Tests auf Geschlechtskrankheiten & das Tragen von Kondomen die neue Normalität in der Welt nach HIV wurden.

3) Mach' die R < 1 Maßnahmen, bis wir Behandlungsoptionen entwickelt haben, die es viel, viel unwahrscheinlicher machen, dass COVID-19 intensivmedizinische Maßnahmen erfordert. (Das sollten wir *auf jeden Fall* tun!) Den Bedarf für Intensivstationen um das 10-fache zu senken hat den gleichen Effekt wie die Kapazität der Intensivstationen um das 10-fache zu erhöhen:

**Hier ist eine Simulation *ohne* anhaltende Immunität, *ohne* Impfsstoff und selbst ohne irgendeine Maßnahme – einfach ein langsamer Anstieg der Kapazitäten, um die langfristigen Spitzen zu überleben:**

<div class="sim">
		<iframe src="sim?stage=yrs-5&format=lines" width="800" height="540"></iframe>
</div>

Selbst im schlimmsten Worst-Case-Szenario... das Leben geht weiter.

Vielleicht möchtest du unsere Annahmen hinterfragen und andere R<sub>0</sub>'s oder Werte ausprobieren. Oder deine *eigene* Kombination von Interventionsmaßnahmen ausprobieren!

**Hier ist ein (optionaler) Sandkastenmodus, bei dem *alles* verfügbar ist. (Scrolle, um alle Einstellungen zu sehen) Simuliere und spiele nach Herzenslust herum:**

<div class="sim">
		<iframe src="sim?stage=SB&format=sb" width="800" height="540"></iframe>
</div>

Dieser einfache "epidemische Flugsimulator" hat uns viel beigebracht. Er hat es ermöglicht, Fragen zu den letzten paar Monaten, den nächsten paar Monaten und den nächsten paar Jahren zu beantworten.

Lass uns endlich zurückkehren zum ...

<div class="section chapter">
    <div>
        <img src="banners/curve.png" height=480 style="position: absolute;"/>
        <div>Jetzt</div>
    </div>
</div>

Das Flugzeug ist untergegangen. Wir hocken zusammengedrängt in den Rettungsbooten. Es ist Zeit, Festland zu suchen.[^dry_land]

[^dry_land]: Festland-Metapher [von Marc Lipsitch und Yonatan Grad, auf STAT News](https://www.statnews.com/2020/04/01/navigating-covid-19-pandemic/)

Teams aus Epidemiologinnen und Epidemiologen und Menschen in der Politik ([links](https://www.americanprogress.org/issues/healthcare/news/2020/04/03/482613/national-state-plan-end-coronavirus-crisis/), [rechts](https://www.aei.org/research-products/report/national-coronavirus-response-a-road-map-to-reopening/ ), und [überparteilich](https://ethics.harvard.edu/covid-roadmap)) haben einen Konsens darüber erzielt, wie wir COVID-19 schlagen können und gleichzeitig unser Leben *und* unsere Freiheiten schützen.

Hier ist die grobe Idee, mit einigen (weniger konsensfähigen) Alternativplänen:

![](pics/plan.png)

Was bedeutet das für DICH, jetzt gerade?

**Für jede und jeden:** Respektiere die Ausgangsbeschränkungen, damit wir so schnell wie möglich aus Phase I herauskommen können. Wasche dir weiter die Hände. Stelle deine eigenen Masken her. Lade eine *datenschutzfreundliche* App zur Ermittlung von Kontaktpersonen herunter, sobald diese im nächsten Monat verfügbar sind. Bleib gesund - körperlich und geistig! Und schreib den lokalen Entscheidungstragenden, dass sie ihren Hintern hochkriegen sollen und...

**Für Politikerinnen und Politiker:** Erlassen Sie Gesetze zur Unterstützung von Menschen, die sich selbst isolieren/quarantänisieren müssen. Stellen Sie mehr menschliche Kontaktverfolgerinnen und Kontaktverfolger ein, *unterstützt* durch datenschutzfreundliche Apps. Leiten Sie mehr Mittel in die Dinge, die wir herstellen sollten, wie..

**Für Maker[^maker]:**  Stellt Tests her, Beatmungsgeräte, Personenschutzausrüstung für Krankenhäuser und Arztpraxen. Stellt Tests, Masken und Apps her, dazu antivirale Medikamente, Prophylaktika und andere Behandlungsmethoden, die keine Impfstoffe sind. Und stellt Impfstoffe, Tests, Tests und nochmals Tests her. Erzeugt Hoffnung.

[^maker]: Eine Erklärung des Begriffes ist hier zu finden.(https://de.wikipedia.org/wiki/Maker)

Spiele die Angst nicht herunter, um Hoffnung aufzubauen. Unsere Angst sollte sich mit unserer Hoffnung *verbünden*, wie die Erfinder der Flugzeuge und Fallschirme. Durch Vorbereitung auf eine schreckliche Zukunft *erschaffen* wir eine hoffnungsvolle Zukunft.

Das einzige, was man fürchten muss, ist die Vorstellung, dass das einzige, was man fürchten muss, die Furcht selbst ist. 
