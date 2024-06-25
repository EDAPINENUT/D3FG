# Functional-Group-Based Diffusion for Pocket-Specific Molecule Generation and Elaboration

This repo is for our NeurIPS 2023 paper `D3FG` for molecule generation.

[[arXiv]](https://arxiv.org/abs/2306.13769) &nbsp;


**Code**: Code is avaiable in[[CBGBench]](https://github.com/EDAPINENUT/CBGBench/tree/master). 

**Authors**: Haitao Lin, Yufei Huang, Odin Zhang, Lirong Wu, Siyuan Li, Zhiyuan Chen, Stan Z. Li.



## Abstract
In recent years, AI-assisted drug design methods have been proposed to generate molecules given the pockets' structures of target proteins. Most of them are atom-level-based methods, which consider atoms as basic components and generate atom positions and types. In this way, however, it is hard to generate realistic fragments with complicated structures. To solve this, we propose D3FG, a functional-group-based diffusion model for pocket-specific molecule generation and elaboration. D3FG decomposes molecules into two categories of components: functional groups defined as rigid bodies and linkers as mass points. And the two kinds of components can together form complicated fragments that enhance ligand-protein interactions.
To be specific, in the diffusion process, D3FG diffuses the data distribution of the positions, orientations, and types of the components into a prior distribution; In the generative process, the noise is gradually removed from the three variables by denoisers parameterized with designed equivariant graph neural networks. In the experiments, our method can generate molecules with more realistic 3D structures, competitive affinities toward the protein targets, and better drug properties. Besides, D3FG as a solution to a new task of molecule elaboration, could generate molecules with high affinities based on existing ligands and the hotspots of target proteins.
![teaser](https://raw.githubusercontent.com/EDAPINENUT/D3FG/main/d3fg_workflow.PNG)

## Code 
D3FG codes have been released to [[CBGBench]](https://github.com/EDAPINENUT/CBGBench/tree/master).


## Citation
If you find this work useful in your research, please consider citing:
```
@misc{lin2024functionalgroupbased,
      title={Functional-Group-Based Diffusion for Pocket-Specific Molecule Generation and Elaboration}, 
      author={Haitao Lin and Yufei Huang and Odin Zhang and Lirong Wu and Siyuan Li and Zhiyuan Chen and Stan Z. Li},
      year={2024},
      eprint={2306.13769},
      archivePrefix={arXiv},
      primaryClass={id='q-bio.BM' full_name='Biomolecules' is_active=True alt_name=None in_archive='q-bio' is_general=False description='DNA, RNA, proteins, lipids, etc.; molecular structures and folding kinetics; molecular interactions; single-molecule manipulation.'}
}
```
