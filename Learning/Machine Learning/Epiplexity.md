
> **Warning**: This topic is not widely accepted in the academic community

### Material
- [Paper Explanation on Youtube](https://www.youtube.com/watch?v=5xP7fZMaYmI)
- [Paper Overview on Zhihu](https://zhuanlan.zhihu.com/p/1997642487322396508)
- [Discussion on Zhihu: 「如何评价 CMU学者提出的认知复杂度（Epiplexity）理论？」](https://www.zhihu.com/question/1992694826018300486/answer/1992695606846707159)

### Basic
- A new term proposed from [From Entropy to Epiplexity Rethinking Information for Computationally Bounded Intelligence (2601.03220v1)](../../Literatures/Papers/From%20Entropy%20to%20Epiplexity%20Rethinking%20Information%20for%20Computationally%20Bounded%20Intelligence%20(2601.03220v1).md)
- **Meaning**: Learnable structured information under bounded computation
	- **"Learning"**: compressible and understandable
- Not a generally accepted concept, still debating

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

### New framework
- $\text{Total information} = \text{Epiplexity} + \text{Time Bounded Entropy}$
	- $\text{Time Bounded Entropy}$: Relative random noise to the model, might have underlying meaning, but unpredictable anyway under the bounded computation, so can only be treated as random noise. This is toxic and useless to AI models, would waste a lot of computation without actually learning anything
- Two metrics to measure Epiplexity in data
	1. Prequential Coding (预序估计)
	2. Requential Coding (序列编码)
- Then before training AI, we can first evaluate the data, keeping only those with high Epiplexity and removing those with high Entropy

### Implication
- Synthetic data might be a good way instead of a 权宜之计 to train models
- We might need a lot less data to train a equally strong model, saving computation and thus energy

### Criticism
- Is this method limited to specific neural network (transformer)? Does it still work in other neural network structure?
- Would the measurement of Epiplexity itself consume a lot of energy, cancelling out the benefit?
- Would synthetic data affect the training performance?
- Epiplexity is not a new concept, it already exists in the field of Complex Systems


### Related Concepts
- Kolmogrov complexity