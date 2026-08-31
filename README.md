# FTSE All Share Index – Volatility Modeling (GARCH & TARCH)

**Authors:** Daniel Zliechovec, Kryštof Přída  
**Course:** Applied Econometrics (SS 2026), Charles University (FSV UK)  
**Instructor:** Jiří Kukačka  

---

This repository contains our term paper analyzing the daily volatility dynamics of the **FTSE All Share Index** over the period 2010–2023 (3,326 observations).

### Summary & Main Findings:

* **Stylized facts:** Daily returns show heavy fat tails (kurtosis ~ 12.6), negative skewness, and clear volatility clustering. ARCH-LM tests confirmed strong conditional heteroskedasticity.
* **GARCH(1,1):** High volatility persistence with $\alpha + \beta \approx 0.97$, meaning market shocks take a long time to decay.
* **GJR-GARCH / TARCH:** Statistically significant asymmetry ($\gamma \approx 0.24$, $p < 0.001$), confirming a leverage effect where negative shocks drive future volatility much more than positive shocks of equal size.
* **Model diagnostics:** The asymmetric GJR-GARCH specification with Student-$t$ innovations outperforms symmetric GARCH on both AIC and BIC, leaving no remaining ARCH effects in the standardized residuals.

---

### File:
* `Term_Paper_Přída_Zliechovec.pdf` – full term paper with methodology, empirical results, and diagnostics.
