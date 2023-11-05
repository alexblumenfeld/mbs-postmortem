# code
Last updated: November 5, 2023

### Conda environment
Environment name is mbs_postmortem_20231105. Package list is saved in `mbs_postmortem_20231105.yml`.


### Notebook Descriptions and Order to Run In:
DATA EXTRACTION

- extract_bond_pmts: Extract the main principal and interest payments data
    - Output: bond_pmts.pkl
- extract_delinquency_stats: Extract the mortgage delinquency statistics in terms of counts (number of loans)
    - Output: delinquency_stats.pkl
- extract_delinquency_stats_balances: Extract the mortgage delinquency statistics in terms of balances (dollar value of loans)
    - Output: delinquency_stats_balances.pkl
- extract_mortgage_losses: Extract the principal writedown numbers, both for the whole deal and for fixed/ARM up through May 2013
    - Output: realized_losses.pkl and hist_payoff_loss_jan07_may13.pkl
- extract_remittances_to_trust: Extract the payments made to the MBS trust, along with payments from the swap deal
    - Output: remit_trust_with_swap.pkl
- extract_monthly_prepayments.pkl: Extract the volume of prepayments
    - Output: prepayments.pkl
- credit_ratings: Save the credit ratings data
    - Output: credit_ratings.pkl
- clean_hist_PL: Clean up the hist_payoff_loss_jan07_may13 dataset by adding fixed/ARM and Group I/Group II breakdowns
    - Input: hist_payoff_loss_jan07_may13.pkl
    - Output: hist_PL_with_totals.pkl

DATA ANALYSIS

### Figure Names
LIST OF FIGURES AND TABLES IN REPORT DRAFT 1.3 Oct 5.pdf
- P. 11: timeline_of_important_events
  - timeline.ipynb
- P. 12: stackplot_share_of_principal_group_i
  - EDA_april_6.ipynb
- P. 13: stackplot_share_of_principal_group_ii
  - EDA_april_6.ipynb
- P. 15: table_deal_summary
  - 
- P. 16: stackplot_delinq_status
  - delinq_ideas_june23.ipynb
- P. 17: stackplot_delinq_status_with_writeoffs
  - delinq_ideas_june23.ipynb
- P. 18: timeseries_prepayments
  - calcs_for_report.ipynb
- P. 21: timeseries_delinq_status_fixed_vs_arm
  - delinq_ideas_june23.ipynb
- P. 22: table_realized_losses_fixed_vs_arm
  - 
- P. 23: timeseries_cumulative_losses_fixed_vs_arm
  - calcs_for_report.ipynb
- P. 26: timeseries_losses_vs_writedowns
  - losses_vs_writedowns_aug_18.ipynb
- P. 27: timeseries_security_principal_pmts_composition
  - losses_vs_writedowns_aug_18,ipynb
- P. 29: timeseries_swap_performance
  - calcs_for_report.ipynb
- P. 34: table_maiden_lane_performance
  - 
- P. 34: timeseries_maiden_lane_ia3
  - credit_ratings.ipynb
- P. 35: timeseries_maiden_lane_ii1a3
  - credit_ratings.ipynb
- P. 45-46: table_subgroup_performance_broken_out
  - 
