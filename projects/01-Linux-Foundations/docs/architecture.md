# Nortstar Architecture

## Introduction
Northstar is a growing technology company. The company has Linux servers supporting internal applications, engineering teams, operational reports, and sensitive configuration files. The existing setup has problems as described in the [Project-level Readme](../README.md). This system was built to provide a repeatable Linux server administration environment that establishes a sensible filesystem structure, manages identities and permissions, verifies access boundaries, and provides evidence that the environment is working correctly

## Directory structure, Groups and users
The below describes the Northstar directory structure as created in the virtual environment

/srv/northstar -
                |---> development/Readme.md | Group - developers - users - janedev,johndev,marydev
                |---> platform-engineering | Group - engr - users - janeengr,johnengr,maryengr
                |---> security-&-compliance | Group - security - users - janesecurity,johnsecurity,marysecurity
                |---> operations | Group - operations - users - janeoperations,johnoperations,maryoperations
 
## Design decision
The northstar Linux server was organized this way for the following reasons:

+ To store all folders in a neutral shared space which all users can access
+ To store department specific files in groups and ensure that inly authorized users get access to files and folders
