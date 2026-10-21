# In Silico Evaluation of Eugenol and Curcumin as Direct InhA Inhibitors

A comparative molecular docking and ADMET study of two dietary phenolics against *Mycobacterium tuberculosis* InhA, with isoniazid as reference.

## Summary

Isoniazid, a front-line TB drug, is a prodrug that must be activated by the enzyme KatG before it can inhibit InhA. Loss of KatG is the commonest cause of isoniazid resistance. This project asks whether two dietary phenolics — eugenol (clove) and curcumin (turmeric) — can bind the InhA substrate site directly, which would avoid that resistance route.

**Key finding:** By raw docking score, curcumin ranks best. But once the score is normalised per heavy atom (ligand efficiency), eugenol matches isoniazid while curcumin falls to less than half. Eugenol is the better-supported candidate for follow-up.

## Target

| Organism | *Mycobacterium tuberculosis* H37Rv |
| Protein | Enoyl-ACP reductase (InhA), EC 1.3.1.9 |
| Structure | PDB 2B35 (2.30 Å, triclosan-bound) |
| UniProt | P9WGR1 |

## Methods

- **Ligand prep:** SMILES from PubChem (isoniazid, eugenol, curcumin)
- **ADMET:** SwissADME (drug-likeness, absorption, structural alerts)
- **Docking:** AutoDock Vina 1.1.2 via Mcule 1-Click Docking
- **Analysis:** ligand efficiency = |binding affinity| / heavy atoms

## Results

| Ligand | Binding affinity (kcal/mol) | Heavy atoms | Ligand efficiency |
|---|---|---|---|
| Curcumin | −8.3 | 27 | 0.31 |
| Eugenol | −7.4 | 12 | 0.62 |
| Isoniazid | −6.4 | 10 | 0.64 |

All three pass Lipinski's rule of five and are predicted to have high GI absorption. Curcumin carries a PAINS alert and is known to be chemically unstable and poorly bioavailable.

## Conclusion

Eugenol is best described as a fragment-like hit worth growing, not a lead. All results are computational predictions and do not constitute evidence of antimycobacterial activity.

## Tools

SwissADME · PubChem · Mcule 1-Click Docking (AutoDock Vina) · RCSB PDB

## Author

Gayathri Bongannur — independent computational research project, October 2026.

## Note

This is a student self-study project for learning molecular docking and ADMET prediction. It is not experimental work and makes no therapeutic claims.
