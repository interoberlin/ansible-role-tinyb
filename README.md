# Ansible Role: tinyb

Installs tinyb.

## Requirements

None.

## Role Variables

    packages:
    - libglib3.0-cil-dev
    - libglib2.0-dev
    - clang
    - openjdk-8-jdk
    - cmake

Packages to be installed before tinyb installation.

    tinyb_sha1: 'd9c777bc576b5365c2064d55fe872f272faa92e8'

tinyb hash.

    cmake_cxx_flags: 'set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")'

make flags that are used during installation.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - { role: interoberlin.tinyb }

## License

GPLv3

## Author Information

This role was created in 2016 by [Florian Schwanz](https://interoberlin.de/).
