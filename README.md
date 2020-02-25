# Ansible Role: Install required tools

Install a set of tools required to build CCDC C++ applications.

### Linux

- curl # for downloads
- wget # for downloads
- doxygen # for building documentation
- graphviz # for building documentation
- jfrog-cli # for connecting to Artifactory

### macOS

- xz # efficient compression
- wget # for downloads, curl is part of the system
- doxygen # for building documentation
- graphviz # for building documentation
- jfrog-cli-go # for uploading to artifactory
- ninja # for fast builds
- cmake
- swig

### Windows

- 7zip.install # for installer creation
- 7zip.portable
- curl # for downloads
- wget # for downloads
- doxygen.install # for building documentation
- graphviz # for building documentation
- jfrog-cli # for uploading to artifactory
- ninja # for fast builds
- cmake
- swig
- sysinternals

## Requirements

None.

## Role Variables

None.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - ccdc-cpp-required-tools

## License

MIT / BSD

## Author Information

This role was created in 2020 by Claudio Bantaloukas, based on existing roles at CCDC, by Jeff Geerling and google searches