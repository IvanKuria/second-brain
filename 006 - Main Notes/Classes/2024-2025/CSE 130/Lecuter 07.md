Class: [[CSE 130]]
Subject: #computer-science #computer-systems 
Date: 2025-04-30
Teacher: Dr. **Veenstra**

# Modularity

## Soft Modularity

### Function Calls
- implement modularity by dividing code into named procedures
- *errors can propagate between modules!*
	- i.e
		- called function never returns(function crashes)
		- called function writes values to the wrong location
#### Soft Modularity invites error propagation
- this can be limited by using [[constrained languages]] 
##### Solution
- *enforced modularity*
- but can this be done in a high level language?

## Hard Modularity
- essentially use explicit messages for interactions between modules
	- *client*: initiates a request
	- *server*: responds to the request with a *response* or *reply*
### Advantages
- independent memory and interpreters
- less [[fate sharing]], more fault containment

### Communication
- makes use of a "wire" (real or virtual); models like a web browser/server
 

