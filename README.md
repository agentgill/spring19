# SFDX  App

## Dev, Build and Test


## Resources


## Description of Files and Directories


## Pull metadata from non-scratch org

Pull source from Dev Org `sfdx force:mdapi:retrieve -r ./mdapipkg -u play -k package.xml`
Unzip source `unzip ./mdapipkg/unpackaged.zip -d ./mdapipkg/`  `
Convert source into sfdx `sfdx force:mdapi:convert -r ./mdapipkg/unpackaged`  
Push source into Scratch Org `sfdx force:source:push -u XXX`  
