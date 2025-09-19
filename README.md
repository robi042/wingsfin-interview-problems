# wingsfin-interview-problems

# Problem 1: Bash Script Dockerfile Generator

**Category:** Back-end Challenge

## Problem Statement
Write a **Bash script** that creates a `Dockerfile` with the following specifications:

- Use a base image that installs **Python 3** using the `FROM` command.
- Install Python modules **`numpy`**, **`scipy`**, and **`pandas`** on a single line with `RUN pip install`.
- Set the default command to run **`./main.py`** using `CMD`.

The resulting `Dockerfile` should look like this:

```dockerfile
FROM python:3
RUN pip install numpy scipy pandas
CMD ["python", "./main.py"]
````

Requirements

The Bash script should print the SHA1 hash of the Dockerfile contents in the following format:

Example Output
2fd4e1c67a2d28fced849ee1bb76e7391b93eb12 Dockerfile

# Problem 2: Searching Challenge

**Category:** Back-end Challenge / Algorithm

## Problem Statement
Write a function `SearchingChallenge(strArr)` that reads a **4x4 matrix** of characters stored in `strArr`.  
The grid contains the following characters:

- **C** – Charlie the dog  
- **H** – Charlie’s home  
- **F** – Dog food  
- **O** – Empty space  

Your goal is to **figure out the least number of moves** required for Charlie to:

1. Grab each piece of food in the grid by moving **up, down, left, or right**, and  
2. Return home **after collecting all food**.  

> **Note:** Charlie **cannot move onto the home** before collecting all pieces of food.

### Additional Requirements
- The solution must contain the keyword `__define-ocg__` in at least one comment.
- At least one variable must be named `varOcg`.
- Use a variable named `varFiltersCg`.

### Example

#### Input
```java
new String[] {"OOOO", "OOFF", "OCHO", "OFOO"}
```

#### output
````java
01:akfpi0cxd
````


# Problem 3: WebSocket JSON Message Processor

**Category:** Back-end Challenge / JavaScript

## Problem Statement
Write a **JavaScript program** to simulate the processing of **WebSocket messages** that involve JSON data.

### Requirements
1. Define a function `handleJsonMessages` that takes an **array of message strings**.  
   Each message string is a JSON object representing a WebSocket message:

```json
{
  "type": "update" | "delete",
  "id": integer,
  "data": object (only for "update" type)
}
```


# Problem 4: Matrix Challenge (Boggle-style)

**Category:** Back-end Challenge / Algorithm / Java

## Problem Statement
Write a function `MatrixChallenge(strArr)` that reads an array of strings stored in `strArr`, which contains **2 elements**:

1. **First element:** A `4x4` matrix of letters, represented as a comma-separated string of rows.  
2. **Second element:** A long string of comma-separated words (each at least 3 letters), in alphabetical order, representing a dictionary.

### Objective
Determine if **all words** from the dictionary exist in the 4x4 matrix.  

- A word can be constructed from **sequentially adjacent spots** in the matrix (horizontal, vertical, or diagonal).  
- A word **cannot reuse the same location** more than once.  

> Similar to the rules in the game **Boggle**.

### Requirements
- Include the keyword `__define-ocg__` in at least one comment.
- Use a variable named `varOcg`.
- Use a variable named `varFiltersCg`.

### Example

#### Input 1
```java
new String[] {"aaey, rrum, tgmn, ball", "all,ball,mur,raeymnl,tall,true,trum"}
```


# Problem 5: Age Counting and File Hash

**Category:** Back-end Challenge / JavaScript / File Handling

## Problem Statement
Write a **JavaScript program** to perform a **GET request** on the route:  
```` http://coderbyte.com/api/challenges/json/age-counting
````


The API response contains a **data key** with a string of items in the format:  


### Objective
1. Count how many items have **age equal to 32**.  
2. Create a **write stream** to a file called `output.txt` containing the `key` values of the matching items, each on a separate line, in the order they appear in the JSON. Ensure the file ends with a **newline character**.  
3. Output the **SHA1 hash** of `output.txt`.  
4. Finally, combine the SHA1 hash with your **ChallengeToken** (`dxc0ipfka`) in **reverse order**, separated by a colon.

### Requirements
- Include the keyword `__define-ocg__` in at least one comment.
- Use a variable named `varOcg`.
- Use a variable named `varFiltersCg`.

### Example

#### Input (API Response)
```json
{
  "data": "key=IAfpK, age=32, key=WNVdi, age=64, key=jp9zt, age=40, key=9snd2, age=32"
}
```

