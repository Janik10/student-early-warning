# How early can you flag at-risk students, and who gets flagged?

An early-warning analysis on the Open University Learning Analytics Dataset (OULAD): about 32,000 students, 10.6M click records and every assessment result. Trained on 2013 courses, tested on 2014, scoring only students still enrolled each week.

**Key results**
- By **week 4**, activity and assessment signals reach AUC 0.76, and **9 in 10 of the top 10% flagged are truly at risk** (vs. ~44% by random pick). Demographics alone plateau around AUC 0.62.
- A demographics-heavy model flags students from the most deprived areas at **~11x** the rate of the least deprived, though their actual risk differs by ~1.4x. Behavior-based models narrow that gap and are more precise for both groups; dropping demographics costs little (precision 0.90 → 0.88).
- Students flagged at week 4 who later withdrew did so a median **53 days** later: about 7 weeks for advisor outreach.

**Caveats:** one UK distance-learning university; US campuses differ. Deprivation band is the only equity variable checked.

→ [Open the notebook](early_warning_oulad.ipynb)

Data: OULAD (Kuzilek, Hlosta & Zdrahal, 2017), CC BY 4.0 · By Jahangir Mammadli · [mammadli.dev](https://mammadli.dev)
