Intra-operative endovascular treatment of intracranial aneur-ysms calls for rapid and reliable hemodynamic quantification. 
Angiographic Parametric Imaging (API) is derived from DSA time--density curves (TDCs), yet irregular frame rates and dose-reduction gaps often make conventional pixel-wise Gamma-variate fitting unstable and computationally expensive. 
We propose PIC-Former, a physics-inspired continuous transformer that reconstructs a physiologically plausible TDC function $\hat{c}(t)$ from irregular DSA samples. 
PIC-Former uses $\Delta t$-aware causal attention for inter-frame gaps and physics-inspired regularization to encourage valid contrast arrival, peak, and washout dynamics. 
On 52 paired DSA--4D Flow MRI cases and an independent 11-case CFD cohort, QDSA velocities computed from the reconstructed TDCs achieve relative MAEs of 3.1\% and 2.01\%, respectively, outperforming Gamma-variate fitting (11.8\% on DSA--4D Flow MRI). 
PIC-Former generates full-field parametric maps for a complete DSA run in 12.45\,s and remains stable under a 20\% frame-drop stress test. 
In a retrospective intra-operative risk stratification study, the proposed pipeline improves stratification accuracy from 87.5\% to 95.0\% compared to the Gamma-variate-based baseline. Code is available at \url{https://github.com/LY-SUSTech/PIC-Former.git}.
