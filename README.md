**Sequential Testing in Python: Beyond Traditional A/B Testing**

This repository demonstrates a Python-based simulation and visualization of various sequential testing algorithms that help solve the limitations of traditional A/B testing, 
such as long run times and inflated false positives from repeated peeking.

We compare the performance and stopping behavior of the following methods:

**✅ Implemented Methods**
	•	Traditional A/B Test (fixed horizon)
	•	Bonferroni Correction (Naive Sequential Testing)
	•	Group Sequential Designs (GSD)
	•	Pocock Boundary
	•	O’Brien-Fleming Boundary
	•	Alpha Spending Function (Linear)
	•	SPRT (Sequential Probability Ratio Test)
	•	mSPRT (Mixture Sequential Probability Ratio Test)

**🔍 Use Case**

We simulate an A/B experiment with:
	•	Baseline conversion rate = 0.5%
	•	Test group with a 6% relative lift
	•	1.2M samples per variant
	•	Analysis checkpoints every 100,000 users

**The goal** is to evaluate how different sequential testing frameworks perform in terms of:
Early stopping, Type I error control, Sensitivity to noise, Operational practicality

📈 Visualizations

Each method is plotted in a separate subplot showing:
	•	P-value (or likelihood ratio) evolution
	•	Statistically adjusted decision boundaries
	•	Highlighted stopping point (if detected)
