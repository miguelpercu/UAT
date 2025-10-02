Unified Applicable Time (UAT) Framework
📖 Overview
The Unified Applicable Time (UAT) Framework is a novel cosmological framework that integrates quantum gravitational corrections with standard $\Lambda$CDM cosmology. This framework provides a conservative extension to established cosmological models while maintaining full compatibility with observational data.

🎯 Key Features
Quantum-Cosmological Integration: Combines Loop Quantum Gravity (LQG) corrections with standard cosmology

Observational Validation: Statistically equivalent to $\Lambda$CDM against H(z) data ($\chi^2 = 14.8$)

Mass-Dependent Corrections: Controlled modifications based on Primordial Black Hole (PBH) mass parameters

Conservative Extension: Maintains backward compatibility with $\Lambda$CDM at reference mass $M_0 = 10^{12}$ kg

📊 Statistical Results
Metric	$\Lambda$CDM	UAT Framework
$\chi^2$	14.8	14.8
$\chi^2_{\text{red}}$	0.528	0.528
$\Delta\chi^2$	--	0.0
🔬 Scientific Foundations
Core UAT Equation
text

Copy

Download
t_UAT = t_event × 1/a(t) × √[max(1 - 2GM/c²r, (l_Planck/r)²) × 1/(1 + γl_Planck²/4πr_s²)] + d_L/c
Hubble Parameter Formulation
text

Copy

Download
H_UAT(z, M) = H_0 × E_ΛCDM(z) × [1 + γ·ln(M/M_0)·ln(1+z)]
Parameters:

$\gamma = 0.2375$ (Barbero-Immirzi parameter, LQG)

$M_0 = 10^{12}$ kg (reference PBH mass)

Physical bounds: $-0.2 \leq f(z, M) \leq +0.2$

📁 Repository Structure
text

Copy

Download
UAT-Framework/
├── 📄 main.tex                          # LaTeX manuscript
├── 📄 references.bib                    # Bibliography
├── 📊 uat_vs_lcdm_comparison.png        # Main comparison figure
├── 📊 uat_comprehensive_analysis.png    # Comprehensive analysis
├── 📊 uat_sensitivity_analysis.png      # PBH mass sensitivity
├── 📋 dataset_summary.txt               # Data summary
└── 📖 README.md                         # This file
🚀 Quick Start
For Researchers
Review the manuscript: main.tex contains complete theoretical framework

Examine results: Statistical validation against 30 H(z) measurements

Analyze sensitivity: PBH mass corrections from $-1.39%$ to $+2.08%$

For Developers
python

Copy

Download
# Basic UAT Hubble parameter implementation
def H_UAT(z, M, H0=67.4, Omega_m=0.315, gamma=0.2375, M0=1e12):
    E_LCDM = np.sqrt(Omega_m * (1+z)**3 + (1-Omega_m))
    correction = gamma * np.log(M/M0) * np.log(1+z)
    correction = np.clip(correction, -0.2, 0.2)  # Physical bounds
    return H0 * E_LCDM * (1 + correction)
📈 Key Findings
Statistical Equivalence
Identical $\chi^2$ values with $\Lambda$CDM cosmology

30 H(z) data points across $z = 0.07$ to $z = 1.75$

Reduced $\chi^2 = 0.528$ indicating excellent fit

Physical Insights
Conservative corrections: Maximum $\pm 2.2%$ variation

Mass-dependent scaling: Logarithmic dependence on PBH mass

Redshift evolution: Controlled growth with cosmic time

🔗 Related Repositories
Main UAT Framework: Complete implementation and analysis

UAT Explanation: Detailed documentation and examples

📚 Citation
If you use this framework in your research, please cite:

bibtex

Copy

Download
@article{percudani2025uat,
    author = {Percudani, Miguel Angel},
    title = {Advanced Unified Applicable Time Framework: Cosmological Validation and New Insights into $\Lambda$CDM Extensions},
    year = {2025},
    url = {https://github.com/miguelpercu/A-Unified-Applicable-Time-Framework-for-Modeling-Primordial-Black-Holes}
}
🎓 Applications
Current Capabilities
Cosmological parameter estimation

PBH evolution modeling

Quantum gravity phenomenology

Cosmological tensions investigation

Future Extensions
CMB and BAO data integration

Bayesian parameter inference

Inflationary scenario applications

Multi-messenger astronomy connections

🤝 Contributing
We welcome contributions in:

Theoretical extensions

Numerical implementations

Observational validations

Documentation improvements

📄 License
This project is open source and available under the MIT License.

📞 Contact
Miguel Angel Percudani
Independent Researcher
Puan, Buenos Aires, Argentina
Email: miguel_percudani@yahoo.com.ar
GitHub: @miguelpercu

⭐ If you find this framework useful, please star the repository!

Last updated: September 2025