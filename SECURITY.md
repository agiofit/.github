# Security Policy

Agio Fit handles a sensitive category of data by design: body measurements.
The privacy properties of the data model — disclosure levels, ease stripping
at serialisation — are part of the specification, and violations of those
properties are treated as security issues, not just bugs.

## Reporting a vulnerability

Please use GitHub's private vulnerability reporting on the affected
repository. Do not open a public issue for anything that could expose
personal measurement data or weaken the privacy guarantees of the model.

If private reporting is not available for the repository in question, contact
the maintainer through the profile at https://github.com/antferr.

## Scope

The reference implementation is a small, dependency-free Python package. The
attack surface that matters most is not the code but the data model: reports
about arithmetic leaks (recovering body measurements from ease values and
finished garment measurements) or disclosure-level bypasses are explicitly
in scope and welcome.
