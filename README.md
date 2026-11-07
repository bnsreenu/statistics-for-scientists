# Statistics for scientists

Python notebooks for the statistics tutorials on the [DigitalSreeni](https://www.youtube.com/@DigitalSreeni) YouTube channel.

These tutorials cover statistical concepts that come up in everyday research: how to report results honestly, how much to trust a number, and what a metric does and does not tell you. They are written for scientists, researchers, and data scientists who know basic Python but may not have a strong statistics background. The focus is on intuition and interpretation first, with the math and code explained along the way.

## Tutorials

All videos are collected in the YouTube playlist: [Statistics for scientists](PLAYLIST_LINK)

| # | Topic | Folder |
|---|---|---|
| 01 | When is 90% not 90%? Understanding confidence intervals for percentages (Clopper-Pearson) | [`01_clopper_pearson_confidence_interval`](01_clopper_pearson_confidence_interval) |

Each folder is self-contained, with its own notebook and README describing the requirements and any datasets.

### 01: When is 90% not 90%?

A player who makes 9 of 10 free throws and one who makes 900 of 1,000 both shoot 90%, but the evidence behind those numbers is very different. This notebook explains the Clopper-Pearson exact binomial confidence interval using basketball examples (including Stephen Curry's 13-of-17 game in 2016), then applies it to a malaria cell classifier trained on the NIH malaria cell images dataset.

Topics covered:

- Observed proportion versus true probability
- Why sample size matters
- What a 95% confidence interval means (repeated-sampling simulation)
- One-sided lower bounds versus two-sided intervals
- How Clopper-Pearson works: binomial tails, the beta distribution, and `scipy.stats.beta.ppf`
- Exact versus approximate intervals, and why exact intervals are conservative
- Reporting accuracy, sensitivity, and specificity with confidence bounds
- Limits of confidence intervals: patient-level dependence, dataset bias, and clinical reliability

## Getting started

```bash
git clone https://github.com/bnsreenu/statistics-for-scientists.git
cd statistics-for-scientists/01_clopper_pearson_confidence_interval
pip install numpy pandas scipy matplotlib scikit-learn pillow jupyterlab
jupyter lab
```

See the README inside each tutorial folder for details, including dataset download instructions.

## Requirements

Python 3.9 or newer. The notebooks use standard scientific Python packages (NumPy, Pandas, SciPy, Matplotlib, scikit-learn). No GPU is required.

## Data and citations

Datasets are not stored in this repository. Each notebook includes download instructions and citations for the data it uses. Please cite the original dataset authors if you use their data in your own work.

## More from DigitalSreeni

- YouTube: https://www.youtube.com/@DigitalSreeni
- Website: https://digitalsreeni.com
- GitHub: https://github.com/bnsreenu
