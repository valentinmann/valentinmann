Master's student in Atmosphere/Energy at Stanford, in the department of Civil
and Environmental Engineering. Before that, Ecole Polytechnique.

I work on optimisation, power systems and energy storage, and on the scientific
computing and machine learning that sit underneath them: methods applied to real
data, where a formulation that is sound on paper can still fail quietly on one
input or on one machine.

### single-diode

[single-diode](https://github.com/valentinmann/single-diode) fits the five
parameters of a photovoltaic module's equivalent circuit from its published
datasheet, then solves the circuit. The difficulty is numerical rather than
conceptual: the textbook closed form overflows double precision on real
modules, and whether the parameter fit converges depends on where it starts.

### campaign

[campaign](https://github.com/valentinmann/campaign) runs a parameter sweep
described in one YAML file, locally or as SLURM job arrays, and checks every
run against invariants the physics says cannot fail. What it guards against is
output that looks fine: a run killed mid-write that still counts as finished,
or a result reused after its model file has changed.

### cyclelife

[cyclelife](https://github.com/valentinmann/cyclelife) predicts how long a
lithium-ion cell will last from its first 100 cycles, on the public MIT-Stanford
dataset, splits strictly by cell, and replicates the paper's linear model to
within five cycles. The first run was off by a factor of three on one test set:
two physically impossible capacity readings, found by comparing each set with
the paper separately.

Reach me at valmann@stanford.edu, or on
[LinkedIn](https://www.linkedin.com/in/valentin-mann).
