# **openEHR Clinical modelling tools setup**

These instructions will guide you through the process of setting up your computer with a set of openEHR clinical models (archetypes and templates), and a number of tools that will let you create new models or modify existing models.

## **Non-Windows systems**
Please note that the current Archetype Editor and Template Designer will only work with Windows, but it is not critical that every course participant has access to the tools during the workshop. It is generally beneficial for participants to work in small groups, and there are usually a sufficient number of Windows machines available.

For interest, a new set of open-source web-based tools is in early development and can be found at these links.  
[Archetype Designer](http://ehrscape.marand.si/designer/)  
[Template Designer](http://ehrscape.marand.si/designer/)  
[Source Code](https://github.com/openEHR/adl-designer)  

Please note that these tools are not yet suitable for training use.



## **A. Download and install the XMIND freeware Mindmap tool**

As clinical modellers we make extensive use of mind map tools and find that the free XMIND tool is one of the best. It works on Windows, Linux and MacOSX.

![XMIND](./images/xmind_logo2.png)  

You should download XMIND from [XMIND installer](http://xmind.net/downloads/).



## **B. Download and install the openEHR Archetype Editor**

The Archetype Editor is the tool we use to create and adapt archetypes.

![](./images/ae_screen.png)

Download the [latest version](http://www.openehr.org/download_files/archetype_editor/archetype_editor_2.8.972.1-windows_32bit.exe) of Archetype Editor.

This installs the openEHR Archetype Editor (ArchetypeEditor.exe) in the folder …

``C:\Program Files\openEHR\Archetype Editor`` on Windows-32 systems
``C:\Program Files(x86)\openEHR\Archetype Editor`` on Windows-64 systems

and should set up links on your Desktop or Start Menu etc.

Further details are available at the [openEHR Archetype Editor Download page](http://www.openehr.org/downloads/archetypeeditor/home).



## **C. Download and install Ocean Template Designer**

The Ocean Template Designer is a free download available at …

[Ocean Template Designer Latest Beta Release](http://www.openehr.org/download_files/TemplateDesigner/TemplateDesignerSetup_2.8.94.2.exe)

Once installed you can run the Template Designer from the Desktop or Start Menu.  

![](./images/td_screen.png)

Further details are available at the [openEHR Modelling Tools Page](http://www.openehr.org/downloads/modellingtools).



## **D. Download models from freshEHR github**

Go to the [freshEHR github page](https://github.com/freshehr/openehr_tool_docs). At the point you can either download the entire github repository as a zip file or - if you are familiar with using github - you can clone the repository.

If you have downloaded the repository, you then need to unzip it a location of your choice, e.g. openehr_training. You should have a folder structure like this:

```
* docs
* images
* models
	* ckm
		* local
			* archetypes  
				* cluster  
				* composition  
				* demographic  
				* entry  
				* section  
		* remote
			* ...
	* local
		* archetypes
			* ...
		* templates
* technical

```

## **E. Setup the openEHR Archetype Editor**

Run the Archetype Editor from the Desktop or Start Menu.

At the initial screen, open any existing archetype on your system e.g. one of the CKM archetypes previously downloaded

``..\Documents\models\ckm\remote\archetypes\cluster\OPENEHR-EHR-CLUSTER.device.v1.adl``

Or one of the sample archetypes provided at

..\Users\Public\Documents\My Clinical Models\Sample Set\Archetypes

### **Set the default Archetype Editor paths**

     Go to ``Tools->Options->File Locations`` and set both

          **Archetype Repository path**  
          and  
          **Archetype XML Repository path**  

      to    ``..\Documents\openehr_training``  

![](./images/ae_tool_setup.png)

### **Setup User Defaults**

Go to ``Tools->Options->User Defaults``

and enter your details e.g.

```
Name: Ian McNicoll

Email: [ian@freshehr.com]
Organisation: freshEHR Clinical Informatics, UK
```
![](./images/ae_user_setup2.png)



## **F. Setup Template Designer**

Run the Template Designer from the Desktop or Start Menu.

Go to ``Tools->Knowledge repository->Edit Repository List``

1. Add a new Repository e.g. ``openEHR Training``  

![](./images/td_setup_repo_1.png)

2. Complete these paths…

  **Archetype Files**

 ``..\Documents\openehr_training\CKM``

 **Working Archetype Files**

 ``..\Documents\openehr_training\local\archetypes``

 **Template Files**

 ``..\Documents\openehr_training\local\templates`` 

![](./images/td_setup_repo_2.png)



## **G. Install ADL Workbench (optional)**

The Archetype Workbench is a technical tool used for experimentation and testing, and it is not usually required by archetype authors.  

The latest version is available at
[openEHR ADL Archetype Workbench](http://www.openehr.org/downloads/ADLworkbench/home)



## **H. CKM resources**

[openEHR CKM](http://www.openehr.org/ckm/): Models maintained by the international openEHR community.

[NEHTA CKM](http://dcm.nehta.org.au/ckm/): Models maintained by NEHTA for the Australian national eHealth program.

[UK CKM](http://clinicalmodels.org.uk/ckm): Models maintained by a consortium of UK health organisations.

[Norwegian CKM](http://arketyper.no/ckm/): Models maintained by the Norwegian national eHealth program.

[Slovenian CKM](http://ukz.ezdrav.si/ckm/OKM.html): Models maintained by the Slovenian national eHealth program.



## **I. Tools Internationalisation**

The Archetype Editor and Template Designer can be setup to use non-English languages.

[Instructions on setting language and other internationalisation options](./docs/tools_internationalisation.md)
