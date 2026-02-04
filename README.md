# -Implementation-of-Merge-Sort-in-ARM-Cortex-M0+

Implementation of the **Merge Sort** algorithm in **ARM Cortex-M0+ Assembly**. This project follows the **Thumb-1** instruction set constraints and utilizes a recursive divide-and-conquer approach. 

---

## Project Structure

* **Part 1 (`part1.s`)**: 
    * Sorts exactly **five elements**.
    * Elements are initially placed in registers **R0–R4**.
    * The final sorted array is returned in registers **R0–R4**.
* **Part 2 (`part2.s`)**:
    * Sorts an **8-element array** stored in memory.
    * The array base address is loaded into **R7**.
    * The final sorted result is stored across registers **R0–R7**.

## Implementation Details

* **Recursive Strategy**: Uses `my_MergeSort` for the divide phase and `my_Merge` for the conquer phase.
* **Stack Management**: Implements proper **PUSH/POP** operations for context preservation and **LR** handling.
* **Memory Handling**: Allocates **temporary buffers** on the stack for merge operations.
* **Naming Conventions**: Follows the required structure: `main`, `my_MergeSort`, and `my_Merge`.
