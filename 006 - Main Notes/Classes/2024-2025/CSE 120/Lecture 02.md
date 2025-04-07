Class: [[CSE 120]]
Subject: #computer-science #computer-architecture
Date: 2025-04-07
Teacher: **Prof. Nath

# Transistors

## Denard Scaling
- [[Denard Scaling]] is a way to scale transistor parameters(including voltage) to keep power density constant

*A question to ask is, if transistor size has kept decreasing (250nm in 1997 to 2nm in 2025), why has frequency started flatlining?*

## End of Denard Scaling
- a huge drawback to Denard Scaling is that it ignored the "leakage current" and "threshold voltage" which establish a baseline of power per transistor.
- as a result, it has created a "power wall" that has limited processor frequency to around 4GHz since 2006(yikes!)

![[Pasted image 20250407141306.png]]

### Potential Improvements
1. Using multiple cores
2. Parallelism
3. Speculative prediction