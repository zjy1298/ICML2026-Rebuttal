<p align="center">
  <img src="Figure1_Comparison.png" alt="L2 Norm Comparison" width="800">
  <br>
  <b>Figure 1: L2 Norm comparison across layers for Thinking vs. Non-Thinking responses.</b>.
</p>

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
