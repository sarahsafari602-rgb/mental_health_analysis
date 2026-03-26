# Mental Health Survey Analysis

## Problem
Analyse von Faktoren, die beeinflussen, ob Personen eine Behandlung für psychische Probleme in Anspruch nehmen. Ziel ist es, typische Muster in den Daten zu erkennen und Data-Analytics-Fähigkeiten zu demonstrieren.

## Datensatz
- Quelle: Kaggle (Mental Health in Tech Survey)  
- Größe: ca. 1200 Zeilen, 10 Spalten  
- Relevante Spalten: treatment, gender, age, work_environment, family_status  

## Vorgehensweise
1. **Datenbereinigung**  
   - Gender-Kategorien vereinheitlicht  
   - Fehlende Werte geprüft und behandelt  
   - Timestamp angepasst  
   - Irrelevante Spalten entfernt  

2. **Explorative Analyse (EDA)**  
   - Gender  vs. Treatment
   - Age vs. Treatment
   - Family History vs. Treatment
   - Remote Work vs. Treatment
   - Work Interfere vs. Treatment
   - Unternehmensgröße vs. Treatment

3. **Visualisierung**  
   - (gruppierte) Balkendiagramme für die wichtigsten Zusammenhänge
   - Prozentzahlen sind direkt über den Balken dargestellt, um die Unterschiede klar zu zeigen.  
 
## Ergebnisse
## Explorative Analyse: Gender vs. Treatment
**Fragestellung:** 
    - Untersuchung des Anteils an Personen, die sich für eine Behandlung entscheiden, aufgeteilt nach Gender.
**Kategorien:**
    - Gender: Male, Female, Unknown (einschließlich Cis, Binär, Trans etc.)
    - Treatment: Yes / No
**Beobachtungen:**
69,5 % der Frauen haben Treatment gewählt.
45,3 % der Männer haben Treatment gewählt.
65,9 % der Personen in der Unknown-Kategorie haben Treatment gewählt.

**Statistik:**
Ein Chi-Quadrat-Test zeigt, dass die Unterschiede im Treatment-Verhalten zwischen den Gender-Gruppen statistisch signifikant sind (χ² = 49,14, p < 0,001). 
Die Effektgröße nach Cramér’s V beträgt 0,198, was einen kleinen bis moderaten Zusammenhang anzeigt.

## Explorative Analyse: Age vs. Treatment
**Fragestellung:**
Untersuchung des Anteils an Personen, die sich für eine Behandlung entscheiden, aufgeteilt nach Altersgruppen.
**Kategorien:**
    - Age Group: 0-20, 21-30, 31-40, 41-50, 51-60, 61-70, 71+
    - Treatment: Yes / No
**Beobachtungen:**
Die prozentuale Verteilung von Treatment Yes/No unterscheidet sich nur geringfügig zwischen den Altersgruppen.
Es gibt kein klares Muster, das darauf hindeutet, dass Alter die Treatment-Entscheidung stark beeinflusst.
**Statistik:**
Ein Chi-Quadrat-Test zeigt, dass die Unterschiede im Treatment-Verhalten zwischen den Altersgruppen nicht signifikant sind (χ² = 9,71, p = 0,137).
Die Effektgröße nach Cramér’s V beträgt 0,088, was auf einen sehr kleinen Zusammenhang hinweist.

## Explorative Analyse: Family History vs. Treatment
**Fragestellung:**
Untersuchung des Anteils an Personen, die sich für eine Behandlung entscheiden, abhängig von einer familiären Vorgeschichte psychischer Erkrankungen.
**Kategorien:**
    - Family History: Yes / No
    - Treatment: Yes / No
**Beobachtungen:**
Personen mit familiärer Vorgeschichte wählen deutlich häufiger Treatment als Personen ohne.
**Statistik:**
Ein Chi-Quadrat-Test zeigt, dass die Unterschiede im Treatment-Verhalten zwischen den Gruppen statistisch signifikant sind (χ² = 178,27, p < 0,001).
Die Effektgröße nach Cramér’s V beträgt 0,376, was auf einen mittleren bis starken Zusammenhang hinweist.

## Explorative Analyse: Remote Work vs. Treatment
**Fragestellung:**
Untersuchung des Anteils an Personen, die sich für eine Behandlung entscheiden, abhängig davon, ob sie remote arbeiten.
**Kategorien:**
    - Remote Work: Yes / No
    - Treatment: Yes / No
**Beobachtungen:**
Die prozentuale Verteilung von Treatment Yes/No unterscheidet sich nur minimal zwischen den Gruppen.
**Statistik:**
Ein Chi-Quadrat-Test zeigt, dass die Unterschiede nicht signifikant sind (χ² = 0,80, p = 0,371).
Die Effektgröße nach Cramér’s V beträgt 0,025, was auf praktisch keinen Zusammenhang hinweist.

## Explorative Analyse: Work Interfere vs. Treatment
**Fragestellung:**
Untersuchung des Anteils an Personen, die sich für eine Behandlung entscheiden, abhängig davon, wie stark die Arbeit das Privatleben beeinflusst.
**Kategorien:**
    - Work Interfere: Never, Rarely, Sometimes, Often, NA
    - Treatment: Yes / No
**Beobachtungen:**
Mit steigender Beeinträchtigung durch Arbeit („Often“) steigt auch der Anteil der Personen, die Treatment wählen.
**Statistik:**
Ein Chi-Quadrat-Test zeigt, dass die Unterschiede hoch signifikant sind (χ² = 294,84, p < 0,001).
Die Effektgröße nach Cramér’s V beträgt 0,544, was auf einen starken Zusammenhang hinweist.

## Explorative Analyse: Unternehmensgröße vs. Treatment
**Fragestellung:**
Untersuchung des Anteils an Personen, die sich für eine Behandlung entscheiden, abhängig von der Unternehmensgröße.
**Kategorien:**
    - Unternehmensgröße (no_employees): 1–5, 6–25, 26–100, 100–500, 500–1000, More than 1000
    - Treatment: Yes / No
**Beobachtungen:**
Die prozentuale Verteilung von Treatment Yes/No unterscheidet sich nur geringfügig zwischen den Unternehmensgrößen.
**Statistik:**
Ein Chi-Quadrat-Test zeigt, dass die Unterschiede nicht signifikant sind (χ² = 8,76, p = 0,119).
Die Effektgröße nach Cramér’s V beträgt 0,083, was auf praktisch keinen Zusammenhang hinweist.

## Fazit
Die Entscheidung für Treatment wird am stärksten durch Work Interfere und Family History beeinflusst. Gender hat einen kleinen bis moderaten Effekt, während Age, Remote Work und Unternehmensgröße praktisch keinen Einfluss zeigen. Arbeitsbelastung und familiäre Vorgeschichte sind demnach zentrale Faktoren für die Wahl von Treatment.

## GitHub-Link
- [Hier Link zum Notebook einfügen, falls hochgeladen]