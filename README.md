# Off-by-One Error in COBOL PERFORM Loop

This repository demonstrates a common off-by-one error in COBOL PERFORM loops and its solution.

## Bug
The `bug.cob` file contains a COBOL program with a PERFORM loop that suffers from an off-by-one error. The loop intends to iterate 10 times but due to the loop condition, it iterates 11 times.  This leads to an incorrect value being assigned to `WS-COUNTER`.

## Solution
The `bugSolution.cob` file presents a corrected version of the loop, ensuring the loop iterates exactly 10 times.

## How to Run
You will need a COBOL compiler to run these programs.  The exact steps depend on your chosen compiler but generally involve compiling and linking the code.

For example using GnuCOBOL:
```bash
gnucobol -x bug.cob
gnucobol -x bugSolution.cob
```