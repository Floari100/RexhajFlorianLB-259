# RexhajFlorianLB-259

# TMDB Movies Dataset Analysis Project

## 1) Dataset Description
Dieses Projekt verwendet das TMDB Movies Dataset, das auf Kaggle verfügbar ist. Der Datensatz enthält umfangreiche Informationen zu Filmen, darunter Felder wie Titel, Veröffentlichungsdatum, Budget, Einnahmen, Popularität, durchschnittliche Bewertungen und weitere. Diese Felder stehen in einem realen Zusammenhang – beispielsweise kann das Budget den erzielten Revenue beeinflussen oder die Popularität mit der durchschnittlichen Bewertung korrelieren. Die Vielzahl numerischer und kategorialer Felder ermöglicht es, verschiedene Vorhersagemodelle, Regressionen und Klassifikationen zu realisieren.

## 2) Data Privacy and Licensing
Das TMDB Movies Dataset wird unter einer offenen Lizenz (vergleichbar mit CC- oder MIT-Lizenz) auf Kaggle veröffentlicht und ist für Forschungs- und Bildungszwecke frei zugänglich. Es enthält ausschließlich öffentlich verfügbare Filminformationen und keine personenbezogenen Daten, wodurch Datenschutzbedenken weitgehend entfallen. Sowohl die Datenherausgeber als auch dieses Projekt halten sich an die geltenden Datenschutzrichtlinien, sodass eine unbedenkliche Nutzung gewährleistet ist.

## 3) Installation & Setup
Stellen Sie sicher, dass eine aktuelle Python-Version (3.8+) installiert ist. Die benötigten Pakete (z. B. pandas, matplotlib, scikit-learn) sollten vor der Nutzung vorhanden sein.


## Teilauftrag 2 – Datenbeschreibung (`Data_description.ipynb`)

1. **Zielvariable**  
   - Vorhersage von `revenue` (Einnahmen).
2. **Deskriptive Statistik**  
   - Berechnung von Mittelwert, Median und Standardabweichung aller numerischen Felder.
3. **Visualisierung**  
   - Histogramm des Budgets.
   - Streudiagramm Budget vs. Revenue.
4. **Feature-Engineering**  
   - Standardisierung des Feldes `budget` mit `StandardScaler`.
   - Erläuterung (50–100 Wörter) zur Notwendigkeit der Skalierung.


## Teilauftrag 3 – Modellierung (`Model.ipynb`)

1. **Datenaufteilung**  
   - `train_test_split` (80 % Training, 20 % Test).
2. **Modellwahl**  
   - `RandomForestRegressor` (100 Bäume, max_depth=10).
   - Robuste Abbildung nicht-linearer Zusammenhänge, unempfindlich gegen Ausreißer.
3. **Training & Evaluation**  
   - R²-Score und MAE auf dem Testset.
   - Gegenüberstellung tatsächlicher und vorhergesagter Revenues.
4. **Erkenntnisse** (ca. 80 Wörter)  
   - Budget, Popularität und Bewertung sind starke Prädiktoren. Bei Blockbustern treten größere Abweichungen auf. Hyperparameter-Tuning und zusätzliche Features (Genre-Dummies, Text-Merkmale) könnten die Vorhersage verbessern.