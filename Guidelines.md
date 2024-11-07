# Guidelines

## Community Guidelines

This is a community provided Custom Device and we prescribe to the ideals and concepts outlined in the Python Software Foundation Code of Conduct. By contributing or using this repository you are also prescribing to behave accordingly as set out in the code of conduct within this respository.

https://policies.python.org/python.org/code-of-conduct/

## Contributor Guidelines

It is an expectation that anyone using the underlying LabVIEW code, modifying or repairing, has a working knowledge of LabVIEW built, VeriStand custom devices.

In order to contribute, first open an Issue, it will be reviewed and decided whether to be investigated and worked on.

**This repository is not intended to be officially supported by UKAEA, if you want an issue fixed, the best way to do so is to create the fix yourself and then submit the fix as a merge request.**

## Style Guidelines

This code is written such that it conforms with the normal expectations of a VeriStand custom device.

Whilst in the context of the System Explorer, i.e. pages, data around channels, groups and files are stored in the System Definition File XML format through the VeriStand Custom Device API.

However, in the Engine, transferrance to the engine and some helper "scripts" such as the import and export functionality, class definitions of File, Group and Channel are used to store and manage data.

This is partly because class usage is not supported for compiled settings transferred between the system explorer and engine.

To avoid file name collisions in libraries, classes have preprended their class name to the VI name.