Master's student in Atmosphere/Energy at Stanford, in the department of Civil
and Environmental Engineering. Before that, Ecole Polytechnique.

I work on optimisation and power systems, and on the scientific computing that
sits underneath them: numerical methods applied to real data, where a
formulation that is sound on paper can still fail quietly on one input or on
one machine.

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

Reach me at valmann@stanford.edu, or on
[LinkedIn](https://www.linkedin.com/in/valentin-mann).
