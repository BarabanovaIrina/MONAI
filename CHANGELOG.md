# Changelog
All notable changes to MONAI are documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
## [0.2.0] - 2020-07-02
### Added
* Overview document for [feature highlights in v0.2.0](https://github.com/Project-MONAI/MONAI/blob/master/docs/source/highlights.md)
* Type hints and static type analysis support
* `MONAI/research` folder
* `monai.engine.workflow` APIs for supervised training
* `monai.inferers` APIs for validation and inference
* 7 new tutorials and examples
* 3 new loss functions
* 4 new event handlers
* 8 new layers, blocks, and networks
* 12 new transforms, including post-processing transforms
* `monai.apps.datasets` APIs, including `MedNISTDataset` and `DecathlonDataset`
* Persistent caching, `ZipDataset`, and `ArrayDataset` in `monai.data`
* Cross-platform CI tests supporting multiple Python versions
* Optional import mechanism
* Experimental features for third-party transforms integration
### Changed
> For more details please visit [the project wiki](https://github.com/Project-MONAI/MONAI/wiki/Notable-changes-between-0.1.0-and-0.2.0)
* Core modules now require numpy >= 1.17
* Categorized `monai.transforms` modules into crop and pad, intensity, IO, post-processing, spatial, and utility.
* Most transforms are now implemented with PyTorch native APIs
* Code style enforcement and automated formatting workflows now use autopep8 and black
* Base Docker image upgraded to `nvcr.io/nvidia/pytorch:20.03-py3` from `nvcr.io/nvidia/pytorch:19.10-py3`
* Enhanced local testing tools
* Documentation website domain changed to https://docs.monai.io
### Removed
* Support of Python < 3.6
* Automatic installation of optional dependencies including pytorch-ignite, nibabel, tensorboard, pillow, scipy, scikit-image
### Fixed
* Various issues in type and argument names consistency
* Various issues in docstring and documentation site
* Various issues in unit and integration tests
* Various issues in examples and notebooks

## [0.1.0] - 2020-04-17
### Added
* Public alpha source code release under the Apache 2.0 license ([highlights](https://github.com/Project-MONAI/MONAI/blob/0.1.0/docs/source/highlights.md))
* Various tutorials and examples
  - Medical image classification and segmentation workflows
  - Spacing/orientation-aware preprocessing with CPU/GPU and caching
  - Flexible workflows with PyTorch Ignite and Lightning
* Various GitHub Actions
  - CI/CD pipelines via self-hosted runners
  - Documentation publishing via readthedocs.org
  - PyPI package publishing
* Contributing guidelines
* A project logo and badges

[highlights]: https://github.com/Project-MONAI/MONAI/blob/master/docs/source/highlights.md

[Unreleased]: https://github.com/Project-MONAI/MONAI/compare/0.2.0...HEAD
[0.2.0]: https://github.com/Project-MONAI/MONAI/compare/0.1.0...0.2.0
[0.1.0]: https://github.com/Project-MONAI/MONAI/commits/0.1.0
