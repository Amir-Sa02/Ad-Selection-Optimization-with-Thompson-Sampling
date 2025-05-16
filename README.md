# Thompson Sampling – Ad Selection Optimization

This project demonstrates how **Thompson Sampling**, a probabilistic approach to solving the Multi-Armed Bandit problem, can be used to optimize ad selection based on user interactions (click-through rates).

---

## Project Overview

The goal of this project is to select the most effective online advertisement from a set of 10 different ads using **Reinforcement Learning**.
The algorithm uses Thompson Sampling to balance exploration and exploitation over 10,000 rounds and identify the ad with the highest performance.

---

## Algorithm: Thompson Sampling

Thompson Sampling is a Bayesian method for solving the multi-armed bandit problem. At each round, the algorithm:

1. Draws a random sample from the Beta distribution for each ad.
2. Selects the ad with the highest sample.
3. Observes the reward (whether the ad was clicked or not).
4. Updates the parameters of the Beta distribution for that ad.

---

## Dataset

* **File**: You can download the dataset from this link: https://www.kaggle.com/datasets/akram24/ads-ctr-optimisation
* **Format**: Each row represents a round of ad display, and each column represents a different ad.
* **Values**: `1` (clicked) or `0` (not clicked) for each ad.

---

## How to Run

1. Clone the repository:

   ```bash
   $ git clone https://github.com/Amir-Sa02/Ad-Selection-Optimization-with-Thompson-Sampling
   $ cd thompson-sampling-ad-selection
   ```

2. Upload your dataset `Ads_CTR_Optimisation.csv` to your Google Drive or working directory.

3. Run the script in Google Colab or Jupyter Notebook.

4. A histogram will be generated showing the number of times each ad was selected.

---

## Results

The final histogram displays how frequently each ad was selected by the algorithm over 10,000 rounds.
Thompson Sampling progressively focuses on the most successful ads based on observed click-through rates.

---

## Outcome

* Improved ad selection through reinforcement learning
* Balanced exploration of all ads with exploitation of high-performing ones
* Demonstrated a practical use case for Bayesian inference

---

## Reference

This project is based on the Thompson Sampling implementation in the [SuperDataScience Machine Learning A–Z™ course](https://www.udemy.com/course/machinelearning/).

---

Let me know if you'd like help converting this to a `README.md` file or adjusting it further.
