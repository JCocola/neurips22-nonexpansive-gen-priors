# Signal Recovery with Non-Expansive Generative Network Priors  

This repository contains the accompanying code for the NeurIPS 2022 paper:  

**_Signal Recovery with Non-Expansive Generative Network Priors_**  
📄 *Advances in Neural Information Processing Systems 35 (NeurIPS 2022) - Main Conference Track*  
👥 *Author: Jorio Cocola*  

**⚠ Note:** This repository contains only the code used for experiments and *does not include the full paper*. The paper can be accessed here:  
🔗 [NeurIPS Proceedings](https://proceedings.neurips.cc/paper_files/paper/2022/hash/91d193b65d0b120d29503590827de1ea-Abstract-Conference.html)

## Summary  

We study compressive sensing with a deep generative network prior. Initial theoretical guarantees for efficient recovery from compressed linear measurements have been developed for signals in the range of a ReLU network with Gaussian weights and logarithmic expansivity: that is when each layer is larger than the previous one by a logarithmic factor. It was later shown that constant expansivity is sufficient for recovery. It has remained open whether the expansivity can be relaxed, allowing for networks with contractive layers (as often the case of real generators). In this work we answer this question, proving that a signal in the range of a Gaussian generative network can be recovered from few linear measurements provided that the width of the layers is proportional to the input layer size (up to log factors). This condition allows the generative network to have contractive layers. Our result is based on showing that Gaussian matrices satisfy a matrix concentration inequality which we term Range Restricted Weight Distribution Condition (R2WDC) and which weakens the Weight Distribution Condition (WDC) upon which previous theoretical guarantees were based. The WDC has also been used to analyze other signal recovery problems with generative network priors. By replacing the WDC with the R2WDC, we are able to extend previous results for signal recovery with expansive generative network priors to non-expansive ones. We discuss these extensions for phase retrieval, denoising, and spiked matrix recovery.

## Repository Structure  

- `Analysis.ipynb` – Analysis of results and validation of recovery properties  
- `Recovery_CS_python_experiment1.ipynb` – First set of experiments for compressive sensing recovery  
- `Recovery_CS_python_experiment2.ipynb` – Second set of experiments for compressive sensing recovery  
- `results/` – Folder for storing generated results from the experiments  

## Requirements  

The code is written in Python and relies on PyTorch. The following libraries are required:  

- Python 3  
- PyTorch  
- NumPy  
- Matplotlib  

## Running Experiments  

1. Open `Recovery_CS_python_experiment1.ipynb` or `Recovery_CS_python_experiment2.ipynb` in a Jupyter Notebook.  
2. Run the notebook cells to reproduce the experimental results.  
3. The results will be saved in the `results/` folder.  

## Citation  

If you find this work useful, please cite:  

```bibtex
@article{cocola2022signal,
  title={Signal recovery with non-expansive generative network priors},
  author={Cocola, Jorio},
  journal={Advances in Neural Information Processing Systems},
  volume={35},
  pages={23036--23048},
  year={2022}
}
```  
