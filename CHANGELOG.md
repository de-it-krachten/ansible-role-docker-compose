# [1.11.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.10.1...v1.11.0) (2024-12-29)


### Features

* Update supported platforms & CI ([5b52591](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/5b525917a87a61e5ed97a5d87239207e48a34a10))

## [1.10.1](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.10.0...v1.10.1) (2024-09-26)


### Bug Fixes

* Change docker_compose -> docker_compose_v2 due to decrecation ([68de567](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/68de5675bb3e36e3cedeabe2b4b8da7abf3cf222))
* pin requests<2.32 due to issues ([da6fc0d](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/da6fc0d0608a1ff93afbdabd2cd3a76c4e8034c9))

# [1.10.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.9.2...v1.10.0) (2024-06-01)


### Features

* Add support for Ubuntu 24.04 LTS + Fedora 40 ([fa4bd00](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/fa4bd009753708a0ec74f8d99bbc19707418f245))

## [1.9.2](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.9.1...v1.9.2) (2024-04-12)


### Bug Fixes

* Defaults to pip version only in virtual environment ([91dfe2c](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/91dfe2caee23fa18b327ca708b49d251efd0ef47))
* pin venv to docker<7 ([cef5b28](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/cef5b28e67a52821649ce0fad3e9d75d48798539))

## [1.9.1](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.9.0...v1.9.1) (2023-11-08)


### Bug Fixes

* Make it possible to choose python version for venv ([4899aa5](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/4899aa5a60817f64a277004e03c67e53f53c318c))

# [1.9.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.8.1...v1.9.0) (2023-11-03)


### Features

* Add support for docker-compose in python virtual environment ([edaaed7](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/edaaed7471f47e1d038c5c82dd2ac59655ab6302))

## [1.8.1](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.8.0...v1.8.1) (2023-10-25)


### Bug Fixes

* Execute template code as root (optionally) ([73e63ee](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/73e63ee807ff1b57c1b734b0aa01a3df696d8f1f))

# [1.8.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.7.0...v1.8.0) (2023-08-30)


### Features

* Update supported platforms & CI ([a67803c](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/a67803c5fb4bf4aedcdd4b4f4c4024ddfaa1ef58))

# [1.7.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.6.0...v1.7.0) (2023-07-07)


### Bug Fixes

* Add project directory creation ([c8c82e2](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/c8c82e2ec98fa4fa072cd8265c883f95c8040fcd))
* Restrict directories by stripping permissions for others by default ([3f15a90](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/3f15a90bad3aa06bd67b87d446cca2e852e155dc))


### Features

* Add support for SLES/OpenSUSE Leap 15 ([af6e8ff](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/af6e8ffa19e483d80e612005411b3b82862bf2e6))

# [1.6.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.5.1...v1.6.0) (2023-06-21)


### Bug Fixes

* Fix type in restart variable name ([b160f40](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/b160f40020ee010f0cd2fd7fe8e104a29c8b7ba0))


### Features

* Add support for Fedora 38 ([207b387](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/207b3878a0d86602efee51f6efde628db5c77c27))
* Remove support for Fedora 36 ([b51769d](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/b51769d13a48c1960f98757a07973e1a5e485195))
* Remove support for Ubuntu 18.04 LTS ([72bf5b7](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/72bf5b7069bfb11eedd55713a7367df144233fa7))

## [1.5.1](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.5.0...v1.5.1) (2023-06-06)


### Bug Fixes

* Stop using handlers for restarting containers ([bd64c74](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/bd64c74e391496585991bfb47815ff9b496cce80))

# [1.5.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.4.1...v1.5.0) (2023-05-06)


### Features

* Add support for compose files ([b1ab6cd](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/b1ab6cdab71883ea74067f0453825bef60575bcd))
* Move to namespaced role names ([cad235e](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/cad235e1defe34b6cc1840362e25c49f8a9e1470))

## [1.4.1](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.4.0...v1.4.1) (2022-11-27)


### Bug Fixes

* Make this role install both binary and pypi package by default ([64e471a](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/64e471a17ed38a98b9de1a02af2aa4e9bd4d3cd2))

# [1.4.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.3.0...v1.4.0) (2022-11-18)


### Features

* Add support for OracleLinux 9 ([c4d1d5d](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/c4d1d5d567622285830f9c089a99482fb85309f2))

# [1.3.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.2.0...v1.3.0) (2022-10-12)


### Features

* Add support for both pip and binary package ([a09be6c](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/a09be6c68b025c03c1762d88eed6a02f2440e50c))
* Move to FQCN ([87f1cf2](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/87f1cf2af04f653dcf15a5bfea2ffa0b4bbc87dd))
* Update CI to latest standards ([369199e](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/369199e18d19d4b51bce02ec574c6bcb7900500d))

# [1.2.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.1.0...v1.2.0) (2022-07-28)


### Features

* Implement ansible-lint v6 support ([3191395](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/319139591fa4c526c325ac4a6bff35088626c30f))

# [1.1.0](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.0.1...v1.1.0) (2022-07-09)


### Features

* Add support for several newer platforms ([cc99a98](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/cc99a980d1ebcf821944916cfacd639a4ca74cab))

## [1.0.1](https://github.com/de-it-krachten/ansible-role-docker_compose/compare/v1.0.0...v1.0.1) (2022-02-26)


### Bug Fixes

* fix pip install via proxy ([13e0efd](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/13e0efd7e8598f1358d273cf0a5677e47611da13))

# 1.0.0 (2022-01-15)


### Features

* initial release ([f1b7d25](https://github.com/de-it-krachten/ansible-role-docker_compose/commit/f1b7d25f9e81988a17f8f69c20a4688bfb155479))
