Role Name
=========

An opinionated role that installs Gradle. Has the ability to install and configure different versions on both the system level and on a user level.

Requirements
------------
No external requirements.

User centric version configuration requires that environment variables and path additions be read from ~/.profile.d/ in a similar fashion as /etc/profile parses /etc/profile.d/

Role Variables
--------------

`gradle_version` : [string] (required) The Gradle version which should be installed. Find available versions [here](https://gradle.org/releases/).

`gradle_version_checksum` : [string] (required) The checksum for the relevant version's binary only ZIP package as published [here](https://gradle.org/release-checksums). 

`gradle_global` : [boolean] (optional) Indicates if the requested Gradle version should be configured to be the default version on the system level (default: true)

`gradle_users` : [list] (optional) Contains user names on the system which should have the requested Gradle version be configured specifically for them, overriding the system level default.  

`gradle_user_home` : [string] (optional) The path within the user's home directory that should be set as the environment variable GRADLE_USER_HOME (default: ~/.gradle).



Dependencies
------------

None.

Example Playbook
----------------

TODO

License
-------

MIT license. See attached license file.

Author Information
------------------

Find me at https://www.hth.is
