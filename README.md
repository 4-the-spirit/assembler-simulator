# assembler-simulator

# 🎉 Introduction
This project was developed as the final assignment for the **C Programming Lab (20465)** course. Throughout its creation, I not only enhanced my C programming skills but also gained a deeper understanding of the significance of defining key components of software to address the original challenge effectively. Additionally, the project highlighted that a clear vision of all necessary functions and types is often not available from the outset; instead, the implementation evolves and adjusts based on ongoing requirements and discoveries.

# 🎯 Core Functionalities
+ **The `types.h` File:** The `types.h` file defines the most critical structures for the assembler-like program, including `Macro`, `Label`, `Operand`, `Command`, `Field`, `Operation`, and others. These structures are essential for creating the Macros Table, managing the Symbols Table, and encoding both commands and data definitions into machine code. The `Macro` structure supports the expansion of macros within the code, while the `Label` structure facilitates the definition and referencing of both data and command labels. The `Operand`, `Command`, `Field`, and `Operation` structures contain critical information about the commands, which will later be used to encode them into machine language.

+ **Macros Expansion:** The preprocessing of the assembly-like program involves expanding any macros called within the code. This step ensures that all macro definitions are fully expanded and integrated into the program before the actual assembly process begins.

+ **Symbols Table:** The first iteration of the assembler is primarily focused on creating the Symbols Table. This table holds essential information about the data and command labels used in the assembly-like program, including the label's instruction counter (IC), data counter (DC), and name. Each label's details are stored within an instance of the `Label` structure, ensuring that the assembler can accurately reference and process these labels throughout the second iteration in order to complete the encoding of the command and data definitions.

+ **Error Detection:** Before the final compilation of the program, which generates the object, external, and machine code files, the `detect(...)` function is executed to identify any errors in the program. The specifics of these errors are defined in the `errors.h` file, which outlines the various types of issues that the function will check for during this error detection phase.
