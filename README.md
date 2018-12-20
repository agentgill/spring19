# SFDX  App

Demo Build for Salesforce Weekly Blog (Spring 19 Pre-release)

## Dev, Build and Test


## Resources


## Description of Files and Directories
- Application Custom Object
- Application Layout
- Application Permission Set
- Application Custom Tab
- New Application Lightning Flow


## Setup Scratch Org

1. Create scratch org `sfdx force:org:create -v play  -s -a test -d 3 -f config/project-scratch-def.json`
2. Push source `sfdx force:source:push -u test`
3. Assign Perm Set `sfdx force:user:permset:assign -n Application_Permission` 


## Pull metadata from non-scratch org (Reference only)

1. Pull source from Dev Org `sfdx force:mdapi:retrieve -r ./mdapipkg -u play -k package.xml`
2. Unzip source `unzip ./mdapipkg/unpackaged.zip -d ./mdapipkg/` 
3. Convert source into sfdx `sfdx force:mdapi:convert -r ./mdapipkg/unpackaged`  


