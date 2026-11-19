# Kritiek, replicaties, correcties en intrekkingen bij de kernstudies van de notitie "Onderzoekend vermogen in een tijd van AI" (peildatum 18 november 2026)

Onderzoeksnotities, opgesteld door de AI-assistent Claude. Waar Claude zelf een methodologisch punt heeft afgeleid dat niet in de literatuur staat, staat dat expliciet als "analyse Claude, geen gepubliceerde kritiek". Bronnen zonder peer review zijn gelabeld: **PREPRINT**, **WERKDOCUMENT**, **BLOG**, **PERS**, **LEVERANCIER**. Verdicten: **houdbaar**, **houdbaar met kanttekening**, **overschat** (de notitie claimt meer dan de studie toont).

## Zoekverantwoording: welke databases zijn doorzocht en met welke methode?

### Takeaway
Voor 27 DOI's en twee arXiv-preprints zijn correcties en intrekkingen systematisch nagegaan via Crossref (dat sinds 2023 de Retraction Watch-database bevat). Commentaren en brieven zijn gezocht via OpenAlex (citerende werken van het type letter/erratum/retraction en titels met "comment", "reply", "reanalysis", "replication" en dergelijke), via Europe PMC (comment- en correctielinks, titelzoekacties) en via gerichte webzoekacties. Uitgeverssites van PNAS, The Lancet, ScienceDirect, INFORMS, AOM en MDPI blokkeerden geautomatiseerde toegang (HTTP 403). Daardoor is van een deel van de brieven alleen het bestaan vastgesteld en niet de volledige inhoud.

### Cited Findings
- **Crossref REST API** (`updated-by`, `relation`): alleen drie van de onderzochte werken hebben een update. Bastani et al. kreeg een correctie op 20-08-2025, Budzyń et al. een erratum op 01-11-2025 en Gerlich een correctie die Crossref op 03-01-2025 dateert (Semantic Scholar: 10-09-2025). Geen enkele bron in de notitie is ingetrokken. Voorbeeld: [Crossref, Bastani](https://api.crossref.org/works/10.1073/pnas.2422633122); [Crossref, Budzyń](https://api.crossref.org/works/10.1016/S2468-1253(25)00133-5); [Crossref, Gerlich](https://api.crossref.org/works/10.3390/soc15010006).
- **Crossref-zoekactie in PNAS** (ISSN 0027-8424, vanaf 01-11-2025) naar "Reply to Westwood" en "Reply to Bastani": er bestaat een briefwisseling over Westwood, maar er zijn geen brieven over Bastani gevonden — [Crossref query](https://api.crossref.org/works?query.bibliographic=Reply%20to%20Westwood&filter=from-pub-date:2025-11-01,issn:0027-8424).
- **OpenAlex** (`cites:`-filter met type letter/erratum/retraction en titelzoektermen) leverde alleen brieven op bij Budzyń et al. (drie brieven en een antwoord van de auteurs in *Lancet Gastroenterol Hepatol*). Bij Bastani, Lee, Fernandes, Barcaui, Bergenholtz, Kestin, Dell'Acqua, Autor, Scarfe, Linardon, Bisbee, Sarstedt, Westwood en Gerlich vond OpenAlex geen brieven of commentaren — [OpenAlex Bastani W4411627694](https://openalex.org/W4411627694); [OpenAlex Budzyń W4413186556](https://openalex.org/W4413186556).
- **Europe PMC** (commentCorrectionList en titelzoekactie "deskilling" in GI-tijdschriften): het erratum bij Bastani, het erratum bij Budzyń, de Lancet-brieven en drie vervolgstudies naar deskilling (Okumura 2026, Pedersen 2026, Dominitz 2026) — [Europe PMC](https://europepmc.org/article/MED/40816301).
- **Semantic Scholar API** voor abstracts van Dell'Acqua 2026a/b, Fernandes, Allen & McDonald, Boussioux, Balt, Gonsalves en de Gerlich-correctie ("Error in Table") — [Semantic Scholar Gerlich-correctie](https://api.semanticscholar.org/graph/v1/paper/DOI:10.3390/soc15090252).
- **arXiv** (versiegeschiedenis en journal-ref) voor Becker et al. en Kosmyna et al. — [arXiv 2507.09089](https://arxiv.org/abs/2507.09089); [arXiv 2506.08872](https://arxiv.org/abs/2506.08872).
- **PubPeer**: geen threads gevonden via een site-beperkte webzoekactie. De zoekmachine indexeert PubPeer slecht. Een rechtstreekse API-bevraging is niet uitgevoerd, omdat die een ontwikkelaarssleutel van derden vraagt. Een negatieve uitkomst voor PubPeer is dus zwak — [zoekactie site:pubpeer.com, uitgevoerd 18-11-2026, geen URL beschikbaar].
- **Webzoekacties** (algemeen, plus Science Media Centre, Retraction Watch, METR-blog, vakblogs) per studie, met termen als "critique", "letter", "replication", "reanalysis" en "follow-up".
- **Volledige teksten gelezen** via Europe PMC/PMC (Bastani-abstract, Kestin, Scarfe, Balt, Linardon, Westwood) en via pdf (Fernandes et al. 2026, Lee et al. 2025, de Rothschild-brief over Westwood) — [Kestin PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/); [Fernandes pdf](https://thomaskosch.com/wp-content/papercite-data/pdf/fernandes2025ai.pdf); [Lee pdf](https://advait.org/files/lee_2025_ai_critical_thinking_survey.pdf).

### Inferences
- Voor de meeste studies is "geen gepubliceerde kritiek gevonden" een echte uitkomst: drie onafhankelijke bronnen (Crossref, OpenAlex, Europe PMC) en webzoekacties gaven geen treffers. Dat geldt het sterkst voor tijdschriften waar brieven als eigen record worden geïndexeerd (Lancet, PNAS). Het geldt minder sterk voor tijdschriften zonder brievenrubriek (bijv. *Social Sciences & Humanities Open*, *Computers in Human Behavior*). Daar loopt kritiek eerder via blogs of nieuwe studies.
- Gepubliceerde, inhoudelijke discussie bestaat vooral bij twee studies: **Budzyń et al.** (brieven, expertreacties en twee prospectieve studies die geen deskilling vonden) en **Westwood** (PNAS-briefwisseling, een tegenstudie in PNAS en een door een leverancier gefinancierde preprint).

### Gaps
- De volledige tekst van de Lancet-brieven (Lam; Levartovsky & Kopylov; van de Sande et al.), van het auteursantwoord en van het Ahmad-commentaar was niet toegankelijk (paywall/403).
- Google Scholar "cited by" en Scopus zijn niet direct bevraagd (geen API-toegang). OpenAlex dekt deze grotendeels, maar niet volledig.

## 1. Bastani et al. (2025), PNAS: houdt "Generative AI without guardrails can harm learning" stand?

### Takeaway
Er is geen gepubliceerde brief, reanalyse of mislukte replicatie gevonden. De enige correctie gaat over de affiliatie van één auteur. De notitie geeft de cijfers correct weer en noemt de populatie ("scholieren"). Het blijft wel K-12-onderzoek (één Turkse middelbare school, één vak, GPT-4 in het najaar van 2023), en de vertaling naar hbo-onderzoeksvaardigheden is een extrapolatie. **Verdict: houdbaar met kanttekening.**

### Cited Findings
- **Studie zoals geciteerd:** Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö., & Mariman, R. (2025). Generative AI without guardrails can harm learning: Evidence from high school mathematics. *PNAS, 122*(26), e2422633122 — [DOI](https://doi.org/10.1073/pnas.2422633122).
- **Claim in de notitie (punt 2, §5):** "In een veldexperiment met bijna duizend scholieren stegen de oefencijfers wiskunde met een standaardversie van ChatGPT met 48%. Zonder AI scoorde die groep daarna 17% lager dan leerlingen die nooit AI hadden." In de kanttekening staat dat de hint-tutor de schade "grotendeels" voorkwam. §5 noemt de studie "het sterkste bewijs" — [notitie, lokaal bestand](file:///Users/witoldtenhove/Documents/HAN/afstudeeronderzoek/docs/notitie-onderzoekend-vermogen-ai.html).
- **Wat de studie zegt (abstract):** "48% improvement in grades for GPT Base and 127% for GPT Tutor"; zonder AI "students actually perform worse than those who never had access (17% reduction in grades for GPT Base)"; "These negative learning effects are largely mitigated by the safeguards in GPT Tutor" — [Europe PMC/PMC12232635](https://pmc.ncbi.nlm.nih.gov/articles/PMC12232635/).
- **Correctie (type: correctie door uitgever):** Correction for Bastani et al. (2025). *PNAS, 122*(34), e2518204122. Door een productiefout stond de affiliatie van Osbert Bastani verkeerd; de bevindingen veranderen niet — [PMC12403119](https://pmc.ncbi.nlm.nih.gov/articles/PMC12403119/); [DOI](https://doi.org/10.1073/pnas.2518204122).
- **Brieven, reanalyses en replicaties:** in Crossref (PNAS-zoekactie), OpenAlex (type letter, titels met "reply"/"comment") en Europe PMC (alleen het erratum gelinkt) is niets gevonden — [Crossref](https://api.crossref.org/works/10.1073/pnas.2422633122); [OpenAlex](https://openalex.org/W4411627694).
- **Context volgens de auteurs:** veldexperiment op één grote Turkse middelbare school, leerjaren 9–11, najaar 2023; de auteurs zelf: "our study focuses on two generative AI tutors for a single topic (mathematics) deployed in a single high school in Turkey" (citaat via zoeksamenvatting van de PNAS-tekst) — [PNAS pdf](https://www.pnas.org/doi/pdf/10.1073/pnas.2422633122).
- **Vervolgonderzoek van dezelfde groep (type: follow-up, WERKDOCUMENT):** Bastani en Chung testten een gepersonaliseerde AI-tutor met guardrails in een Python-cursus van vijf maanden op tien middelbare scholen in Taipei. Examenscores stegen met 0,15 SD. Dit is geen replicatie van het schade-effect — [Mack Institute, 2026](https://mackinstitute.wharton.upenn.edu/2026/research-spotlight-bastani-chung/).
- **Verwante, deels nuancerende evidentie (PREPRINT):** Contractor, Z., & Reyes, G. (2026). *Experimental evidence on the learning impact of generative AI* (arXiv:2607.08849). In een bewaakt, gerandomiseerd experiment met bachelorstudenten verhoogde AI-toegang de scores op toetsen zonder hulp, en een kleinere winst hield een week stand. De winst bleef bij studenten die AI als tutor gebruikten en verdween bij studenten die AI lieten schrijven — [arXiv](https://arxiv.org/abs/2607.08849).

### Inferences
- De claim in punt 2 is cijfermatig correct, en de notitie zegt "scholieren". De samenvatting ("In het kort") generaliseert het patroon naar "studenten". Bastani gaat over leerlingen in het voortgezet onderwijs en wiskunde-oefensessies, niet over hbo-studenten en onderzoeksvaardigheden. De sprong naar probleemformulering en onderzoek is een redenering, geen bevinding (analyse Claude).
- "17% lager" is een relatieve daling in cijfers ten opzichte van de controlegroep, geen effect in standaarddeviaties. De notitie formuleert het correct.
- Modelgeneratie: GPT-4 uit 2023 in een chatinterface. Het mechanisme (antwoorden overnemen als "crutch") hangt minder af van modelkwaliteit dan van het ontwerp. Daarom veroudert deze bevinding waarschijnlijk minder snel dan foutpercentages van tools (analyse Claude).
- Contractor & Reyes (preprint) en de tutorarm van Bastani zelf wijzen dezelfde kant op als de notitie: het gebruikspatroon bepaalt de uitkomst, niet de toegang tot AI. Dat ondersteunt de regel "eerst zelf, AI als tutor". Het ondergraaft wel de stelligheid van "een vast patroon" (zie Kernvraag D).

### Gaps
- Er is geen onafhankelijke, vooraf geregistreerde replicatie van het Bastani-design gevonden (2025–2026).
- Het is niet gecontroleerd of de PNAS-versie dezelfde effectgroottes en significanties rapporteert als de SSRN-versie uit 2024. De abstracts noemen dezelfde 48/127/17%.

## 2. Lee et al. (2025), CHI: houdt de Microsoft-enquête over kritisch denken stand?

### Takeaway
Er is geen gepubliceerde kritiek, reanalyse of replicatie gevonden. De belangrijkste beperkingen noemen de auteurs zelf: het gaat om zelfrapportage, deelnemers verwarren "minder moeite" met "minder kritisch denken", het zelfvertrouwen is subjectief, de steekproef is Engelstalig, jong en technisch vaardig, en het onderzoek is cross-sectioneel. De notitie labelt het correct als enquête, maar het woord "verschoof" suggereert een gemeten verandering. **Verdict: houdbaar met kanttekening.**

### Cited Findings
- **Studie:** Lee, H.-P., Sarkar, A., Tankelevitch, L., Drosos, I., Rintel, S., Banks, R., & Wilson, N. (2025). The impact of generative AI on critical thinking: Self-reported reductions in cognitive effort and confidence effects from a survey of knowledge workers. *CHI '25*, 1–22 — [DOI](https://doi.org/10.1145/3706598.3713778).
- **Claim in de notitie (punt 1):** "In een enquête onder 319 kenniswerkers verschoof kritisch denken met AI naar informatie controleren, antwoorden samenvoegen en het werk bewaken. Meer vertrouwen in AI ging samen met minder kritisch denken."
- **Beperkingen volgens de auteurs:** deelnemers "occasionally conflated reduced effort in using GenAI with reduced effort in critical thinking … potentially leading to inaccurate self-reporting"; "subjective self-confidence may not always be well-calibrated"; een Engelstalige steekproef via Prolific die "biased towards younger, more technologically skilled participants" was; de auteurs bevelen "think-aloud protocols or task-based assessments" aan — [Lee et al., pdf](https://advait.org/files/lee_2025_ai_critical_thinking_survey.pdf).
- **Gepubliceerde kritiek:** geen gevonden in OpenAlex (1.429 citerende werken, geen comment/reply), Crossref (geen updates) of via webzoekacties — [OpenAlex W4409885395](https://openalex.org/W4409885395); [Crossref](https://api.crossref.org/works/10.1145/3706598.3713778).
- **Media-overdrijving (PERS):** koppen als "Study: GenAI Is Eroding Critical Thinking" gaan verder dan de correlationele zelfrapportage — [Redmondmag, 2025](https://redmondmag.com/articles/2025/02/18/genai-is-eroding-critical-thinking.aspx). De notitie neemt die framing niet over.
- **Verwant experimenteel werk (PREPRINT):** een standaard-LLM-baseline gaf het hoogste *ervaren* begrip maar het laagste *objectieve* leren (N = 85). Dat bevestigt indirect het gat tussen zelfrapportage en werkelijke prestatie — [Eleftheriou et al., 2026, arXiv:2604.09444](https://arxiv.org/abs/2604.09444).

### Inferences
- "Verschoof" en "minder kritisch denken" moeten als zelfrapportage gelezen worden: deelnemers *zeggen* minder kritische denkinspanning te leveren. Een betere formulering: "Kenniswerkers die meer vertrouwen hebben in AI, zeggen er minder kritisch over na te denken" (analyse Claude).
- De studie draagt punt 1 als illustratie ("enquête of interviews"), niet als causaal bewijs. De notitie zet haar in punt 1 naast een experiment (Bergenholtz) en praktijkbronnen. Het bewijslabel "ENQUÊTE OF INTERVIEWS" staat erbij.

### Gaps
- Er is geen replicatie met objectieve maten van kritisch denken bij kenniswerkers gevonden (2025–2026).

## 3. Budzyń et al. (2025), Lancet Gastroenterology & Hepatology: deskilling van endoscopisten

### Takeaway
Dit is de studie met de meeste gepubliceerde reactie: een begeleidend commentaar, drie brieven en een antwoord van de auteurs in hetzelfde tijdschrift, een erratum, expertreacties over confounding, en twee prospectieve vervolgstudies die **geen** deskilling vonden. De notitie formuleert de bevinding causaal en algemeen ("Ook ervaren professionals worden minder waakzaam"). Dat gaat verder dan een observationele voor-en-nastudie draagt, en verder dan de auteurs zelf gaan. **Verdict: overschat** (de cijfers kloppen; de formulering en de stelligheid niet).

### Cited Findings
- **Studie:** Budzyń, K., Romańczyk, M., Kitala, D., … Mori, Y. (2025). Endoscopist deskilling risk after exposure to artificial intelligence in colonoscopy: A multicentre, observational study. *Lancet Gastroenterol Hepatol, 10*(10), 896–903 — [DOI](https://doi.org/10.1016/S2468-1253(25)00133-5).
- **Claim in de notitie (punt 6):** "Ook ervaren professionals worden minder waakzaam. Artsen die drie maanden met AI hadden gewerkt, vonden daarna zonder AI minder voorstadia van darmkanker: 22,4% tegen eerder 28,4%." Bewijslabel: OBSERVATIONEEL ONDERZOEK.
- **Design:** retrospectieve vergelijking in vier Poolse centra (ACCEPT-trial). 795 colonoscopieën zonder AI vóór en 648 zonder AI ná de invoering van AI, telkens in een periode van drie maanden. De ADR daalde van 28,4% naar 22,4% (verschil −6,0%, 95%-BI −10,5 tot −1,6; OR 0,69) — [AGA News, 2026](https://news.gastro.org/issues/2026/september-2026/ais-deskilling-question-has-a-gi-metric-adr/). De auteurs schrijven dat AI-blootstelling de kwaliteit "might reduce" — [AGA News](https://news.gastro.org/issues/2026/september-2026/ais-deskilling-question-has-a-gi-metric-adr/).
- **Begeleidend commentaar (type: comment):** Ahmad, O. F. (2025). Endoscopist deskilling: An unintended consequence of AI-assisted colonoscopy? *Lancet Gastroenterol Hepatol* — [DOI](https://doi.org/10.1016/S2468-1253(25)00164-5). Volgens een secundaire bron (**PREPRINT**, niet geverifieerd tegen de originele tekst) wijst Ahmad op verschillen tussen de patiëntgroepen vóór en ná, op het ontbreken van terugtrektijden, op het kleine aantal endoscopisten (19) en op secundaire uitkomsten die niet significant daalden — [arXiv:2607.12125](https://arxiv.org/pdf/2607.12125).
- **Brieven (type: letter), allemaal in *Lancet Gastroenterol Hepatol, 10*(12), dec. 2025:**
  - Lam, K. (2025), p. 1060 — [DOI](https://doi.org/10.1016/S2468-1253(25)00290-0).
  - Levartovsky, A., & Kopylov, U. (2025), pp. 1060–1061 — [DOI](https://doi.org/10.1016/S2468-1253(25)00289-4).
  - van de Sande, D., Sleijfer, S., Buijsman, S. N. R., Gommers, D., & van Genderen, M. E. (2025), pp. 1061–1062 (Erasmus MC/TU Delft) — [DOI](https://doi.org/10.1016/S2468-1253(25)00288-2). Volgens zoeksamenvattingen noemt deze brief terugtrekken uit AI-ondersteuning op basis van de studie "een onvolledige lezing" en plaatst hij de discussie in het kader van mens-AI-interactie (inhoud niet zelf gelezen) — [Lancet-abstractpagina](https://www.thelancet.com/journals/langas/article/PIIS2468-1253(25)00288-2/abstract).
  - Antwoord van de auteurs: Budzyń, K., Romańczyk, M., & Mori, Y. (2025), p. 1062 — [DOI](https://doi.org/10.1016/S2468-1253(25)00324-3); lijst via [Europe PMC](https://europepmc.org/search?query=TITLE%3A%22deskilling%22%20AND%20TITLE%3A%22colonoscopy%22).
- **Erratum:** *Lancet Gastroenterol Hepatol, 10*(11), e12 — [DOI](https://doi.org/10.1016/S2468-1253(25)00294-8). De inhoud van het erratum is niet gecontroleerd.
- **Expertreacties (type: expertcommentaar, niet peer-reviewed), Science Media Centre:**
  - Prof. Venet Osmani (QMUL) wijst op confounding door werkdruk: het aantal colonoscopieën "nearly doubled after the AI tool was introduced, going from 795 to 1382". Hij noemt ook niet-gemeten organisatieveranderingen, een periode van "just three months" en het verschil tussen gewoonte en vaardigheid.
  - Prof. Allan Tucker (Brunel) noemt het "only one study", één AI-systeem, selectie van gemotiveerde clinici en "major changes to the endoscopy department … in the middle of the study". Volgens hem zijn gerandomiseerde crossovertrials nodig.
  - Bron: [Science Media Centre, aug. 2025](https://www.sciencemediacentre.org/expert-reaction-to-observational-study-looking-at-detection-rate-of-precancerous-growths-in-colonoscopies-by-health-professionals-who-perform-them-before-and-after-the-routine-introduction-of-ai/).
- **Vervolgstudie 1, geen deskilling (type: onafhankelijke prospectieve studie):** Okumura, T., Kudo, S.-E., … Misawa, M. (2026). Long-term impact of computer-aided adenoma detection: A prospective observational study. *Endoscopy, 58*(2), 121–129. Eén centrum in Japan, 2021–2023, 4.712 gematchte colonoscopieën: "the detection rate in procedures performed without CADe was maintained and did not decline over time" — [DOI](https://doi.org/10.1055/a-2661-2624); [Europe PMC](https://europepmc.org/search?query=DOI%3A%2210.1055%2Fa-2661-2624%22).
  - Daarop volgden een brief van Henry & East en een antwoord: Okumura, T., & Misawa, M. (2026). Reply to Henry and East. *Endoscopy, 58*, 315–316 — [DOI](https://doi.org/10.1055/a-2764-0296). Volgens een zoeksamenvatting zagen Henry & East meer hooggradige adenomen in de groep zonder CADe; het antwoord meldt geen significant verschil in geavanceerde neoplasie (4,1% vs 4,7%; p = .39). Deze cijfers zijn niet zelf geverifieerd.
  - Begeleidend commentaar: Sinonquel, P. (2026). Long-term learning and not deskilling: A reassuring signal for computer-aided detection-assisted colonoscopy. *Endoscopy, 58*, 130–131 — [DOI](https://doi.org/10.1055/a-2710-3248).
- **Vervolgstudie 2, geen deskilling (type: prospectieve pragmatische trial; Mori is co-auteur, dus niet volledig onafhankelijk):** Pedersen, T. A., Mori, Y., Botteri, E., Engjom, T., Seip, B., Dimcevski, G. G., & Havre, R. F. (2026). *Endoscopy, 58*, 1003–1014. Dertien endoscopisten en 5.013 colonoscopieën in drie fasen (vóór, tijdens en na CADe): "In non-CADe-assisted colonoscopy, no upskilling or deskilling was observed following a period of CADe exposure" — [DOI](https://doi.org/10.1055/a-2858-7084).
- **Grote clustergerandomiseerde studie (VA, VS):** CADe verhoogde de ADR met 4,2 procentpunt. De auteurs concluderen: "potential endoscopist deskilling remains undetermined" — Dominitz, J. A., et al. (2026). *Gastroenterology* — [DOI](https://doi.org/10.1053/j.gastro.2026.05.018).
- **Redactionele commentaren:** Weinberg, D. S., & Bretthauer, M. (2026). Upskilling, deskilling, or never skilling: Who benefits from artificial intelligence in colonoscopy? *Gastroenterology, 171*, 780–781 — [DOI](https://doi.org/10.1053/j.gastro.2026.05.026). Ahmad, O. F. (2026). Human–artificial intelligence adaptation in colonoscopy: Beyond deskilling and upskilling. *Endoscopy, 58*, 1015–1016 — [DOI](https://doi.org/10.1055/a-2896-9791). Ray, K. (2025). *Nat Rev Gastroenterol Hepatol, 22*, 672 — [DOI](https://doi.org/10.1038/s41575-025-01122-3).
- **Foute weergave elders:** een scoping review noemt Budzyń ten onrechte een gerandomiseerde trial (al gemarkeerd in het eerdere rapport, bijlage G) — [Heudel et al., 2026](https://doi.org/10.1016/j.esmorw.2026.100693).

### Inferences
- De kritiek is inhoudelijk. Een voor-en-navergelijking zonder controlegroep kan werkdruk (bijna verdubbeling van het aantal procedures), organisatieveranderingen, verschillen in patiëntenmix en regressie naar het gemiddelde niet uitsluiten. Twee prospectieve studies (Okumura 2026; Pedersen 2026) vonden geen daling bij colonoscopie zonder AI. Beide zijn klein in aantal endoscopisten, en bij Pedersen is de laatste auteur van Budzyń mede-auteur. Het bewijs voor deskilling bij endoscopisten is dus **onbeslist**, niet bevestigd.
- De notitie schrijft "Ook ervaren professionals worden minder waakzaam" als feit. Budzyń et al. zelf schrijven "might reduce", en de VA-auteurs schrijven "remains undetermined". Voorgestelde formulering: "Een observationele studie bij endoscopisten vond na drie maanden AI een lagere opsporing zonder AI (22,4% tegen 28,4%). Twee latere prospectieve studies vonden die daling niet" (analyse Claude).
- Het argument in punt 6 (vaste controlemomenten, geen blind vertrouwen) hangt niet aan deze studie alleen. Het blijft staan op grond van Lee et al., Fernandes et al. en de praktijkbronnen. De studie kan als signaal blijven staan, maar niet als bewijs dat waakzaamheid afneemt.

### Gaps
- De inhoud van de drie Lancet-brieven en van het auteursantwoord is niet gelezen (paywall/403). Welke specifieke bezwaren (confounding, design) daarin staan, kon niet worden vastgesteld.
- De inhoud van het erratum (nov. 2025) is niet gecontroleerd.

## 4. Fernandes et al. (2026), Computers in Human Behavior: AI verbetert prestaties maar niet de metacognitie

### Takeaway
Er is geen externe kritiek of replicatie gevonden. De studie bevat wel een interne replicatie (Studie 2, gerandomiseerd), en die zwakt één onderdeel van de claim in de notitie af. Met AI overschatten deelnemers hun score (ongeveer 4 punten), en het Dunning-Krugerpatroon verdwijnt. Dat AI-gebruikers zich **"nog meer"** overschatten dan mensen zonder AI, steunt alleen op Studie 1: een quasi-experiment tegen een historische dataset. In het gerandomiseerde Studie 2 overschatten beide groepen zich ongeveer even sterk; de groep zonder AI zelfs iets meer in absolute zin. **Verdict: overschat** (voor "nog meer"); de rest houdbaar.

### Cited Findings
- **Studie:** Fernandes, D., Villa, S., Nicholls, S., Haavisto, O., Buschek, D., Schmidt, A., Kosch, T., Shen, C., & Welsch, R. (2026). AI makes you smarter but none the wiser: The disconnect between performance and metacognition. *Computers in Human Behavior, 175*, 108779 — [DOI](https://doi.org/10.1016/j.chb.2025.108779). Eerder verschenen als preprint (arXiv:2409.16708, 2024) — [arXiv](https://arxiv.org/abs/2409.16708v1).
- **Claim in de notitie (punt 4):** "Mensen schatten hun eigen werk met AI slecht in, meestal te hoog. Deelnemers die redeneeropgaven met AI oplosten, scoorden iets beter, maar overschatten hun prestatie nog meer."
- **Studie 1** (N = 246, ChatGPT-4o, LSAT-items, Prolific): de prestatie lag "three points" boven een normpopulatie en de overschatting was "about 4 points". De vergelijking met de dataset zonder AI (Jansen et al., 2021; N = 3.543) gaf d = 0,93 tegen d = 0,29. De auteurs voegen eraan toe: "a true experiment is needed comparing the biased estimation more closely" — [Fernandes et al., pdf](https://thomaskosch.com/wp-content/papercite-data/pdf/fernandes2025ai.pdf).
- **Studie 2** (gerandomiseerd; 250 + 250 geworven, 245 AI en 207 zonder AI geanalyseerd): "Both the AI and no-AI groups continued to overestimate their performance by similar margins … the absolute levels of performance overestimation are slightly larger for the no-AI group". In de discussie: "there was a lack of a large difference in overestimation between groups in Study 2" — [Fernandes et al., pdf](https://thomaskosch.com/wp-content/papercite-data/pdf/fernandes2025ai.pdf).
- **Beperkingen volgens de auteurs:** Studie 1 is "a quasi-experimental comparison, not a true randomized experiment … suggestive, not causal, evidence". LSAT-items kunnen in de trainingsdata zitten. Het onderzoek gebruikte één taaktype — [Fernandes et al., pdf](https://thomaskosch.com/wp-content/papercite-data/pdf/fernandes2025ai.pdf).
- **Externe kritiek/replicatie:** geen gevonden (OpenAlex: 183 citerende werken, geen comment/reply; Crossref: geen updates; webzoekactie) — [OpenAlex W4415002361](https://openalex.org/W4415002361).

### Inferences
- Wat standhoudt: met AI is de zelfinschatting fors te hoog, zwakke presteerders merken niet dat ze worstelen, en hogere AI-geletterdheid gaat samen met minder accurate zelfinschatting. Dat steunt punt 4 voldoende.
- Wat niet standhoudt in het gerandomiseerde deel: dat AI de overschatting *vergroot*. Voorgestelde formulering: "Deelnemers die met AI redeneeropgaven oplosten, scoorden beter maar overschatten hun score met ongeveer vier punten, ook de zwakste presteerders" (analyse Claude).
- Generalisatie: Amerikaanse Prolific-deelnemers, logische redeneeropgaven en GPT-4o. Dat ligt redelijk dicht bij "beoordelen van eigen analyse", maar het zijn geen hbo-studenten die onderzoek doen.

### Gaps
- De exacte aantallen en effectgroottes van de bayesiaanse vergelijking in Studie 2 zijn uit pdf-tekst gehaald (pdftotext). Symbolen kunnen verminkt zijn.

## 5. Barcaui (2025), Social Sciences & Humanities Open: ChatGPT als "cognitieve kruk", retentie na 45 dagen

### Takeaway
Er is geen gepubliceerde kritiek, reactie of replicatie gevonden. De cijfers in de notitie kloppen. De populatie (Braziliaanse bachelorstudenten bedrijfskunde) ligt dicht bij de doelgroep. De beperkingen zijn wel aanzienlijk: één universiteit, ongeveer 29% uitval vóór de toets, geen meting direct na het leren (dus leerde de groep minder of vergat ze meer?), en een confound in studietijd (3,2 uur tegen 5,8 uur). **Verdict: houdbaar met kanttekening.**

### Cited Findings
- **Studie:** Barcaui, A. (2025). ChatGPT as a cognitive crutch: Evidence from a randomized controlled trial on knowledge retention. *Social Sciences & Humanities Open, 12*, 102287 — [DOI](https://doi.org/10.1016/j.ssaho.2025.102287).
- **Claim in de notitie (punt 2):** "Bachelorstudenten die met ChatGPT studeerden, scoorden op een onaangekondigde toets na 45 dagen 57,5%. Studenten die op de gewone manier studeerden, haalden 68,5%."
- **Design (PERS, PsyPost, op basis van het artikel):**
  - 120 bachelorstudenten bedrijfskunde (FGV/UFRJ, Brazilië), twee groepen van 60.
  - Opdracht: tot twee weken onderzoek naar AI-onderwerpen en een presentatie van tien minuten.
  - Na ongeveer 45 dagen een meerkeuzetoets van 20 vragen. "Nearly thirty percent of the original 120 participants did not return" (85 van de 120).
  - De ChatGPT-groep besteedde 3,2 uur, de controlegroep 5,8 uur. Na correctie voor studietijd bleef het verschil bestaan.
  - Bron: [PsyPost](https://www.psypost.org/chatgpt-acts-as-a-cognitive-crutch-that-weakens-memory-new-research-suggests/).
- **Statistiek:** t(83) = −3,19, p = .002, d = 0,68. Dat past bij 85 geanalyseerde deelnemers, niet bij 120 (zoeksamenvatting op basis van het artikel) — [SSRN-versie](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5353041).
- **Kritiek/replicatie:** geen gevonden (OpenAlex: 130 citerende werken, geen comment/reply; Crossref: geen updates; tijdschrift zonder brievenrubriek) — [OpenAlex W4416818356](https://openalex.org/W4416818356).

### Inferences
- Zonder retentiemeting direct na de leerfase is niet te scheiden of de ChatGPT-groep minder leerde of sneller vergat. Beide wijzen wel op minder blijvende kennis (analyse Claude).
- Uitval van ongeveer 29% bij een onaangekondigde toets kan selectief zijn (wie terugkomt, is gemotiveerder). Volgens PsyPost was de uitval vergelijkbaar tussen de groepen.
- Voor de notitie is dit een relevante studie: het gaat om bachelorstudenten bedrijfskunde en een onderzoeksachtige opdracht (bronnen zoeken, presenteren). Het blijft één studie, wat de notitie impliciet erkent door haar naast Bastani en Autor te zetten.

### Gaps
- De volledige tekst (CONSORT-stroom, verdeling van de uitval per groep, preregistratie) is niet gelezen. ScienceDirect blokkeerde toegang.

## 6. Bergenholtz et al. (2026), Academy of Management Learning & Education: AI verhult verschillen tussen studenten

### Takeaway
Er is geen gepubliceerde kritiek of replicatie gevonden. Uit de artikeltekst (via een Speaker Deck-upload) blijkt een design dat de notitie te ruim weergeeft. Het ging om een **laboratoriumtaak van 22 minuten met betaalde vrijwilligers** uit een algemene proefpersonenpool, niet om een tentamen in het onderwijs. Het studiegebied van de deelnemers is niet gerapporteerd. Vooral: de claim dat **sterke studenten achteruitgingen** door AI is statistisch niet aangetoond. De voor controles gecorrigeerde behandelcoëfficiënt voor sterke studenten is −0,19 (SE 0,44, niet significant). De ruwe daling binnen die groep past bij regressie naar het gemiddelde, omdat de groepen zijn ingedeeld op de eerste taak. **Verdict: overschat** voor "sterke studenten gingen achteruit" en voor de plaatsing als "experiment in het onderwijs"; **houdbaar met kanttekening** voor "AI verhulde prestatieverschillen".

### Cited Findings
- **Studie:** Bergenholtz, C., Vuculescu, O., Günzel-Jensen, F., & Frederiksen, L. (2026). Leveling up or leveling down? The impact of generative AI on student performance in business schools. *Academy of Management Learning & Education, 25*(2), 155–186 — [DOI](https://doi.org/10.5465/amle.2025.0029).
- **Claims in de notitie:**
  - Punt 1: "In een experiment met bedrijfskundestudenten verbeterden zwakke studenten met AI, terwijl sterke studenten achteruitgingen. Zwakke studenten sloegen het analytische werk over en namen AI-uitkomsten over."
  - Punt 4: "Bij bedrijfskundestudenten verhulde AI de prestatieverschillen tussen sterke en zwakke studenten."
  - §5: "Het sterkste bewijs komt uit experimenten in het onderwijs, zoals Bastani et al. (2025) en Bergenholtz et al. (2026)".
- **Abstract:** "low performers improve while high performers decline, resulting in performance convergence"; het mechanisme heet "GenAI-Induced Cognitive Load Inversion"; "traditional assessments fail when GenAI masks performance differences" — [Aarhus University Pure](https://pure.au.dk/portal/en/publications/leveling-up-or-leveling-down-the-impact-of-generative-ai-on-stude/).
- **Design** (uit de artikeltekst op Speaker Deck, geüpload door het account "icopilots"; relatie tot de auteurs onbekend; OCR-tekst, sommige symbolen verminkt):
  - Vooraf geregistreerde RCT; 146 geworven, 141 geanalyseerd.
  - Werving via "the university's behavioral lab subject pool". Betaling ongeveer €19 plus loterij, geen studiepunten.
  - Okt.–nov. 2023, GPT-4 via de API, 22 minuten per taak.
  - Taak 1 zonder AI als nulmeting, daarna taak 2 met of zonder AI; randomisatie per sessie.
  - Beoordeeld door "two of the authors"; blindering wordt niet vermeld.
  - Bron: [Speaker Deck](https://speakerdeck.com/icopilots/leveling-up-or-leveling-down-the-impact-of-generative-ai-on-student-performance-in-business-schools).
- **Resultaten (zelfde bron):**
  - Totaal effect van AI-gebruik ongeveer +0,82 punt (SE 0,30).
  - Interactie voor zwakke presteerders (taak 1 ≤ 5) +1,79 (SE 0,60, p < .01).
  - Behandelcoëfficiënt voor sterke presteerders ongeveer −0,186 (SE 0,443), zonder significantiester.
  - De tekst meldt "their mean score decreased (p < .001)" voor de sterke presteerders binnen de AI-groep.
  - Regressie naar het gemiddelde wordt niet besproken.
  - Het studiegebied van de deelnemers is niet gerapporteerd; de 18 geïnterviewden waren "all … students at the business school".
  - Bron: [Speaker Deck](https://speakerdeck.com/icopilots/leveling-up-or-leveling-down-the-impact-of-generative-ai-on-student-performance-in-business-schools).
- **Beperkingen volgens de auteurs (zelfde bron):** één school, één casus, alleen GPT-4, vooral niet-moedertaalsprekers van het Engels, plafond in de beoordelingsschaal, longitudinaal onderzoek nodig.
- **Kritiek/replicatie:** geen gevonden (OpenAlex: 14 citerende werken; Crossref: geen updates) — [OpenAlex W7135072348](https://openalex.org/W7135072348).

### Inferences
- **Analyse Claude, geen gepubliceerde kritiek:** de groepen zijn ingedeeld op de score van taak 1. Daardoor gaan hoge scorers bij taak 2 gemiddeld vanzelf omlaag en lage scorers omhoog (regressie naar het gemiddelde). Dat geldt in beide condities. De juiste toets is dus het verschil met de controlegroep. Die is voor zwakke presteerders positief en significant, maar voor sterke presteerders −0,19 en niet significant. "Sterke studenten gingen achteruit door AI" is daarmee niet aangetoond. "AI leverde sterke studenten geen winst op" is wel verdedigbaar. De convergentie ("AI verhult verschillen") komt vooral doordat zwakke studenten meer winnen.
- Dat de beoordelaars de auteurs zelf waren, zonder vermelde blindering, is een extra risico bij een open essayopdracht (analyse Claude).
- §5 noemt dit "experimenten in het onderwijs". Het is een laboratoriumexperiment van 70 minuten met betaalde vrijwilligers, geen veldexperiment in een opleiding. Het blijft relevant voor Bedrijfskunde vanwege de open casusopdracht, maar is zwakker dan de notitie suggereert.
- Modelgeneratie: GPT-4 (2023) en 22 minuten tijdsdruk. Met nieuwere modellen en meer tijd kan het mechanisme "overweldigd raken door output" anders uitpakken. Dat geven de auteurs zelf ook aan.

### Gaps
- De versie van het tijdschrift zelf is niet gelezen (AOM blokkeerde toegang). De ontleding van de coëfficiënten komt uit een OCR-tekst van een derde partij en moet tegen het artikel worden gecontroleerd voordat de notitie wordt aangepast.

## 7. Kestin et al. (2025), Scientific Reports: de Harvard-AI-tutor

### Takeaway
Er zijn geen gepubliceerde brieven, reanalyses of onafhankelijke replicaties gevonden. Alleen niet-erkende blogs vragen om replicatie elders. De notitie geeft de studie correct weer en noemt zelf de belangrijkste beperking ("direct na de les gemeten"). Aanvullende kanttekeningen: de tutor kreeg door docenten geschreven stapsgewijze oplossingen mee, de lessen gingen over leerdoelen op het niveau "begrijpen/toepassen", en het betrof Harvard-natuurkundestudenten. **Verdict: houdbaar.**

### Cited Findings
- **Studie:** Kestin, G., Miller, K., Klales, A., Milbourne, T., & Ponti, G. (2025). AI tutoring outperforms in-class active learning: An RCT introducing a novel research-based design in an authentic educational setting. *Scientific Reports, 15*, 17458 — [DOI](https://doi.org/10.1038/s41598-025-97652-6).
- **Claim in de notitie (kanttekening punt 2):** "Een AI-tutor die studenten zelf liet redeneren, leverde Harvard-studenten natuurkunde zelfs meer leerwinst op dan actief leren in de collegezaal. De onderzoekers maten die winst direct na de les."
- **Design en effect (volledige tekst):**
  - Crossover: elke groep volgde in twee opeenvolgende weken een AI-les thuis en een actieve-leerles in de collegezaal (oppervlaktespanning, vloeistofstroming).
  - Effectgrootte lineair 0,63, met kwantielregressie 0,73–1,3 SD.
  - De prompts waren "enriched … with comprehensive, step-by-step" oplossingen, met GPT-4.
  - De auteurs noemen als randvoorwaarden onder meer "expert-crafted, question-specific prompts" en "a carefully structured framework", en de lessen richtten zich op "understanding, applying".
  - Bron: [PMC12179260](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/).
- **Kritiek/replicatie:** geen gevonden (OpenAlex: 559 citerende werken, geen comment of replicatie; Europe PMC: alleen de preprintlink naar Research Square) — [OpenAlex W4411505840](https://openalex.org/W4411505840). Een **BLOG** (ETC Journal, oktober 2026, redacteur zonder vermelde expertise in leerwetenschappen) pleit voor replicatie door onderzoekers die de tutor niet bouwden, aan andere instellingen en met minder voorbereide studenten — [ETC Journal](https://etcjournal.com/2026/10/17/the-harvard-ai-tutor-study-eleven-months-later/).

### Inferences
- De studie toont dat een zorgvuldig ontworpen, inhoudelijk "geladen" tutor kortetermijnleren op basisniveau kan versterken. Ze zegt niets over een generieke chatbot of over hogere onderzoeksvaardigheden zoals probleemformulering. De notitie gebruikt haar terecht als tegengewicht ("AI-vrije periode is niet nodig"), niet als steun voor AI bij onderzoek.

### Gaps
- Er is geen meting van retentie op langere termijn gevonden, ook niet in een vervolgstudie van dezelfde groep.

## 8. Dell'Acqua et al. (2026a), Organization Science: het BCG-experiment ("jagged frontier") en de "19 procentpunt"

### Takeaway
Er zijn geen gepubliceerde peer-reviewed commentaren gevonden, alleen blogs van niet-erkende auteurs. Het cijfer van 19 procentpunt is **verdedigbaar**: de controlegroep had 84,5% goed, de AI-groepen 70,6% (alleen GPT-4) en 60% (GPT-4 met prompttraining), gemiddeld ongeveer 19 procentpunt lager. Het abstract van *Organization Science* formuleert het wel als "19% less likely". Dat leest als een relatieve daling, die rekenkundig ongeveer 23% zou zijn. De belangrijkste kanttekening: het effect "buiten de grens" berust op **één door de onderzoekers ontworpen taak**, met GPT-4 uit 2023. **Verdict: houdbaar met kanttekening.**

### Cited Findings
- **Studie:** Dell'Acqua, F., McFowland, E., III, Mollick, E., Lifshitz, H., Kellogg, K. C., Rajendran, S., Krayer, L., Candelon, F., & Lakhani, K. R. (2026a). Navigating the jagged technological frontier. *Organization Science, 37*(2), 403–423 — [DOI](https://doi.org/10.1287/orsc.2025.21838).
- **Claim in de notitie (punt 3):** "In het bekendste experiment, met 758 BCG-consultants, werkten deelnemers met AI sneller en beter aan taken die AI goed aankan. Bij een taak net buiten dat bereik kwamen ze 19 procentpunt minder vaak tot het goede antwoord. Hun foute adviezen klonken met AI wel overtuigender."
- **Abstract van de gepubliceerde versie:** "completing 12.2% more tasks and completing them 25.1% more quickly … for a complex managerial task selected to be outside the frontier, subjects using AI were 19% less likely to produce correct solutions compared with those without AI" — [Semantic Scholar/abstract](https://api.semanticscholar.org/graph/v1/paper/DOI:10.1287/orsc.2025.21838?fields=abstract).
- **Groepspercentages:** controlegroep "answered correctly 84.5% of the time"; "accuracy fell to 70.6% for those with GPT access" en "60% for those with access and the prompt-engineering overview" — [Harvard D^3 / AI Institute](https://aiinstitute.hbs.edu/?p=29980). Co-auteur Mollick (2023): controlegroep "84% of the time", AI-groepen "60-70%" — [One Useful Thing](https://www.oneusefulthing.org/p/centaurs-and-cyborgs-on-the-jagged).
- **Werkdocument (2023):** secundaire bronnen citeren uit het HBS-werkdocument 24-013 "19 percentage points less likely to produce correct solutions" (niet zelf geverifieerd; HBS-pdf gaf 403) — [secundair overzicht](https://wphillipmoore.github.io/the-infrastructure-mindset/research/R0007-ai-cognitive-amplifier/2026-03-19/C013-bcg-outside-frontier-degradation/claim).
- **BLOG (niet-erkende auteur):** Dewar, J. M. (2026, 30 januari). *Reconsidering the jagged frontier*. Zijn argumenten:
  - Er is één taak buiten de grens tegenover achttien erbinnen, en die ene taak is ontworpen om AI te laten falen.
  - De benodigde data stonden in een bestand dat GPT-4 niet betrouwbaar kon lezen.
  - "Correctness" is alleen voor de taak buiten de grens gemeten.
  - Kwaliteitsscores (door BCG-medewerkers en MBA-studenten) waren "largely uninfluenced by whether the answer was correct or incorrect".
  - Bron: [Substack](https://reasoningwithai.substack.com/p/reconsidering-the-jagged-frontier).
- **BLOG van een leverancier (Lokad, 2024):** geen kostenmaat, niet-specialisten zonder RAG of fine-tuning, en BCG-beoordelaars (mogelijk belangenconflict) — [Lokad](https://www.lokad.com/blog/2024/4/8/a-nuanced-perspective-on-jagged-technological-frontier/).
- **Peer-reviewed kritiek/replicatie:** geen gevonden (OpenAlex: 1.673 citerende werken, geen comment/reply; Crossref: geen updates) — [OpenAlex W7135096569](https://openalex.org/W7135096569).

### Inferences
- "19 procentpunt" klopt als gemiddelde van beide AI-condities. Preciezer is: "84,5% van de consultants zonder AI kwam tot het goede antwoord, tegen 70,6% en 60% in de twee AI-groepen". Dat voorkomt verwarring met de formulering "19%" in het tijdschriftartikel (analyse Claude).
- "Foute adviezen klonken overtuigender" past bij de waarneming dat kwaliteitsscores met AI hoger lagen, ongeacht de juistheid. Die zin is niet direct tegen het artikel gecontroleerd (zie Gaps).
- De blogkritiek dat de taak buiten de grens ontworpen is om AI te laten falen, is inhoudelijk maar niet nieuw: de auteurs zeggen zelf dat de taak "selected to be outside the frontier" was. Voor de notitie verandert dat weinig. Het punt is juist dat je de grens vooraf niet ziet; de studie toont dat met één ontworpen taak, niet met een representatieve steekproef van taken.
- Modelgeneratie: GPT-4 uit 2023. De notitie noemt in §5 dat de grens opschuift.

### Gaps
- De passage over "overtuigender" foute adviezen en de exacte regressiecoëfficiënt in de *Organization Science*-versie zijn niet tegen de volledige tekst gecontroleerd (INFORMS/HBS 403).

## 9. Becker et al. (2025), METR: ervaren ontwikkelaars 19% trager

### Takeaway
De studie is nog steeds een **preprint** (arXiv v2, juli 2025, geen tijdschrift). METR zelf noemt de vertraging van 19% in februari 2026 "outdated" voor de huidige tools. De vervolgdata zijn te onbetrouwbaar door selectie-effecten. Het deel dat de notitie gebruikt, de ervaren versnelling van 20% tegenover de gemeten vertraging van 19%, is een bevinding van die ene studie met 16 ontwikkelaars, en METR heeft die perceptiekloof niet opnieuw gemeten. De notitie labelt de bron correct als preprint. **Verdict: houdbaar met kanttekening.**

### Cited Findings
- **Studie:** Becker, J., Rush, N., Barnes, E., & Rein, D. (2025). *Measuring the impact of early-2025 AI on experienced open-source developer productivity* (arXiv:2507.09089) [PREPRINT]. 16 ontwikkelaars, 246 taken. Vooraf voorspeld −24% tijd, achteraf geschat −20%, gemeten +19%. Versies: v1 12-07-2025, v2 25-07-2025; geen journal-ref — [arXiv](https://arxiv.org/abs/2507.09089).
- **Claim in de notitie (punt 4):** "Ervaren softwareontwikkelaars die met AI 19% trager werkten, dachten dat ze 20% sneller waren (Becker et al., 2025, preprint)."
- **Vervolg door METR zelf (type: follow-up van dezelfde auteurs, BLOG):**
  - Late 2025, 57 ontwikkelaars, meer dan 800 taken. De terugkerende ontwikkelaars (n = 10) waren −18% sneller (BI −38% tot +9%), nieuwe ontwikkelaars (n = 47) −4% (BI −15% tot +9%).
  - METR: "the data from our new experiment gives us an unreliable signal". Redenen: 30–50% van de ontwikkelaars hield taken achter die ze niet zonder AI wilden doen, de vergoeding daalde van $150 naar $50 per uur, en tijdregistratie met parallelle agents was onbetrouwbaar.
  - METR denkt dat ontwikkelaars nu "more sped up" zijn.
  - Bron: [METR, 24-02-2026](https://metr.org/blog/2026-02-24-uplift-update/). Op X: "Previously, we found a 20% slowdown. That finding is now outdated" — [METR op X](https://x.com/METR_Evals/status/2026355544668385373).
- **BLOG (erkende commentatoren):** Simon Willison wijst erop dat maar één ontwikkelaar meer dan 50 uur Cursor-ervaring had, en dat die wel versnelling liet zien. Volgens hem is er mogelijk "a high skill ceiling" — [Willison, 2025](https://simonwillison.net/2025/Jul/12/ai-open-source-productivity/). Zvi Mowshowitz bespreekt het ontbrekende leereffect over 30–50 uur — [Mowshowitz, 2025](https://thezvi.wordpress.com/2025/07/18/on-metrs-ai-coding-rct/). Sean Goedecke noemt het design "really good" — [Goedecke](https://www.seangoedecke.com/impact-of-ai-study/).

### Inferences
- Voor punt 4 telt niet het productiviteitscijfer maar de kloof tussen ervaren en gemeten snelheid. Die bevinding is niet weerlegd, maar ook niet gerepliceerd, en ze komt uit een kleine steekproef (N = 16) met tools uit begin 2025. Voorgestelde formulering: "In een kleine studie uit begin 2025 dachten ervaren ontwikkelaars 20% sneller te zijn met AI, terwijl ze 19% trager werkten. De onderzoekers noemen de vertraging inmiddels achterhaald, de inschattingsfout niet" (analyse Claude).
- De notitie heeft genoeg ander bewijs voor punt 4 (Scarfe, Fernandes, Bergenholtz). Becker kan blijven staan als illustratie.

### Gaps
- Er is geen nieuwe, betrouwbare meting van de perceptiekloof gevonden (2026).

## 10. Autor et al. (2026), NBER Working Paper 35720: octrooigemachtigden

### Takeaway
Het is nog steeds een **werkdocument** zonder peer review: NBER, met een geactualiseerde versie op de MIT-site in oktober 2026. Er is geen gepubliceerde methodologische kritiek gevonden. Het onderzoek is uitgevoerd met en gefinancierd door Google, dat ook de tool bouwde. De huidige weergave in de notitie is correct (eerdere fouten zijn hersteld). "Ieders conceptteksten" is iets te ruim, en de studie toont ook iets wat de samenvatting van de notitie tegenspreekt: senioren werden **beter** zonder AI na drie maanden oefenen met AI. **Verdict: houdbaar met kanttekening.**

### Cited Findings
- **Studie:** Autor, D., Rodchenko, T., Martin, J., Iscenko, Z., Strand, S., Pearl, D., & Ferere, M. (2026). *Does AI assistance enhance or erode expertise?* (NBER Working Paper No. 35720) [WERKDOCUMENT] — [DOI](https://doi.org/10.3386/w35720); [NBER pdf](https://www.nber.org/system/files/working_papers/w35720/w35720.pdf); [MIT-versie okt. 2026](https://economics.mit.edu/sites/default/files/2026-10/Does%20AI%20Assistance%20Enhance%20or%20Erode%20Expertise%20Evidence%20from%20a%20Three-Month%20Field%20Experiment%20in%20Patent%20Drafting.pdf).
- **Claim in de notitie (punt 2):** "Bij 133 octrooigemachtigden verbeterde AI de kwaliteit van ieders conceptteksten. Op een latere toets zonder AI hielden vooral de senioren winst over. Junioren gingen er gemiddeld niet op vooruit. De onderzoekers concluderen dat basiskennis nodig is om blijvend van AI te leren."
- **Resultaten (zoeksamenvatting van het werkdocument):** kwaliteit +0,34 SD na 10 dagen en +0,38 SD na 90 dagen, met grotere winst bij junioren. Op de toets zonder AI kwam het effect "entirely from senior lawyers' better redlining"; junioren "showed no average gain relative to controls" — [zoeksamenvatting op basis van NBER](https://www.nber.org/system/files/working_papers/w35720/w35720.pdf). Het eerdere rapport noemt +0,32 SD gemiddeld en +0,45 SD voor senioren — [rapport, lokaal bestand](file:///Users/witoldtenhove/Documents/HAN/afstudeeronderzoek/reports/AI%20en%20onderzoeksvaardigheden%20in%20het%20hbo.md).
- **Commentaar (BLOG van een erkende jurist, Dennis Crouch, Univ. of Missouri):** "Most of the improvement was in avoiding awful work, rather than achieving the highest quality". Bij junioren: "some saw significant skill gain and others saw significant skill reduction". De tool is Google's interne InFlow — [Patently-O, 09-09-2026](https://patentlyo.com/patent/2026/09/who-keeps-the-skill-a-randomized-trial-of-ai-patent-drafting-at-eleven-firms.html).
- **Belangen:** Google voerde het onderzoek uit en financierde het (eerder rapport, bijlage A); Google Research publiceerde een begeleidend stuk — [Google Research](https://research.google/pubs/does-ai-assistance-enhance-or-erode-expertise-evidence-from-a-three-month-field-experiment-in-patent-drafting/).
- **Kritiek/replicatie:** geen gevonden (OpenAlex: 12 citerende werken; Crossref: geen updates) — [OpenAlex W7211893772](https://openalex.org/W7211893772).

### Inferences
- "Ieders conceptteksten" moet worden "de conceptteksten gemiddeld", en vooral de slechtste teksten verbeterden (Crouch). Vermeld in de lopende tekst dat het om een werkdocument gaat; de notitie doet dat wel bij Becker ("preprint").
- Deze studie spreekt de samenvatting "Zonder AI presteren ze daarna gelijk of slechter" gedeeltelijk tegen: bij senioren leidde oefenen met AI tot betere prestaties zonder AI. Dat versterkt juist de kernboodschap van de notitie (eerst basiskennis) en verdient een plek in de samenvatting (analyse Claude; zie Kernvraag D).

### Gaps
- Het is niet gecontroleerd of de MIT-versie van oktober 2026 andere cijfers bevat dan het NBER-werkdocument.

## 11. Scarfe et al. (2024), PLOS ONE: AI-tentamens aan de University of Reading bleven onopgemerkt

### Takeaway
Er zijn geen gepubliceerde reacties, correcties of replicaties gevonden. De cijfers in de notitie kloppen. Er is één relevante uitzondering die de notitie niet noemt: in de module van het laatste studiejaar scoorden de AI-inzendingen juist **lager** dan echte studenten. Verder: GPT-4 uit 2023, thuistentamens zonder toezicht, één opleiding psychologie. **Verdict: houdbaar met kanttekening.**

### Cited Findings
- **Studie:** Scarfe, P., Watcham, K., Clarke, A., & Roesch, E. (2024). A real-world test of artificial intelligence infiltration of a university examinations system: A "Turing Test" case study. *PLOS ONE, 19*(6), e0305354 — [DOI](https://doi.org/10.1371/journal.pone.0305354).
- **Claim in de notitie (punt 4):** "In een blinde test bleef 94% van de volledig door AI geschreven tentamens onopgemerkt. Die tentamens scoorden gemiddeld hoger dan het werk van echte studenten."
- **Abstract:** "94% of our AI submissions were undetected … on average half a grade boundary higher"; "an 83.4% chance that the AI submissions on a module would outperform a random selection" — [PMC11206930](https://pmc.ncbi.nlm.nih.gov/articles/PMC11206930/).
- **Uitzondering in de volledige tekst:** "For four out of five modules AI submissions on average gained higher grades … The exception being the finalist module P3-M1", waar "AI submissions outperformed real students in 19% of cases" — [PMC11206930](https://pmc.ncbi.nlm.nih.gov/articles/PMC11206930/).
- **Kritiek/replicatie:** geen gevonden (OpenAlex: 186 citerende werken, geen comment/reply; Europe PMC: geen commentaarlink; webzoekactie) — [OpenAlex W4400037475](https://openalex.org/W4400037475). Verwant en onafhankelijk: Kofinas et al. (2025, *BJET*), al opgenomen in het eerdere rapport — [DOI](https://doi.org/10.1111/bjet.13585).

### Inferences
- De uitzondering in het laatste studiejaar is relevant voor de notitie. Bij het meest gevorderde werk deed GPT-4 (2023) het slechter dan studenten. Met huidige modellen is dat mogelijk anders. Het onopgemerkt blijven (94%) is het robuuste deel. Het "hoger scoren" geldt niet voor het meest gevorderde niveau (analyse Claude).

### Gaps
- Er is geen replicatie met nieuwere modellen aan dezelfde of een andere instelling gevonden.

## 12. Linardon et al. (2025), Walker & Larson (2025), Bisbee et al. (2024), Sarstedt et al. (2024) en Westwood (2025)

### Takeaway
Voor Linardon, Walker & Larson, Bisbee en Sarstedt is geen gepubliceerde kritiek, correctie of reanalyse gevonden. Latere preprints bevestigen het kernprobleem van Bisbee (te weinig spreiding). Rond **Westwood** is wel een inhoudelijk debat ontstaan, met een PNAS-briefwisseling, een tegenstudie in PNAS en een door een leverancier gefinancierde preprint. Dat debat gaat over hoe vaak AI-agents in de praktijk voorkomen en of ze op te sporen zijn, niet over Westwoods demonstratie zelf. De zin in de notitie "AI-bots doorstonden 99,8% van de aandachtscontroles in online enquêtes" is iets te ruim. Het ging om één door de onderzoeker gebouwde agent in 6.000 testrondes, niet om bots die in echte enquêtes zijn waargenomen. **Verdicten:** Linardon *houdbaar met kanttekening*; Walker & Larson *houdbaar* (geen empirische claim); Bisbee *houdbaar met kanttekening*; Sarstedt *houdbaar*; Westwood *houdbaar met kanttekening*.

### Cited Findings
- **Linardon et al. (2025)** (punt 3: "GPT-4o verzon in 2025 een op de vijf referenties, en bijna de helft van de echte referenties bevatte fouten"):
  - Juni 2025, GPT-4o, zes literatuuroverzichten, 176 referenties. 35 (19,9%) waren verzonnen; van de 141 echte bevatten er 64 (45,4%) fouten.
  - Verzinnen varieerde van 6% (depressie) tot 28–29% (minder bekende stoornissen) en 46% bij gespecialiseerde reviews over eetbuistoornis.
  - Bron: [PMC12658395](https://pmc.ncbi.nlm.nih.gov/articles/PMC12658395/); [DOI](https://doi.org/10.2196/80371).
  - Geen comments of correcties (Crossref; OpenAlex 77 citerende werken) — [Crossref](https://api.crossref.org/works/10.2196/80371).
- **Walker & Larson (2025)** (punt 7, voorbeeldopdracht): een onderwijsontwerp met evaluatie, zonder numerieke claim in de notitie. Geen updates in Crossref — [DOI](https://doi.org/10.1177/10525629241294075).
- **Bisbee et al. (2024)** (punt 5: "Synthetische respondenten treffen gemiddelden goed, maar hebben te weinig spreiding en veranderen met kleine wijzigingen in de vraag"):
  - De studie gebruikte ChatGPT-3.5 met personas uit ANES 2016/2020 — [Political Analysis pdf](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/B92267DC26195C7F36E63EA04A47D2FE/S1047198724000056a.pdf/div-class-title-synthetic-replacements-for-human-survey-data-the-perils-of-large-language-models-div.pdf); [DOI](https://doi.org/10.1017/pan.2024.5).
  - Geen formele reanalyse of weerlegging gevonden. Latere **PREPRINTS** reproduceren het probleem van te weinig spreiding en stellen correcties voor die de systematische vertekening niet volledig wegnemen — [arXiv:2607.28550](https://arxiv.org/html/2607.28550v1); [arXiv:2610.30900](https://arxiv.org/pdf/2610.30900).
- **Sarstedt et al. (2024)** (punt 5): een review met richtlijnen. Geen updates of commentaren gevonden (Crossref; OpenAlex 233 citerende werken) — [DOI](https://doi.org/10.1002/mar.21982).
- **Westwood (2025)** (punt 5: "AI-bots doorstonden bovendien 99,8% van de aandachtscontroles in online enquêtes"):
  - Abstract: "I designed and tested an autonomous synthetic respondent … achieving a 99.8% pass rate on 6,000 trials of standard attention checks" — [PMC12663962](https://pmc.ncbi.nlm.nih.gov/articles/PMC12663962/); [DOI](https://doi.org/10.1073/pnas.2518075122).
  - **PNAS-brief (type: letter):** Van der Stigchel, S., Strauch, C., de Zwart, B., & Van Maanen, L. (2026). Will online behavioral research follow the fate of online survey research? *PNAS, 123*(8), e2535585123 — [DOI](https://doi.org/10.1073/pnas.2535585123). Inhoud niet gelezen; de titel suggereert dat de brief de zorg uitbreidt naar online gedragsonderzoek.
  - **Antwoord (type: reply):** Westwood, S. J., & Frederick, S. (2026). Reply to Van der Stigchel et al.: Empirical evidence that AI survey contamination is real and substantial. *PNAS, 123*(8), e2537420123 — [DOI](https://doi.org/10.1073/pnas.2537420123).
  - **Kritische brief, afgewezen door PNAS en als PREPRINT gepubliceerd:** Rothschild, D. M., Barari, S., Buskirk, T. D., Gordon, A., & Hillygus, D. S. (2026). Reply to Westwood: Questioning the empirical evidence that AI survey contamination is real and substantial. Belangen: "A.G. works for Prolific and D.M.R. previously advised Prolific". Argumenten:
    - Westwood haalt drie fenomenen door elkaar: hulp door een LLM bij het antwoorden, eenvoudige invulling door een agent, en autonome agents binnen een panel.
    - Er ontbreken passende benchmarks.
    - Westwood "withholds its code".
    - Bron: [ResearchDMR pdf](https://researchdmr.com/files/Letter_Westwood.pdf).
  - **Onafhankelijke empirische studie (peer-reviewed):** Zhang, G., Walatka, R., Chen, S. Y., Moore, A. K., Urminsky, O., Fernandez, K., Low, A., Bogard, J. E., & Fox, C. R. (2026). Estimating the threat of AI-agent responding across online survey platforms. *PNAS*. De gevalideerde AI-detectietests scheidden mensen van agents. Op zeven platforms faalde 6–41% van de respondenten op die tests, tegen 2,4% fout-positieven bij mensen ter plaatse. Onopgemerkte agents kunnen uitkomsten beïnvloeden — [DOI](https://doi.org/10.1073/pnas.2606460123).
  - **PREPRINT van een LEVERANCIER (Prolific):** minder dan 1% niet-menselijke antwoorden bij 12 aanbieders en ongeveer 16% bij één aanbieder (MTurk). De eigen checker ving alle 125 AI-ingevulde enquêtes. Westwood weigerde mee te werken en wees op het financiële belang van Prolific — [Retraction Watch, 30-04-2026](https://retractionwatch.com/2026/04/30/are-ai-chatbots-infiltrating-online-survey-data-not-yet-says-new-study/).
  - Westwood won met deze studie de Cozzarelli Prize van PNAS (2025) — [Dartmouth](https://fas.dartmouth.edu/news/2026/04/sean-westwood-wins-pnas-prize-ai-polling-study).

### Inferences
- Linardon: "taalmodellen" generaliseert vanuit één model (GPT-4o) in één domein. De spreiding naar onderwerp (6% tot 46%) is voor de notitie juist nuttig: bij nichethema's, zoals veel afstudeeronderwerpen bij Bedrijfskunde, verzint een model vaker. Het eerdere rapport noemt een bredere bandbreedte (20–40% verzonnen referenties).
- Bisbee: de kern (te weinig spreiding) wordt in latere preprints bevestigd. De studie gebruikte wel GPT-3.5. Voorgestelde aanvulling: "ook bij nieuwere modellen blijft de spreiding te klein" kan alleen op preprints steunen.
- Westwood: de demonstratie (een agent haalt standaard-aandachtscontroles) staat. Omstreden is hoe vaak het in de praktijk gebeurt (Zhang: 6–41% per platform; Prolific: minder dan 1% bij de meeste) en of detectie kansloos is (Zhang: gevalideerde tests werken). Voorgestelde formulering: "Een door een onderzoeker gebouwde AI-agent doorstond 99,8% van de standaard-aandachtscontroles. Hoe vaak zulke agents echte enquêtes invullen, verschilt sterk per platform" (analyse Claude). Voor de KSAVE-aanbeveling (synthetische data kritisch beoordelen, cluster E) versterkt het debat de notitie eerder dan dat het haar verzwakt.

### Gaps
- De inhoud van de brief van Van der Stigchel et al. en van het antwoord van Westwood & Frederick is niet gelezen.

## 13. Overige empirische studies met een numerieke claim in de notitie

### Takeaway
Voor geen van deze studies is gepubliceerde kritiek, een correctie of een intrekking gevonden (Crossref: geen updates). Bij drie studies is de weergave iets te ruim: Wu et al. (het percentage hoort grotendeels bij LLM's zonder zoekfunctie), Balt et al. (kappa 0,68 geldt voor de makkelijkere deeltaak) en Allen & McDonald ("daardoor" is causaler dan "partially explained").

### Cited Findings
- **Wu et al. (2025), *Nature Communications*** (punt 3: "Bij medische vragen werd 50 tot 90% van de antwoorden niet volledig gedragen door de geciteerde bronnen", toegeschreven aan "AI-zoektools met bronvermelding"). De 50–90% geldt voor zeven LLM's. Voor GPT-4o met webzoekfunctie (RAG) was ongeveer 30% van de losse beweringen niet gedragen, en "nearly half" van de antwoorden niet volledig gedragen (zoeksamenvatting van het artikel) — [DOI](https://doi.org/10.1038/s41467-025-58551-6). Geen kritiek gevonden. **Verdict: houdbaar met kanttekening.** Voor zoektools met bronvermelding is "ongeveer de helft" preciezer dan "50 tot 90%".
- **Lau & Golder (2025), *Cochrane Evidence Synthesis and Methods*** (punt 3: Elicit 39,5% tegen 94,5%). Bevestigd: "sensitivity of Elicit was poor, averaging 39.5% (25.5–69.2%) compared to 94.5%". Het artikel doorliep open peer review in meerdere rondes (Crossref-relaties v1–v4) — [DOI](https://doi.org/10.1002/cesm.70050); [Crossref](https://api.crossref.org/works/10.1002/cesm.70050). Elicit publiceerde een eigen evaluatie (**LEVERANCIER**) die screening meet, niet de sensitiviteit van het zoeken, en reageert niet op Lau & Golder — [Elicit-blog](https://elicit.com/blog/how-we-evaluated-elicit-systematic-review). **Verdict: houdbaar met kanttekening** (vier casussen, versie van Elicit ten tijde van de evaluatie).
- **Balt et al. (2025), *Frontiers in Public Health*** (punt 5: "overeenstemming van 0,68 (Cohens kappa)"). De volledige tekst laat zien dat κ = 0,68 hoort bij de binaire classificatie van vooraf gesegmenteerde fragmenten. De realistischere sliding-windowtaak haalde een nauwkeurigheid van 0,67, met grote variatie per code en hallucinaties in samenvattingen — [PMC11879832](https://pmc.ncbi.nlm.nih.gov/articles/PMC11879832/). **Verdict: houdbaar met kanttekening.**
- **Allen & McDonald (2026), *Strategy Science*** (punt 1: "kozen de nieuwste taalmodellen stelselmatig voor het bestaande product … Daardoor scoorden ze lager dan MBA-studenten"). Abstract: frontiermodellen van medio tot eind 2025 (GPT-5, Claude Opus 4.5, Gemini 3) "underperforming both earlier LLMs and MBA students. This decline is partially explained by a systematic bias toward exploiting the core business" — [DOI](https://doi.org/10.1287/stsc.2025.0444). **Verdict: houdbaar met kanttekening** ("daardoor" vervangen door "deels doordat"; redeneermodellen van eind 2024 tot begin 2025 scoorden juist hoger dan MBA-studenten).
- **Boussioux et al. (2024), *Organization Science*** (punt 5): "human crowd solutions exhibited higher novelty … human-AI solutions demonstrated superior strategic viability, financial and environmental value, and overall quality" — [DOI](https://doi.org/10.1287/orsc.2023.18430). **Verdict: houdbaar.**
- **Gonsalves (2025), *Assessment & Evaluation in Higher Education*** (punt 4: 74% vulde de AI-verklaring niet in): "74% of students failed to declare AI usage despite declaration being a requirement" (King's Business School) — [DOI](https://doi.org/10.1080/02602938.2024.2415654). **Verdict: houdbaar.**
- **Dell'Acqua et al. (2026b), *Organization Science*** (punt 7: individuen met AI haalden het niveau van teams zonder AI; punt 1: AI verbetert vooral ideeën, het menselijk oordeel houdt waarde bij selectie). Het abstract bevestigt beide: "individuals with AI matched the performance of teams without AI" en "human judgment retains value in evaluative selection" — [DOI](https://doi.org/10.1287/orsc.2025.20702). **Verdict: houdbaar.**

### Inferences
- Bij foutpercentages van AI-tools (Wu, Linardon, Lau & Golder) zegt de notitie in §5 al dat ze snel verouderen. Dat is de juiste algemene kanttekening.

### Gaps
- Niet gecontroleerd: "Vier van de zes verzonnen er zelf een" (Allen & McDonald), "In het P&G-experiment onderschatten deelnemers hun werk juist" (Dell'Acqua 2026b) en Kumar et al. (2025). Kumar is in het eerdere rapport geverifieerd en hier niet opnieuw nagelopen.

## 14. Gerlich (2025) en Kosmyna et al. ("Your brain on ChatGPT"): status ter bevestiging

### Takeaway
De notitie citeert Gerlich (2025) **niet** (bibliografie gecontroleerd). Het artikel heeft een correctie ("Error in Table") en is correlationeel en gebaseerd op zelfrapportage. Een peer-reviewed commentaar is niet gevonden. Kosmyna et al. is per november 2026 **nog steeds een preprint** (arXiv v2, 31-12-2025, geen tijdschrift) met een methodologisch commentaar (preprint). De notitie beschrijft dat in §5 correct. Correlationeel werk dat lijkt op Gerlich speelt in de notitie alleen een rol via Lee et al. (enquête) en de bestuurdersinterviews (BCG/Goel; Bevilacqua). De centrale claims rusten op experimenten. **Verdict: de omgang van de notitie met beide bronnen is houdbaar.**

### Cited Findings
- **Gerlich:** Gerlich, M. (2025). AI tools in society: Impacts on cognitive offloading and the future of critical thinking. *Societies, 15*(1), 6 — [DOI](https://doi.org/10.3390/soc15010006). Correctie: *Societies, 15*(9), 252, gepubliceerd 10-09-2025, abstract "Error in Table" — [Semantic Scholar](https://api.semanticscholar.org/graph/v1/paper/DOI:10.3390/soc15090252?fields=title,abstract,year,publicationDate); [DOI](https://doi.org/10.3390/soc15090252). Volgens een secundaire bron ging het om een gedupliceerde tabel en bleven de conclusies volgens de auteur ongewijzigd (niet geverifieerd; MDPI 403). Kritiek in blogs en overzichten richt zich op het correlationele design en zelfgerapporteerd AI-gebruik ("either heavy AI use erodes critical thinking, or weaker critical thinkers lean on AI harder") — [mindmargin.org](https://mindmargin.org/research/gerlich-cognitive-offloading). OpenAlex: 2.502 citerende werken, geen comment/reply — [OpenAlex W4406026056](https://openalex.org/W4406026056).
- **Kosmyna:** arXiv:2506.08872, v1 10-06-2025, v2 31-12-2025, geen journal-ref; 54 deelnemers, 18 in sessie 4 — [arXiv](https://arxiv.org/abs/2506.08872).
  - **Commentaar (PREPRINT):** Stankovic, M., Hirche, E., Kollatzsch, S., & Doetsch, J. N. (2025). *Comment on: Your brain on ChatGPT* (arXiv:2601.00856). Bezwaren over het design (kleine steekproef), de reproduceerbaarheid, de EEG-analyse, inconsistente rapportage en transparantie — [arXiv](https://arxiv.org/abs/2601.00856).
  - **Peer-reviewed bron die de status bevestigt:** Campos, J. P., & Koff, T. (2026, 8 juli). Your brain on ChatGPT, but whose brain? *Frontiers in Developmental Psychology* (Hypothesis & Theory): "It is a preprint, not yet through peer review, and a critical comment on its methods has already appeared"; "lower neural activity need not mean worse cognition" — [DOI](https://doi.org/10.3389/fdpys.2026.1885225).
  - **PERS:** Kosmyna waarschuwt zelf tegen overinterpretatie — [Scientific American](https://www.scientificamerican.com/article/does-using-chatgpt-really-change-your-brain-activity/).

### Inferences
- De keuze om beide bronnen niet als bewijs te gebruiken is verdedigbaar en actueel.
- Lee et al. heeft hetzelfde type zwakte als Gerlich (zelfrapportage, correlationeel), al met beter gedocumenteerde beperkingen en een correct label in de notitie. Zie studie 2.

### Gaps
- De inhoud van de Gerlich-correctie is niet zelf gelezen.

## Kernvraag A: welke studies kregen gepubliceerd commentaar, brieven of reanalyses, en hoe sterk zijn de bezwaren?

### Takeaway
Alleen bij **Budzyń** (inhoudelijk sterke bezwaren plus twee studies die het effect niet vonden) en **Westwood** (debat over hoe vaak AI-agents voorkomen en of ze op te sporen zijn, niet over de demonstratie zelf) is er gepubliceerde discussie. Bij **Bastani** gaat de enige correctie over een affiliatie. Bij de overige kernstudies is na een echte zoektocht geen gepubliceerde kritiek gevonden. De sterkste problemen die dit onderzoek aan het licht bracht, komen uit de studies zelf: de gerandomiseerde Studie 2 van **Fernandes**, de coëfficiënt voor sterke studenten bij **Bergenholtz** en de uitzondering in de laatstejaarsmodule bij **Scarfe**.

### Cited Findings
- Budzyń: Ahmad-commentaar, drie Lancet-brieven, auteursantwoord en erratum; expertreacties over werkdruk en organisatieverandering; Okumura (2026) en Pedersen (2026) vinden geen deskilling — [Europe PMC-lijst](https://europepmc.org/search?query=TITLE%3A%22deskilling%22%20AND%20TITLE%3A%22colonoscopy%22); [SMC](https://www.sciencemediacentre.org/expert-reaction-to-observational-study-looking-at-detection-rate-of-precancerous-growths-in-colonoscopies-by-health-professionals-who-perform-them-before-and-after-the-routine-introduction-of-ai/); [Pedersen et al., 2026](https://doi.org/10.1055/a-2858-7084).
- Westwood: PNAS-brief en antwoord; de afgewezen Rothschild-brief; Zhang et al. (2026) in PNAS — [Westwood & Frederick, 2026](https://doi.org/10.1073/pnas.2537420123); [Zhang et al., 2026](https://doi.org/10.1073/pnas.2606460123).
- Bastani: alleen een correctie van een affiliatie — [PMC12403119](https://pmc.ncbi.nlm.nih.gov/articles/PMC12403119/).
- Kosmyna (niet geciteerd als bewijs): commentaar als preprint — [arXiv:2601.00856](https://arxiv.org/abs/2601.00856).

### Inferences
- Weinig formele kritiek betekent hier vooral dat de studies jong zijn (2025–2026) en vaak in tijdschriften zonder brievenrubriek staan. Het is geen bewijs van robuustheid.

### Gaps
- PubPeer kon niet betrouwbaar worden doorzocht.

## Kernvraag B: zijn studies in 2025–2026 (on)succesvol gerepliceerd door onafhankelijke teams?

### Takeaway
Echte onafhankelijke replicaties zijn zeldzaam. **Budzyń** is twee keer niet gerepliceerd, in kleine prospectieve studies. De kern van **Westwood** is bevestigd (agents kunnen standaardcontroles halen), maar de stelling dat detectie kansloos is, wordt tegengesproken. Het spreidingsprobleem van **Bisbee** is in preprints gereproduceerd. **Fernandes** repliceerde zichzelf maar ten dele. Voor **Bastani, Barcaui, Bergenholtz, Kestin, Dell'Acqua 2026a, Scarfe, Lee en Autor** is geen replicatie gevonden. **METR** (Becker) noemt de eigen bevinding achterhaald.

### Cited Findings
- Okumura et al. (2026) — [DOI](https://doi.org/10.1055/a-2661-2624); Pedersen et al. (2026) — [DOI](https://doi.org/10.1055/a-2858-7084).
- Zhang et al. (2026) — [DOI](https://doi.org/10.1073/pnas.2606460123).
- Fernandes Studie 2 — [pdf](https://thomaskosch.com/wp-content/papercite-data/pdf/fernandes2025ai.pdf).
- METR-vervolg — [METR, 2026](https://metr.org/blog/2026-02-24-uplift-update/).
- Verwante nieuwe evidentie die het patroon "met AI beter, zonder AI slechter" nuanceert: Contractor & Reyes (2026, PREPRINT) — [arXiv](https://arxiv.org/abs/2607.08849).

### Inferences
- Het bewijs voor "eerst zelf, dan AI" rust op een handvol losse studies met verschillende populaties. Ze wijzen wel dezelfde richting op (het gebruikspatroon is doorslaggevend), maar zijn niet gerepliceerd.

### Gaps
- Er is geen replicatie van een experiment in het hoger onderwijs (Barcaui, Bergenholtz) door een ander team gevonden.

## Kernvraag C: zijn preprints en werkdocumenten inmiddels peer-reviewed, en veranderden de resultaten?

### Takeaway
**Becker/METR** (arXiv), **Autor et al.** (NBER, nieuwe versie oktober 2026) en **Kosmyna** (arXiv v2) zijn per 18-11-2026 niet peer-reviewed gepubliceerd. Bij studies die van werkdocument naar tijdschrift gingen, bleven de kerncijfers volgens de abstracts gelijk: Bastani (SSRN 2024 → PNAS 2025: 48/127/17%), Dell'Acqua 2026a (HBS WP 2023 → *Organization Science* 2026: 12,2%/25,1%/19), Fernandes (arXiv 2024 → CHB 2026, Studie 2 al in de preprint) en Kestin (Research Square → *Scientific Reports*). Wel veranderde in Dell'Acqua de **formulering** van "19 percentage points" (werkdocument, volgens secundaire bronnen) naar "19% less likely" (tijdschrift).

### Cited Findings
- Becker: geen journal-ref — [arXiv](https://arxiv.org/abs/2507.09089).
- Autor: NBER WP en MIT-versie okt. 2026 — [NBER](https://www.nber.org/system/files/working_papers/w35720/w35720.pdf); [MIT](https://economics.mit.edu/sites/default/files/2026-10/Does%20AI%20Assistance%20Enhance%20or%20Erode%20Expertise%20Evidence%20from%20a%20Three-Month%20Field%20Experiment%20in%20Patent%20Drafting.pdf).
- Kosmyna: v2, geen journal-ref — [arXiv](https://arxiv.org/abs/2506.08872).
- Bastani, SSRN-versie — [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4895486); PNAS-abstract — [PMC12232635](https://pmc.ncbi.nlm.nih.gov/articles/PMC12232635/).
- Dell'Acqua 2026a, tijdschriftabstract "19% less likely" — [DOI](https://doi.org/10.1287/orsc.2025.21838).
- Fernandes, preprint met Studie 2 — [arXiv:2409.16708](https://arxiv.org/abs/2409.16708v1).
- Kestin, preprintrelatie in Crossref — [Crossref](https://api.crossref.org/works/10.1038/s41598-025-97652-6).

### Inferences
- De notitie labelt Becker correct als preprint. Autor staat als werkdocument in de bibliografie, maar niet in de lopende tekst.

### Gaps
- Een systematische vergelijking tussen de preprint- en tijdschriftversies op het niveau van tabellen is niet uitgevoerd.

## Kernvraag D: claimt de notitie meer dan de studies tonen (populatie, design, modelgeneratie)?

### Takeaway
Op drie plaatsen gaat de notitie aantoonbaar verder dan de studie: **Budzyń** (causale, algemene formulering bij een observationele voor-en-nastudie die niet gerepliceerd is), **Fernandes** ("nog meer" overschatten steunt alleen op het quasi-experiment) en **Bergenholtz** (een niet-significante "achteruitgang" van sterke studenten, en een labtaak gepresenteerd als experiment in het onderwijs). De samenvatting "Experimenten laten een vast patroon zien … Zonder AI presteren ze daarna gelijk of slechter" is te stellig. Autor (senioren), Kestin, Contractor & Reyes (preprint) en de tutorarm van Bastani laten zien dat de uitkomst afhangt van het gebruikspatroon. Kleinere onnauwkeurigheden: Westwood (één gebouwde agent, geen waargenomen bots), Wu (het percentage hoort grotendeels bij LLM's zonder zoekfunctie), Balt (kappa van de makkelijkere deeltaak), Allen & McDonald ("daardoor") en Autor ("ieders"). Bijna alle studies gebruikten GPT-3.5, GPT-4 of GPT-4o uit 2023–2025. De notitie erkent dat in §5.

### Cited Findings

| Studie | Populatie | Design | Model | Verdict |
|---|---|---|---|---|
| Bastani et al. 2025 | Turkse leerlingen, leerjaren 9–11 (K-12) | veld-RCT | GPT-4 (2023) | houdbaar met kanttekening |
| Lee et al. 2025 | 319 kenniswerkers (Prolific) | enquête, zelfrapportage | diverse (2024) | houdbaar met kanttekening |
| Budzyń et al. 2025 | endoscopisten in 4 Poolse centra (volgens secundaire bron 19) | observationeel, voor-en-na | CADe | **overschat** |
| Fernandes et al. 2026 | Prolific (VS), LSAT | quasi-experiment plus RCT | GPT-4o | **overschat** ("nog meer") |
| Barcaui 2025 | 120 bachelorstudenten bedrijfskunde, Brazilië | RCT, 29% uitval | ChatGPT | houdbaar met kanttekening |
| Bergenholtz et al. 2026 | 141 betaalde vrijwilligers uit een labpool, Aarhus | lab-RCT, 22 min | GPT-4 (2023) | **overschat** (sterke studenten); houdbaar met kanttekening (verhullen) |
| Kestin et al. 2025 | 194 Harvard-natuurkundestudenten | crossover-RCT, directe meting | GPT-4 met uitgewerkte oplossingen | houdbaar |
| Dell'Acqua et al. 2026a | 758 BCG-consultants | veldexperiment | GPT-4 (2023) | houdbaar met kanttekening |
| Becker et al. 2025 | 16 ontwikkelaars | RCT, PREPRINT | AI-tools begin 2025 (o.a. Cursor) | houdbaar met kanttekening |
| Autor et al. 2026 | 133 octrooigemachtigden | veld-RCT, WERKDOCUMENT | Google InFlow | houdbaar met kanttekening |
| Scarfe et al. 2024 | psychologie, Reading | blinde veldtest | GPT-4 (2023) | houdbaar met kanttekening |
| Linardon et al. 2025 | GPT-4o, geestelijke gezondheid | experiment | GPT-4o | houdbaar met kanttekening |
| Bisbee et al. 2024 | ANES-personas | vergelijking | GPT-3.5 | houdbaar met kanttekening |
| Sarstedt et al. 2024 | review/richtlijnen | n.v.t. | n.v.t. | houdbaar |
| Westwood 2025 | gebouwde agent, 6.000 trials | demonstratie | diverse LLM's | houdbaar met kanttekening |
| Wu et al. 2025 | medische vragen, 7 LLM's | evaluatie | o.a. GPT-4o (RAG) | houdbaar met kanttekening |
| Balt et al. 2025 | 38 NL-interviews | evaluatie | Llama 3 (lokaal) | houdbaar met kanttekening |
| Allen & McDonald 2026 | 34 LLM's, strategiesimulatie | benchmark | t/m GPT-5, Opus 4.5, Gemini 3 | houdbaar met kanttekening |

- Bronnen per regel: zie de secties 1–13 hierboven.
- Tegenvoorbeelden bij "vast patroon": senioren +0,45 SD zonder AI na oefenen met AI — [Autor et al., 2026](https://www.nber.org/system/files/working_papers/w35720/w35720.pdf); AI-toegang verhoogde scores op toetsen zonder hulp, ook na een week — [Contractor & Reyes, 2026, PREPRINT](https://arxiv.org/abs/2607.08849); 0,73–1,3 SD meer leerwinst — [Kestin et al., 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/).

### Inferences
- Voorgestelde herformulering van "In het kort" (analyse Claude): "Experimenten laten zien dat AI de prestatie met AI bijna altijd verhoogt. Wat zonder AI overblijft, hangt af van hoe AI is gebruikt: wie het denkwerk aan AI overlaat, presteert daarna gelijk of slechter; wie eerst zelf werkt of AI als tutor gebruikt, houdt winst over."
- De drie aanbevelingen van de notitie (eerst zelf werken, AI-uitkomsten leren controleren, toetsen zonder AI) blijven overeind. Geen ervan hangt aan een studie die is weerlegd of ingetrokken. De correcties gaan over formulering en stelligheid, niet over richting.

### Gaps
- Geen enkele gevonden studie test onderzoeksvaardigheden zoals probleemformulering of onderzoeksontwerp bij hbo-studenten. De notitie erkent dat in §5.
