# DS/ML Project: Flight Delay Prediction Challenge

## Synopsis

This notebook represents our analysis of the [flight delay dataset for Tunisair](https://zindi.africa/competitions/flight-delay-prediction-challenge) from [Zindi](https://zindi.africa). The general exercise reads as follows:

> **Value of Product**: Build a flight delay predictive model using Machine Learning techniques. The accurate prediction of flight delays will help all players in the air travel ecosystem to set up effective action plans to reduce the impact of the delays and avoid loss of time, capital and resources.

We try to predict the length of flight delay in $\mathrm{min}$. We evaluate our models with the root mean square error ($\mathrm{RMSE}$), in alignment with the requirements of the challenge.

As a baseline model, we choose a linear regression using weekday as predictor for flight delays, resulting in a $\mathrm{RMSE}$ of approximately $114$.

As the main ML model, we used CatBoost that is suited for situation where the majority of features is categorical, resulting in a $\mathrm{RMSE}$ of approximately $96$.

## Installation

### Requirements

- Python 3.11.3
- pyenv

### Setup

1. Navigate to a working directory of your choice, then clone the repository and enter it:

   ``` shell
   git clone https://github.com/julialoeschel/capstone-SignalSigma.git &&
       cd capstone-SignalSigma
   ```

2. Choose a setup option based on your operating system and intended use:

   - `make basic-unix` / `make basic-win`: for general use or exploration (core dependencies only).
   - `make dev-unix` / `make dev-win`: for contributors (includes development tools like linters and pre-commit hooks).

   If you prefer to run the commands manually yourself or want to inspect what each `make` target does first, use the `-n` flag for a dry run. This prints the commands without executing them:

   ``` shell
   make -n <target>
   ```

3. Activate the virtual environment:

   - On macOS/Linux, run:

     ```shell
     source .venv/bin/activate
     ```

   - On Windows (PowerShell), run:

     ``` powershell
     .\.venv\Scripts\Activate.ps1
     ```

---

## Note was created from

<https://github.com/kvn-dtrx/ds-ml-project-template>

---

## Colophon

**Authors:**

- [MoSeBaur](https://github.com/MoSeBaur)
- [greseberisha](https://github.com/greseberisha)
- [kvn-dtrx](https://github.com/kvn-dtrx)

**Acknowledgements:**

I would like to thank my ghostwriter [Gregory Peter Thompson](https://chatgpt.com).

**Template:**
This repository was created from the [Template Name](https://github.com/neuefische/ds-ml-project-template) template.

**License:**
[MIT License](licence.txt)
