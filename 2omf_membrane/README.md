# 2omf_membrane test inputs

Provenance for `system.psf` and `equil.dcd`.

## System

- PDB 2OMF OmpF porin **monomer**, *E. coli*, 2.4 A, 340 residues
- Built with CubeBuilder 1.8.8
- 190 POPC + 49 CHL bilayer, 14,572 TIP4P waters, 52 Na+ / 40 Cl-
- Box 91.983 x 91.983 x 106.798 A (90/90/90, P1)

## Equilibration

- step2.1-derived NAMD-style `.inp`, `nstep=25000`, `nstdcd=5000`
  -> 25 ps, 5 frames every 5 ps (dt = 0.001 ps / 1 fs)
- OpenMM 8.5.2.dev, CPU

## Files

- `system.psf` — PSF EXT, segment ID in field 2, `!NATOM=92,537`
- `equil.dcd` — 5 frames

## Notes

- 4-letter capping residues NALA (res 1) / CPHE (res 340) appear in PDB
  cols 18-21 for the PROT_A selection
- Canonical selection: `--sel "segid PROT_A"`