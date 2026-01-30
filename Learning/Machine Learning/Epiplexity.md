
### Material
- [Paper Explanation on Youtube](https://www.youtube.com/watch?v=5xP7fZMaYmI)
- [Paper Overview on Zhihu](https://zhuanlan.zhihu.com/p/1997642487322396508)
- [Discussion on Zhihu: 「如何评价 CMU学者提出的认知复杂度（Epiplexity）理论？」](https://www.zhihu.com/question/1992694826018300486/answer/1992695606846707159)

### Basic
- A new term proposed from [From Entropy to Epiplexity Rethinking Information for Computationally Bounded Intelligence (2601.03220v1)](../../Literatures/Papers/From%20Entropy%20to%20Epiplexity%20Rethinking%20Information%20for%20Computationally%20Bounded%20Intelligence%20(2601.03220v1).md)
- **Meaning**: Learnable structured information


### Comparison with [Entropy](Entropy.md)
- Entropy measures uncertainty in information, a classical theory in information theory

### Three seemingly paradoxes in Information Theory
1. Information cannot be increased by deterministic processes.
	> **Example**: Inside $y=f(x)$, the information contained in cannot exceed the sum of that in $f$ and $x$
	> **Example**: The training of AlphaGo with [GAN](GAN.md) involves only computation without data, so where does the "intelligence" comes from?
2. Information is independent of factorization order.
	> **Example**: `I will go home tomorrow` is easy to learn for models, while `tomorrow go home will I` is not
3. Likelihood modeling is merely distribution matching
	> **Explanation**: Classical theory claims that models are just matching the underlying distribution of the data, so it should not be able to learn patterns that does not exhibit in the data, yet we observe [emergence](../Dynamical%20Systems/Emergence.md) in actual AI learning

### Key reason to such diversion
- Claimed by the author of the paper, it is the false assumption that the observer has unbounded computation (power and time)
- **Example**: The information abundance of $\pi$ is very small as it can be fully represented by a few lines of code given **unbounded computation**, and we can obtain infinite figures in infinite time, so in this circumstance, $\pi$ is very simple without any uncertainty. Yet if computation is bounded and the computer cannot generate later figures of $\pi$, it would seem "random" to AI.
- So under classical theory, given unbounded computation, we can just feed large amount of data to AI and it will learn the pattern. Yet in reality, the computation of AI is limited, so in order to predict the data, it must construct complicated model to obtain the result, leading to the occurrence of emergence, creating new information



Related Concepts
- Kolmogrov complexity