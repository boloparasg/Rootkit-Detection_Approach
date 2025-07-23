# SeqShield: Behavior-Based Rootkit Detection Using API Call Sequences 🔒

### Abstract

Rootkits are among the most elusive types of malware, capable of bypassing traditional static analysis methods due to their metamorphic behavior. Signature-based detection techniques struggle against these threats, necessitating a shift toward dynamic analysis approaches.

We propose **SeqShield**, a behavior-based rootkit detection approach designed specifically for the Windows OS, leveraging API call sequences for dynamic behavior analysis. Instead of relying on static signatures, SeqShield examines the execution patterns of API calls, which inherently reflect malicious intent.

Analyzing API sequences, we can effectively identify rootkit-like behavior. We also employed a metamorphic code engine to generate **10× mutated variants** of rootkits, demonstrating their obfuscation strategies. SeqShield applies **n-gram analysis** to extract **bigram and trigram** features from these API call sequences, enabling effective detection of rootkit-like activity.

Among the models tested, **Random Forest** achieves the highest accuracy of **97.27% (bigram)** and **96.17% (trigram)**. To optimize performance and decrease dimensionality, we apply **feature importance ranking** using the **Gini Impurity Index**, iteratively selecting the most significant features.

The optimized lower-dimensional feature matrix significantly enhances detection efficiency without sacrificing accuracy. Using the optimized feature set, our approach achieves **96.72% accuracy for bigrams** and **97.81% accuracy for trigrams**.

---

### Highlights

-  Behavior-based detection (no static signature reliance)
-  Metamorphic rootkit variant generation (10×)
-  Bigram & trigram n-gram analysis
-  Random Forest model with 97%+ accuracy
-  Feature optimization using Gini Impurity Index

---

### [Paper Link]

The Research paper is still under the process for the publication in Journals or in Conference. Once done the link will be updated.
