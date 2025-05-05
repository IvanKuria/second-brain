Class: [[CSE 120]]
Subject: #computer-science #computer-architecture 
Date: 2025-04-27
Teacher: **Prof. Nath

# RISC-V Cont

## Arrays in RISC-V

### Example 1

#### C code
``` c
a = b + pow[7];
```

**Assume 
	pow2 base address is in x3
	pow2's element size is 4B(1 word)**

#### RISC-V code
```
**

lw x4, 28(x3)   // x4 = Memory[pow2[7]]
add x2, x1, x4  // a = b + pow2[7]

**
```


### Example 2

#### C code
``` c
a[i] = b + c
```

**Assume: 
	i in x3,
	b in x1,
	c in x2, 
	a in x4, element size is 8B**

#### RISC-V code
```
**

add  x5, x1, x2   // x5 = b + c  

slli x6, x3, 3    // x6 = 8 * i

add  x6, x4, x6   // x6 = a + 8*i

sd   x5, 0(x6)    // Memory[a[i]] = b+c

**
```


## RISC-V Conditional Branch

### beq
- essentially branch if equal

```
**

beq reg1, reg2, label1

**
```

- consider the code:
#### SB Instruction Format
``` c
if (a == b) goto L1;
a = a + c;
L1: // continue
```

- here's how it would look like in RISC-V

#### RISC-V
```
**

// 8080: beq x1, x2, L1
// 8084: add x1, x3, x4

...

// 8092(L1) # Continue

**
```

### bne
- branch if *not* equal

```
**

bne reg1, reg2, label

**
```

#### SB Instruction Format
``` c
if (a != b) goto L1;
a = a + c;
L1: // continue
```

#### RISC-V code
```
**

bne s0, s1, L1
add s0, s0, s2

...

L1: // continue

**
```

