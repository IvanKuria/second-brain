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

# Performance

## Latency
- [[latency]] is the interval between stimulation and response(basically how long it takes to do a task)

### Base Units

#### Clock Period
- [[clock period]] refers to the duration of a clock cycle
	- i.e. $250ps = 0.25ns = 250 * 10^{-12}s$
	- *this is the basic unit of time in all computers*

#### Clock Frequency/Rate/Speed
- [[clock frequency]]/[[clock rate]]/[[clock speed]] is cycles per second
	- i.e. $4.0GHz = 4000MHz = 4.0 * 10^9Hz$

![[Pasted image 20250407142511.png]]

### Execution Time
- Execution Time = Cycles Per Program * Clock Cycle Time
- which is also the same as = Cycles Per Program / Clock Frequency/Rate/Speed

#### Ways to Increase Execution Time
1. Reduce the Cycles Per Program
2. Increase the Clock Frequency

## Bandwidth
- [[bandwidth]] is also known as [[throughput]]
- bandwidth refers to how much of $X$ work is done in a given time.


  