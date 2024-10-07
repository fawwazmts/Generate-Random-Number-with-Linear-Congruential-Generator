# **Generate Random Number with Linear Congruential Generator**

## **Overview**

This project implements a Linear Congruential Generator (LCG) to produce a sequence of pseudo-random numbers. The implementation is contained in a Jupyter Notebook file named `rand_num_lcg.ipynb`.

## **Linear Congruential Generator (LCG)**

The LCG is a simple and commonly used method for generating a sequence of pseudo-random numbers. It uses the following recurrence relation:

$$
x_{n+1} = (a \cdot x_n + c) \mod m
$$

where:

- $x_n$ is the nth pseudo-random value in a sequence of pseudo-random values,
- $a$ is the multiplier,
- $c$ is the increment,
- $m$ is the modulus,
- $x_0$ is the initial seed value.

### **Key Functions**

1. **`lcg(a, c, m, x0)`**
   * This function is the core LCG implementation that yields pseudo-random numbers based on the provided parameters.
   * **Parameters:**
     * `a` (int): Multiplier
     * `c` (int): Increment
     * `m` (int): Modulus
     * `x0` (int): Seed (initial value)
   * **Yields:**
     * `int`: The next pseudo-random number in the sequence
2. **`my_rand(size, seed)`**
   * This function generates a list of pseudo-random numbers between 0 and 1 using the LCG.
   * **Parameters:**
     * `size` (int): The number of pseudo-random numbers to generate
     * `seed` (int): The initial value for the random number generator
   * **Returns:**
     * `List[float]`: A list of pseudo-random numbers normalized between 0 and 1

### **Example Usage**

To generate a list of pseudo-random numbers, the following example is provided in the notebook:

```python
# Generate and print a list of 5 pseudo-random numbers with a seed of 99999
random_numbers = my_rand(size=5, seed=99999)
print("Generated Pseudo-Random Numbers:", random_numbers)
```

## **Installation and Usage**

To run this project, you will need:

* Python 3.x installed on your machine
* Jupyter Notebook (can be installed via Anaconda or pip)

### **Steps to Run:**

1. Clone this repository:

   ```bash
   git clone https://github.com/fawwazmts/generate-random-number-lcg.git
   ```
2. Navigate to the project directory:

   ```bash
   cd generate-random-number-lcg
   ```
3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook rand_num_lcg.ipynb
   ```
4. Execute the cells in the notebook to generate pseudo-random numbers.

## **Related Article**
There is an article discussing this project in detail. You can read it [here](https://medium.com/@fawwazmts/generating-random-numbers-in-computer-cf4233ac46e8).

## **Contributions**

Feel free to fork this repository and submit pull requests for any improvements or enhancements!
