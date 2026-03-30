<p align="center">
  <img src="Figure1_Comparison.png" alt="L2 Norm Comparison" width="800">
  <br>
  <b>Figure 1: L2 Norm comparison across layers for Thinking vs. Non-Thinking responses.</b>.
</p>

<p align="center">
  <b>Table 1: Performance comparison with selection methods on Qwen3-4B across reasoning benchmarks.</b>
</p>

| Method | aime24 | aime25 | bbh | gpqa_main | gsm8k | gsm-plus | mmlu-pro |
|--------|--------|--------|-----|-----------|-------|----------|----------|
| Base | 60.00 | 56.66 | 84.78 | 48.88 | 95.41 | 79.90 | 67.92 |
| **LRS (Ours)** | **66.67** | **60.00** | 87.20 | **50.22** | 96.20 | **81.04** | **71.41** |
| DeepConf_filter | 56.67 | 53.33 | 88.56 | 47.67 | **96.45** | 79.90 | 65.20 |
| DeepConf_weighted | 63.33 | 60.00 | **89.81** | 48.36 | 95.82 | 80.08 | 61.12 |

<br>

<p align="center">
  <b>Table 2: Performance comparison with selection methods on LLaMA3-8B across reasoning benchmarks.</b>
</p>

| Method | aime24 | aime25 | bbh | gpqa_main | gsm8k | gsm-plus | mmlu-pro |
|--------|--------|--------|-----|-----------|-------|----------|----------|
| Base | 40.00 | 33.33 | 70.48 | 50.45 | 88.34 | 67.95 | 39.75 |
| **LRS (Ours)** | 43.33 | **36.67** | 74.14 | **54.68** | **90.82** | **70.57** | **42.31** |
| DeepConf_filter | 43.33 | 33.33 | 76.83 | 53.13 | 88.40 | 68.38 | 39.02 |
| DeepConf_weighted | 43.33 | **36.67** | **80.65** | 50.45 | 89.96 | 68.47 | 39.16 |

<p align="center">
  <b>Table 3: Performance comparison with steering methods on Qwen3-4B across reasoning benchmarks.</b>
</p>
|Method|aime24|aime25|bbh|gpqa_main|gsm8k|gsm-plus|mmlu-pro|
|---|---|---|---|---|---|---|---|
|Base|60.00|56.66|84.78|50.22|95.41|78.90|67.92|
|**TTTS(Ours)**|**66.67**|**60.82**|87.18|**51.33**|**96.68**|79.76|**71.15**|
|Entropy|56.67|53.33|86.87|48.06|96.38|79.48|68.55|
|LogProb|56.67|55.83|86.61|39.29|95.49|79.46|69.41|
|SAE|65.00|58.33|**87.51**|50.73|96.45|**80.15**|70.64|
<br>

<p align="center">
  <b>Table 4: Performance comparison with steering methods on LLaMA3-8B across reasoning benchmarks.</b>
</p>
|Method|aime24|aime25|bbh|gpqa_main|gsm8k|gsm-plus|mmlu-pro|
|---|---|---|---|---|---|---|---|
|Base|40.00|33.33|70.48|50.45|88.34|67.95|59.27|
|**TTTS(Ours)**|51.67|**40.00**|70.90|**55.13**|90.40|66.43|**60.67**|
|Entropy|40.00|36.67|70.77|53.75|88.47|66.33|58.84|
|LogProb|43.33|33.33|71.27|53.53|88.36|65.93|59.10|
|SAE|**53.33**|38.33|**70.94**|54.20|**90.87**|65.88|59.57|

<p align="center">
  <img src="Figure2_SAEs.png" alt="SAE Variants Comparison" width="800">
  <br>
  <b>Figure 2: Mean Top-K Feature Score across layers for different SAE configurations on Qwen3-4B.</b> We compare the Baseline SAE (hidden_mult=4, epochs=6, lr=1e-3, lambda_l1=1e-3) against variants: reduced capacity (hidden_mult=2), fewer epochs (3), higher sparsity penalty (lambda_l1=5e-3), relative difference ranking ((think-nonthink)/(nothink+ε)), and Top-40 feature dilution. Significant reasoning layers are highlighted in the green shaded region.
</p>

<p align="center">
  <img src="MI1.png" alt="MI and IG Analysis" width="800">
  <br>
  <b>Figure 3: Layer 34 analysis of Mutual Information (MI) and Information Gain (IG) over the final 128 tokens(Case 1).
</p>

<p align="center">
  <img src="MI2.png" alt="MI and IG Analysis" width="800">
  <br>
  <b>Figure 4: Layer 34 analysis of Mutual Information (MI) and Information Gain (IG) over the final 128 tokens(Case 2).
</p>

<p align="center">
  <img src="Case Study1.png" alt="Bad Case Study" width="800">
  <br>
  <b>Figure 5: Bad case study illustrating hallucination and false confidence.</b>.
</p>

<p align="center">
  <img src="Case Study2.png" alt="Bad Case Study" width="800">
  <br>
  <b>Figure 6: Bad case study illustrating overcaution.</b>.
</p>
