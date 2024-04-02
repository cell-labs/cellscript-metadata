# Cell Script Metadata

The Cell Script Metadata is designed to give developers and tools the necessary information to interact with, compile, and debug the contract.

## Overview

The metadata is structured in JSON format, providing a standardized way to describe the properties of the `sUDT` contract. Below, you'll find a description of each field within the metadata.

### Top-Level Fields

- **name**: The name of the contract. In this case, it is "sUDT".
- **metadataVersion**: The version of the metadata format. This helps tools understand how to parse the metadata. The current version is "1.0".
- **language**: The programming language in which the contract is written. For this contract, it is "CellScript".
- **setting**: A collection of settings and versions for the compiler and virtual machine.
- **abi**: The Application Binary Interface (ABI) describes how to interact with the contract's functions.
- **elfcode**: A hexadecimal string representing the compiled contract code.

### Setting

The `setting` field contains configuration details about the environment and tools used to compile and run the contract.

- **compiler**: Information about the compiler used.
  - **version**: The version of the compiler. Here it is "CellScriptCompiler-1.0.0".
- **ckbVMVersion**: The version of the CKB Virtual Machine where the contract is intended to run. Specified as "v0.24.9" in this example.

### ABI

The `abi` array contains descriptions of the contract's functions exposed for interaction.

- **name**: The name of the function. The example includes a single function named "main".
- **parameters**: An array describing the parameters that the function accepts. In this case, the `main` function accepts no parameters.
- **returnType**: The type of value returned by the function. For the `main` function, it returns a "boolean".

### ELF Code

- **elfcode**: Contains the compiled contract code in hexadecimal format. This is the code that will be deployed to the blockchain. The example value "0x123" is a placeholder for the actual compiled code.
