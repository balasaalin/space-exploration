# space-exploration
#### Demo project containing the sample files for the Oxygen WebHelp Publishing Template [presentation video](https://www.youtube.com/watch?v=Q0rZy1oyyUk).  

This is a demo project that introduces the concept of the Oxygen Webhelp [Publishing Template](https://www.oxygenxml.com/doc/ug-editor/topics/whr-publishing-template.html) that defines all aspects of the layout and
style of WebHelp Responsive output. 

The project contains a sample DITA map and a publsihing template that customizes the WebHelp Responsive output by changing the font and color of several sections and adds a background and logo image.

The possible benefits for using the publishing template package include:
- You can use any of the existing built-in templates as a starting point for future customizations
- The customized template packages are easy to share with others (read more [here](https://www.oxygenxml.com/doc/ug-editor/topics/whr-share-tempates.html))
- Custom template packages remain intact even when you upgrade Oxygen to a new version
- A publishing template can be easily integrated with a continuous integration publishing system

Each WebHelp Responsive publishing template is a package that contains a [descriptor](https://www.oxygenxml.com/doc/versions/20.0/ug-editor/topics/whr_publishing_template_contents.html#ariaid-title2) file and
various resources. The descriptor file controls the template package by defining the references to the
other resources in the package.
![Publishing Template package](https://github.com/balasaalin/space-exploration/blob/master/resources/PubTemplatePackage.png)

# Project layout
This project has the following layout:
- **map** - Contains a DITA map sample along with its referenced DITA topics
- **templates** - The [Publishing Templates Gallery](https://www.oxygenxml.com/doc/ug-editor/topics/whr-pt-feature-gallery.html) stored at project level
  - **space** - The Publishing Template package (read more about the [package contents](https://www.oxygenxml.com/doc/ug-editor/topics/whr_publishing_template_contents.html))
    - **img** - Contains the logo image and the background image used in this template. It also contains the template's preview image.
    - **light.css** - The base CSS that defines the styles of the WebHelp output
    - **space.css** - Additional CSS styles
    - **Space Exploration Blue.opt** - The Publishing Template descriptor file
- **resources** - Project miscellaneous resources
- **space-exploration.xpr** - Oxygen project file

# Getting started
1. Load the `space-exploration.xpr` project file in Oxygen
1. Open the `map/space-videos.ditamap` DITA map in the *DITA Maps Manager* view
1. Open the *Configure Transformation Scenario(s)* dialog
1. Duplicate the *DITA Map WebHelp Responsive* built-in transformation scenario
1. Select the *Space Exploration Blue* template 
1. Click *OK* to save the scenario
1. Apply the transformation scenario to publish the DITA map to WebHelp Responsive format.
