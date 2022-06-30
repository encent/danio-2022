## Whole genome insulation profiles

Insulation scores were obtained for good bins (determined by A.Galitsyna) only.

Insulation scores were calculated while calling TAD boundaries using HiChew utility. 

TAD boundaries were called independently for each of the corresponding 7 "stages" of *Danio rerio* embryogenesis. 

Insulation profiles were calculated for all stages within the TAD calling experiment (for the certain stage), given the certain window parameter for each chromosome.

Files:
* `insulation_window_bp_values.csv` -- insulation window parameter (in bp) for each TAD boundaries calling stage, for each chromosome;
* `csv/{stage}.csv` -- TAD boundaries calling experiments for each calling stage. Insulation profiles for each of the 7 stages are given for each `.csv` file;
* `bed/{stage}/{stage}.bed` -- BED-series of insulation score provided for each calling stage (directory), for each insulation profile (`.bed` file). These `.bed` files were prepared for the subsequent generation of `.bw` files (see below);
* `bw/{stage}/{stage}.bw` -- corresponding bigwig series of insulation score profiles.