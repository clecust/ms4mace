# Multi-Scale Integration with MACE

## Introduction

This README provides guidance on seamlessly integrating multi-scale functionality with various e3nn framework equivariant models, 
as demonstrated in the MACE model example in this document.


## Integration Steps

Follow these steps to effortlessly incorporate multi-scale features into MACE:

Open the mace.modules block module file and add the MsInteractionBlock class and RealAgnosticResidualInteractionBlock_L class.

Open the mace.modules model module file and add ScaleShiftLBMACE.

Ensure to add the relevant names in the __init__ file as well.

If training the model is required, explicitly add the necessary modules in the scripts and mace.tools.arg_parser files.



To add multiscale related code to `mace.modules.block` and `mace.modules.model`, follow these steps:

1. Open the `mace.modules.block` module file, and add the class of `MsInteractionBlock` and `RealAgnosticResidualInteractionBlock_L`.
2. Open the `mace.modules.model` module file, and add the class of ``ScaleShiftLBMACE``.
3. Ensure to add the relevant names in the __init__ file as well. If training the model is required, explicitly add the necessary modules in the `scripts.run_train` and `mace.tools.arg_parser` files.

## Additional Notes
Make sure to carefully follow the steps mentioned above to successfully integrate multi-scale functionality into MACE. If you encounter any issues or have questions, refer to the documentation or reach out to the community for support.

Happy coding with multi-scale MACE!