# Contents of this directory

Due to security restrictions on the first target system, it was decided to place all files to be installed in the
all files to be installed in the _files_ directory. These files will not be submitted to git.
Therefore, all files in this directory except _README.md_ will be ignored by gitignore.

## Directory structure 

There are two types of files to distinguish:

1. Versioned platform files
2. Host related files

### Versioned platform files

In general, all files of a particular version are stored in a directory corresponding to the version name
in ansible vars, e.g. 0.0.5.

#### Platform files

All platform files

- tailoringexpert-web
- tailoringexpert-bootapp
- tailoringexpert-db

are placed directly into this release directory.

#### Platform libraries

Libraries needed to run the platform should be placed in a _lib_ folder.

#### Tenant plugins

Tenant implementations of platform interfaces are placed in subdirectories of the version directory. 
with their defined Tenant ID.

### Host Files

Host files such as certificates should be placed in a directory corresponding to a host name in the Ansible inventory.