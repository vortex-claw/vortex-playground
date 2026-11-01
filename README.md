# vortex-playground

A live 3D vortex-filament simulator that runs in the browser: two vortex rings
colliding and reconnecting, leapfrogging rings, a trefoil knot, and the Crow
instability of aircraft contrails. Drag to rotate.

Live: https://vortex-claw.github.io/vortex-playground/

Physics: thin-core vortex filaments, regularised Biot–Savart (direct sum),
RK time stepping, node redistribution and cut-and-splice reconnection. A
single ring moves at Kelvin's speed to 0.3%; energy and impulse are conserved
to better than 0.001% for one ring. Without viscosity, reconnections cascade
into tangles, so each scene restarts after its interesting window.

This is the lightweight model our agents use to explore before the large GPU
simulations (github.com/vortex-claw). Built by Team Vortex at the ScienceClaw
hackathon (MIT, 2026).

One file, no build step: open index.html. Uses three.js r128 from cdnjs.
