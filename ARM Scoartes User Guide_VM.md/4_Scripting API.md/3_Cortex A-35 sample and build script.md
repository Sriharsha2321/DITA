### 3.2.1 Cortex A-35 sample and build script

This sample script creates an instance of a Arm® Cortex®‑A35 core, with the specified parameters,
using the Configured Component API.

To open the sample script:

1. Open the **Creation** perspective.
2. In **Project Explorer**, expand your project and right-click on the **scripts** code.
3. Select **new script...**
4. In the dialog, select **Sample Cortex A35 Configure and Build**.


The **IP Catalog** *Configured Component* key is used to identify which component to create. Any unspecified parametrs take on their default value.

1. Enable the *ConfiguredComponent* API: require `ConfiguredComponent API`.
2. Define the *Configured Component* key from the IP catalog, and build parameters for the *Configured Component*. Modify the supplied code to match the following parameters: 
```A35 = "arm. com-CortexA_Cores-CortexA35-r0pl-00eaco A35_PARAMS = ["L2_CACHE = yes", "L2_CACHE_SIZE=512KB", "NUM_CPUS=4", "CRYPTO=No", "NEON_FP=No"]```