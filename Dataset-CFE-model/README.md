Order of files to run:
1) `create_data.ipynb`
2) `loan_decision.ipynb`
3) `decision_boundary.ipynb`
4) `generate_cfs_new.ipynb`
5) `format_cfs.ipynb`
6) `filter_cfs.ipynb`

In order to change ranks/weights, edit the 10th cell in `format_cfs.ipynb` and run files 5 and 6. The flag `use_rank` must be set to False at the top of `format_cfs.ipynb` to set weights manually.

`filter_cfs.ipynb` will produce four files of counterfactuals, one for each hypothesis.

Take note of the variables `leaf_stop` and `num_orig_pts` in `generate_cfs_new.ipynb`. These will determine how many counterfactuals to generate and thus greatly affect runtime. `leaf_stop` must be defined again as the same value in `format_cfs.ipynb` and `filter_cfs.ipynb`.