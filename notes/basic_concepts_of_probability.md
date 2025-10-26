Here is a detailed summary of the fundamental concepts, approaches, and laws of probability theory based on your source materials:

### I. Fundamental Definitions

Probability theory provides the "language of communicating uncertainty in numbers". The basic building blocks include:

*   **Random Experiment:** An experiment where all possible outcomes are known in advance, but the specific outcome cannot be predicted with certainty before the experiment is performed.
*   **Sample Space ($\Omega$):** The set of all possible outcomes of a random experiment.
*   **Event:** Any subset of the sample space that is of interest. Events can be classified as:
    *   **Elementary Event:** A singleton subset of the sample space, such as $\{\omega_{i}\}$.
    *   **Compound Event:** An event formed by the union of two or more elementary events.
    *   **Impossible Event ($\phi$):** An event with no outcomes favoring its occurrence.
    *   **Sure Event ($\Omega$):** The sample space itself, as all outcomes favor its occurrence.

### II. Approaches to Probability Theory

Four main approaches are used to measure uncertainty:

1.  **Classical Approach:**
    *   The oldest approach, applied when outcomes are finite, mutually exclusive, and equally likely.
    *   The probability of event E ($\mathcal{P}(E)$) is the ratio of the number of favorable outcomes (m) to the total number of exhaustive cases (n): $\mathcal{P}(E) = \frac{m}{n}$.

2.  **Relative Frequency Approach (Statistical Approach):**
    *   Used when outcomes are not equally likely. It estimates probabilities from recorded data or a given frequency distribution.
    *   The **Statistical Approach** defines the probability as the limit to which the ratio of the frequency of event E (m) to the total number of trials (n) converges as $n$ approaches infinity ($\lim_{n\rightarrow\infty}\frac{m}{n}$).

3.  **Subjective Approach:**
    *   Applied when neither the Classical nor the Relative Frequency requirements are met.
    *   The probability is based entirely on the experience, intuition, expertise, and belief of an individual, interpreted as a measure of the degree of belief or quantified judgment.

4.  **Axiomatic Approach:**
    *   A general foundation coined by A. N. Kolmogorov (1933) to overcome the drawbacks of the Classical approach (which requires finite, equally likely outcomes).

### III. Axiomatic Foundations

A function $\mathcal{P}$ is a probability measure if it satisfies the following three axioms:

1.  **Axiom 1 (Non-negativity):** $0\le\mathcal{P}(E)\le1$.
2.  **Axiom 2 (Normalisation):** $\mathcal{P}(\Omega)=1$ (The probability of the entire sample space is 1).
3.  **Axiom 3 (Countable Additivity):** For a sequence of pairwise mutually disjoint events ($E_{i}$), the probability of their union is the sum of their individual probabilities: $\mathcal{P}(\bigcup_{i=1}^{\infty}E_{i})=\sum_{i=1}^{\infty}\mathcal{P}(E_{i})$.

### IV. Conditional Probability and Laws

These concepts allow for the calculation of complex and compound probabilities:

*   **Conditional Probability:** The probability of an event E occurring *given* that another event F has already occurred ($\mathcal{P}(E|F)$). It reduces the sample space to F. The definition is:
    $$\mathcal{P}(E|F)=\frac{\mathcal{P}(E\cap F)}{\mathcal{P}(F)},\mathcal{P}(F)\ne0$$.

*   **Addition Law of Probability:** Used to find the probability of the union of events ($\mathcal{P}(E_{1}\cup E_{2})$):
    *   **Mutually Disjoint Events:** $\mathcal{P}(E_{1}\cup E_{2})=\mathcal{P}(E_{1})+\mathcal{P}(E_{2})$.
    *   **General Case:** $\mathcal{P}(E_{1}\cup E_{2})=\mathcal{P}(E_{1})+\mathcal{P}(E_{2})-\mathcal{P}(E_{1}\cap E_{2})$.

*   **Multiplication Law of Probability:** Used to find the probability of the intersection of events ($\mathcal{P}(E\cap F)$). It is derived from the conditional probability definition:
    $$\mathcal{P}(E\cap F)=\mathcal{P}(F)\mathcal{P}(E|F)$$.

*   **Total Law of Probability:** Used to find the probability of an event A by summing its probability across a partition of the sample space defined by mutually exclusive and exhaustive events ($E_{i}$).
    $$\mathcal{P}(A)=\sum_{i=1}^{n}\mathcal{P}(E_{i})\mathcal{P}(A|E_{i})$$.

### V. Independence of Events

Two events E and F are considered independent if the occurrence or non-occurrence of one event provides no information about the occurrence or non-occurrence of the other.
*   The condition for independence is: $\mathcal{P}(E\cap F)=\mathcal{P}(E)\mathcal{P}(F)$.

### VI. Bayes' Theorem

Bayes' Theorem is also known as the inverse probability theorem because it allows us to reverse the conditioning of events (e.g., relating $\mathcal{P}(E|F)$ to $\mathcal{P}(F|E)$). It allows for the revision of **prior probabilities** ($\mathcal{P}(E_{i})$) into **posterior probabilities** ($\mathcal{P}(E_{i}|A)$) based on new information A.

The formula is:
$$\mathcal{P}(E_{i}|A)=\frac{\mathcal{P}(E_{i})\mathcal{P}(A|E_{i})}{\sum_{i=1}^{n}\mathcal{P}(E_{i})\mathcal{P}(A|E_{i})}$$.

***

This comprehensive overview covers the core concepts used throughout probability theory. 

Where would you like to apply these concepts next? 

Perhaps we could try a practice problem involving Bayes' Theorem, which ties together conditional probability and the Total Law?


