# Builder Pattern – Custom Computer Example

## Overview

This example demonstrates the **Builder Pattern** in a scenario where we need to assemble a **custom computer** with various components (CPU, GPU, RAM, storage, OS). Instead of calling a massive constructor with multiple parameters, we use a **builder** that allows step-by-step configuration of a `Computer` object, culminating in a final `build()` method that returns the fully constructed product.

### Why Builder?

- **Complex Object Setup**: Constructing a `Computer` requires many fields (CPU, GPU, RAM size, storage type, OS, etc.). A single constructor with all parameters could become cumbersome.
- **Readability**: A builder clarifies each configuration step (`setCpu()`, `setGpu()`, `setRamSize()`, etc.) rather than forcing you to memorize parameter ordering.
- **Flexibility**: You can easily introduce optional steps or new fields without breaking existing constructor calls.

## How to Run

1. **Compile the Java Files**  
   - Ensure your directory structure places `Computer`, `ComputerBuilder`, `GamingComputerBuilder`, and `BuilderDemo` together (or in a suitable package).
   - Use `javac` to compile:

   ```bash
   javac *.java
