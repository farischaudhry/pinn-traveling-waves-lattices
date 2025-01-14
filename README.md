# pinn-traveling-waves-lattices

This project implements a TensorFlow-based physics-informed neural network (PINN) model, `FpuWaveNet`, designed to find traveling wave solutions to the FPUT nonlinear lattice system. The model utilizes a characteristic layer for a co-traveling frame, and specialized loss functions to optimize network performance.

The architecture is heavily inspired by the one presented in 'Traveling Wave Solutions of Partial Differential Equations via Neural Networks' (arXiv:2101.08520) by Cho et al.

## Requirements

The code was tested using:

- tensorflow==2.11.0
- numpy==1.26.4
- scipy==1.11.2
- matplotlib==3.9.1
- pillow==10.0.0

You can install the necessary dependencies using:

```bash
pip install requirements.txt
```

## Usage
- Ensure all dependencies are installed.
- Run the script to train the `FpuWaveNet` model.
- Monitor the loss and speed history for training progress.
- Download and run the functions to animate the model's findings.
- We recommend storing the model weights via model.save_weights(path_to_file) and model.load_weights(path_to_file) for reproducibility. 

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
