#🧪 Bayesian Inference of COVID-19 Vaccine Effectiveness (R/JAGS)

This project estimates vaccine effectiveness (VE) and its posterior uncertainty using a compact Bayesian binomial model implemented in JAGS (via rjags). The notebook also includes age-stratified analysis and simple visualizations.

##🧠 What I Did

Built a generative two-arm model (placebo vs. vaccinated)

Defined weakly informative Beta priors for baseline risk and protection

Implemented MCMC inference with rjags and summarized 95% credible intervals

Extended the workflow to age groups with replicated analyses

Produced quick plots and tidy summaries for VE and baseline infection probability

##🧰 Key Tools & Libraries

R (≥ 4.3)

JAGS (+ rjags)

coda, HDInterval, tibble

(optional) Jupyter with IRkernel for notebook execution

##📁 Files

AdvSProject.ipynb — Full R-kernel notebook: model spec, data blocks, MCMC sampling, age-stratified results, and plots

##📈 Sample Output

Posterior mean and 95% credible interval for VE (overall & by age)

Density/interval plots for eff = 1 − ffe and baseline risk pA
(Run the notebook to generate figures in-place.)

##⚙️ How to Run

Install JAGS on your system.

In R:

install.packages(c("rjags", "coda", "HDInterval", "tibble"))


Open AdvSProject.ipynb in Jupyter (R kernel) and run cells top-to-bottom.

##🔧 Customize

Swap in your own counts (nP, nV, nP.I, nV.I) to analyze different trials

Edit prior lines in the model block (e.g., dbeta(...)) to test sensitivity

Increase iterations / adjust burn-in for convergence; check coda diagnostics

##🌍 Why This Matters

Bayesian analysis provides transparent uncertainty and interpretable intervals for vaccine efficacy — useful for:

Rapid trial summaries and comparisons

Age-specific risk/benefit reporting

Sensitivity analyses to prior assumptions

##👩‍💻 Authors

[Roya Joulaei Vijouyeh](https://github.com/RoyaJV97)

Emerson Vero
