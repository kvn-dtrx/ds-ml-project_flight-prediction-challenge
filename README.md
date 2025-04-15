# DS ML Project ⟡ Flight Delay Prediction Challenge

## Synopsis

This notebook represents our[^our] analysis of the ([flight delay dataset for Tunisair]https://zindi.africa/competitions/flight-delay-prediction-challenge) from [Zindi](https://zindi.africa). The general exercise reads as follows:

> **Value of Product**: Build a flight delay predictive model using Machine Learning techniques. The accurate prediction of flight delays will help all players in the air travel ecosystem to set up effective action plans to reduce the impact of the delays and avoid loss of time, capital and resources.

We try to predict the length of flight delay in $\mathrm{min}$. We evaluate our models with the root mean square error ($\mathrm{RMSE}$), in alignment with the requirements of the challenge.

As a baseline model, we choose a linear regression using weekday as predictor for flight delays, resulting in a $\mathrm{RMSE}$ of approximately $114$.

As the main ML model, we used CatBoost that is suited for situation where the majority of features is categorical, resulting in a $\mathrm{RMSE}$ of approximately $96$.

[^our]: At last: "our" refers to [MoSeBaur](https://github.com/MoSeBaur), [greseberisha](https://github.com/greseberisha), [kvn-dtrx](https://github.com/kvn-dtrx).

## Requirements

- Python 3.11.3
- pyenv
<!-- - Node.js -->

And additionally, as usual, the modules to be installed for the virtual environment are listed in requirements.txt.

## Setup

For macOS or Linux, execute:

``` shell
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

On Windows (with PowerShell), use:

``` shell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```
