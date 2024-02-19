# Multi-Scale Integration with MACE

## Introduction

This README provides guidance on seamlessly integrating multi-scale functionality with various e3nn framework equivariant models, as demonstrated in the MACE model example in this document.

## Integration Steps




To add multiscale related code to `mace.modules.block` and `mace.modules.model`, follow these steps:

1. Open the `mace.modules.block` module file, and add the class of `MsInteractionBlock` and `RealAgnosticResidualInteractionBlock_L`.
2. Open the `mace.modules.model` module file, and add the class of ``ScaleShiftLBMACE``.
3. Ensure to add the relevant names in the __init__ file as well. If training the model is required, explicitly add the necessary modules in the `scripts.run_train` and `mace.tools.arg_parser` files.

## Additional Notes
For more detailed information about MACE, including its architecture, features, and usage, please refer to the comprehensive documentation provided in the README4MACE.md file. This document covers a broader spectrum of MACE-related topics and serves as a valuable resource for understanding and leveraging the full potential of the MACE model.

Make sure to carefully follow the steps mentioned above to successfully integrate multi-scale functionality into MACE. If you encounter any issues or have questions, refer to the documentation or reach out to the community for support.

Happy coding with multi-scale MACE!


## References

If you use this code, please cite our papers:
```text
@misc{hu2023efficient,
      title={Efficient Machine Learning Force Field for Large-Scale Molecular Simulations of Organic Systems}, 
      author={Junbao Hu and Liyang Zhou and Jian Jiang},
      year={2023},
      eprint={2312.09490},
      archivePrefix={arXiv},
      primaryClass={cond-mat.soft}
}
```