
https://www.pgmodeler.io/support/installation

On all supported platforms, the first requirement is the Qt framework in the latest major version 6.x. At the moment these instructions were being written, Qt 6.4.2 was the latest stable version. Make sure to use a compatible version to avoid any further problems in the steps below. Bear in mind that failing to observe this first requirement in most cases will cause the compilation to fail due to incompatibilities between the pgModeler's source code and the Qt framework, or even the deployment steps below may not be enough to make the software work after a successful build.

Second, you will need a PostgreSQL installation. In this document we are using the RDBMS in its version 15, so note that the location of headers and libraries in the settings below may vary depending on the version of the database system you've chosen.

Finally, you will need to download a fresh copy of pgModeler's source code. See the source download form for more details about retrieving the source code. Once retrieved the source code, you have to extract it (in case of using a tarball) and run all the commands in the below sections from the root folder.


Important notes

1) Some Linux distros already deliver Qt framework runtime libraries and development packages, but in some few cases, the system installs different versions of the framework causing incompatibilities during the execution of the compilation procedures, so in order to make this step-by-step as simple as possible make sure to be using the Qt version compatible with the codebase being built.

2) Due to the constant improvements in the Qt framework some deprecation warnings may be displayed during the building process. These warnings are harmless in 99% of the time but if the build is aborted due to errors that may point out some incompatibility, please, report it as soon as possible so a patch can be applied to pgModeler's source.
