


 ## 1.A factory produces widgets. Quality control tests show that 95% of the widgets from machine A are acceptable, while 90% of the widgets from machine B are acceptable. Machine A produces 60% of the widgets and machine B produces 40%. If a randomly selected widget is found to be acceptable, what is the probability that it was produced by machine A?

Given:
- P(A) = 0.60 (probability that the widget is from machine A)
- P(B) = 0.40 (probability that the widget is from machine B)
- P(acceptable | A) = 0.95 (probability that a widget from machine A is acceptable)
- P(acceptable | B) = 0.90 (probability that a widget from machine B is acceptable)

We need to find P(A | acceptable), the probability that the widget is from machine A given that it is acceptable.

By Bayes' Theorem:

\[
P(A | \text{acceptable}) = \frac{P(\text{acceptable} | A) \cdot P(A)}{P(\text{acceptable})}
\]

First, calculate P(acceptable), the total probability that a widget is acceptable:

\[
P(\text{acceptable}) = P(\text{acceptable} | A) \cdot P(A) + P(\text{acceptable} | B) \cdot P(B)
\]
\[
P(\text{acceptable}) = (0.95 \cdot 0.60) + (0.90 \cdot 0.40) = 0.57 + 0.36 = 0.93
\]

Now apply Bayes' Theorem:

\[
P(A | \text{acceptable}) = \frac{0.95 \cdot 0.60}{0.93} = \frac{0.57}{0.93} \approx 0.6129
\]

Thus, the probability that the widget was produced by machine A given that it is acceptable is approximately 0.6129, or 61.29%.



 ## 2. A jar contains 3 red balls and 7 blue balls. One ball is drawn at random. What is  the probability that the ball is red?





The total number of balls in the jar = 3 red + 7 blue = 10 balls

The probability of drawing a red ball = (Number of red balls) / (Total number of balls)

P(red) = 3 / 10





## 3. A standard deck of 52 cards contains 4 suits: hearts, diamonds, clubs, and spades. Each suit has 13 cards. What is the probability of drawing a heart given that a red card has been drawn?



The deck has 26 red cards (13 hearts and 13 diamonds). If a red card is drawn, the probability that it is a heart is:

The probability of drawing a heart given that a red card has been drawn can be calculated using conditional probability:

\[
P(\text{Heart}|\text{Red}) = \frac{P(\text{Heart and Red})}{P(\text{Red})}
\]

There are 26 red cards in a deck (13 hearts and 13 diamonds). The probability of drawing a red card is:

\[
P(\text{Red}) = \frac{26}{52} = \frac{1}{2}
\]

Out of the 26 red cards, 13 are hearts, so the probability of drawing a heart and a red card is:

\[
P(\text{Heart and Red}) = \frac{13}{52}
\]

Now, applying the formula:

\[
P(\text{Heart}|\text{Red}) = \frac{\frac{13}{52}}{\frac{26}{52}} = \frac{13}{26} = \frac{1}{2}
\]

Thus, the probability of drawing a heart given that a red card has been drawn is:

\[
\frac{1}{2}
\]




## 4. Two fair six-sided dice are rolled. What is the probability that the sum of the numbers on the dice is 8 given that the first die shows a 3?


The possible outcomes for two fair six-sided dice are 36, as each die has 6 sides. The problem asks for the probability that the sum is 8, given that the first die shows a 3.

If the first die is a 3, the second die must show a 5 for the sum to be 8 (since 3 + 5 = 8). There is only one favorable outcome: (3, 5).

Since the first die is already fixed at 3, we are only concerned with the outcomes of the second die. The second die can show any number from 1 to 6, so there are 6 possible outcomes.

Thus, the probability is:

\[
P(\text{sum is 8} \mid \text{first die is 3}) = \frac{1}{6}
\]


