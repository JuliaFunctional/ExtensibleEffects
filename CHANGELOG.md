# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2021-07-21
### Added
* WriterHandler has now a default accumulator, `Option()`.
* reexporting all DataTypes (from DataTypesBasic.jl and TypeClasses.jl)
* support for `Vector` is now generalized to `AbstractVector`
* added support for `AbstractDictionary` from the `Dictionaries` package 

### Changed
* `noeffect` when given an `Eff`, now passes it through unwrapped, just like `effect`.

### Removed
* `Eff` and `Continuation` are no longer exported, they are now considered internal details.

## [0.1.1] - 2021-03-30
### Added
* CI/CD pipeline
* Minimal Docs using Documenter
* Codecovering
* TagBot & CompatHelper
* License

### Changed
* parts from the README went to the docs

## [0.1.0] - 2020-06-14
initial release

### Added
* core implementation of extensible effects
* handlers for all DataTypes from DataTypesBasics, including ContextManager
* handlers for Task, Future, Vector, State, Writer