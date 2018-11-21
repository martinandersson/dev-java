# A Java development environment

This project is effectively a "fork" of [dev-mini][intro-1], with the addition
of software for Java development.

Clone or otherwise copy-paste repo, then do `vagrant up`.

[intro-1]: https://github.com/martinanderssondotcom/dev-mini

## Software

Latest and greatest of the following apps will be installed during provisioning:

|                                 | Version on 2018-11-21     |
| ------------------------------- | ------------------------- |
| GitKraken                       | 4.1.1                     |
| Gradle                          | 4.10.2                    |
| Ubuntu-default JDK              | OpenJDK 11.0.1 2018-10-16 |
| IntelliJ IDEA Community Edition | 2018.3                    |
| Visual Studio Code              | 1.29.0                    |

Please note that versions installed might be different if the machine is setup
and provisioned on any other date than what is specified in the table header.

## A note on Java's runtime

Java is installed by adding packages `default-jdk` and `default-jdk-doc` (see
[this line][1]). Adding these packages basically translates to a bunch of crap
dropped in `/usr/lib/jvm/`, most importantly; the real deal is dropped in
`/usr/lib/jvm/java-11-openjdk-amd64/`.

IntelliJ will do a rather good job picking up both the runtime as well as the
API docs from said folder. However, there exists no package "default-jdk-source"
and for this reason alone, it has not gone into the Ansible playbook which I am
trying to keep "version independent". If you want the source files, then they
must be added manually:

    sudo apt-get install openjdk-11-source

This translates to a ZIP file being downloaded into a slightly different
location: `/usr/lib/jvm/openjdk-11/lib/src.zip`.

[1]: https://github.com/martinanderssondotcom/dev-java/blob/fe12e035de03666a1277709531090b5b84a9cad2/provisioning/playbook.yml#L41