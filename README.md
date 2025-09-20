# ArcGIS Exploration

OBJECTIVES:

Get started with ArcGIS Pro.

## PROCEDURE:

Access ArcGIS Pro

• ArcGIS Pro is a desktop GIS application installed on a Windows operating system. To access ArcGIS Pro, you will login with your ArcGIS Online credential that is the same as what you use for your mySFA login. Refer to the document named Access ArcGIS Pro in D2L.

• If you’d like to have ArcGIS Pro installed on your own computer, please refer to the document named Access ArcGIS Pro on Your Own Computer. However, you would not have access to the network drives, X, Y, and Z.

*Task:*

Open ArcGIS Pro and visit Configure your licensing options to verify your License Type and License Level.
ArcGIS Pro at Different License Level

• Basic provides comprehensive mapping and analysis tools, along with simple editing and geoprocessing tools.

• Standard includes the full functionality of the Basic, with the addition of advanced editing capabilities. It has the ability to create geodatabase behaviors, such as topology, subtypes, domains, and geometric networks.

• Advanced extends the functionality of both Basic and Standard to include advanced geoprocessing.

# An ArcGIS Pro Project

• ArcGIS Pro organizes data management, data processing, and map composition into a project. By default, when an ArcGIS Pro project is saved, a folder of the project’s name is created. Inside the folder, a file of the project’s name with an extension .aprx is saved. In the same project folder, a file geodatabase (a folder with an extension .gdb) and a toolbox (a file with an extension .atbx) are also found.


*Task:* 

Start ArcGIS Pro. At the start page, go to Setting and select Options. Under Application, select General. Under Create projects, check “New projects are saved in a custom location” and assign it to you gisc_5351lab folder. Back to the start page, select the “Start without a template option” to create a new project. named Lab1ProPractice.

## ArcGIS Pro Essentials

• Catalog/Catalog Pane helps you organize and manage all your GIS information, such as maps, globes, coordinate systems, datasets, models, metadata, and services (such as database and server connections). This is also where you search for maps, data, and tools.
Task: Open Catalog View (View/Catalog View) and save the project named Lab1ProPractice in your gisc_5351lab folder. Add Folder Connection to the network drives (X:, Y: and Z:). Find a dataset at Y:\Graduate\GISC5351\texas\tx_nf_dd.shp. Preview the data by Metadata, by Geography, and by Table. Also read the Description of the data. Check its Properties for detailed information including Data Source and Spatial Reference.

• Map is a comprehensive map authoring application for all map-based tasks including cartography, map analysis and editing. This is where you edit your features and compose/print your maps.

*Task:*

Add a new map to the project (Insert/New Map). Add the shapefile tx_nf_dd.shp to the map. Import an existing ArcMap document Y:\Graduate\GISC5351\usa\USA Base Map.mxd (Insert/Import Map) to the project. In the Table of Contents, try to list the layers by Drawing Order, by Data Source, by Selection, by Editing, etc. Check the Properties (Right-click) of the map, and each layer of the map.

• Layout is where the cartographic works (title, scale, legend, north arrow, etc.) are performed and when finalized, a map can be printed for hardcopies and/or softcopies. The map body of the layout comes from a map in the project.

*Task:*

Add a layout to the project (Insert/New Layout). Add a map frame (Insert/Map Frame) of the USA Base Map Data to the layout. Add a new map to the project (Insert/New Map). Change the layout from portrait to landscape (Layout Properties/Page Setup). Find the Map Surrounds and add a map title and other essential map elements. Export the map as a pdf file (Share/Export Layout).

• Toolbox contains a comprehensive collection of geoprocessing functions. It includes tools for data management, data conversion, vector analysis, geocoding and statistical
analysis etc. Each tool here can be run via its dialog box. When an ArcGIS Pro extension is activated, more tools are available in the Toolboxes.

*Task:*

Open the Toolbox in your ArcGIS Pro project (Analysis/Tools). In the Geoprocessing pane, click on Toolboxes to view all of the tools. How many Toolboxes do you have? How many Toolsets are there in the 3D Analyst Tools toolbox? Let’s first export a feature class Y:\Graduate\GISC5351\texas\texas_data.gdb\statewide\tx_county to a shapefile and save it in your project folder. Then, try the Dissolve tool in Data Management Tools (toolbox)/Generalization (toolset). 

The tool should dissolve all of the county boundaries of Texas and output a polygon of Texas state boundary (e.g., tx_state.shp). Try tools in 3D Analyst Tools tool box. What did you see?

• Python Window is another interface for geoprocessing. Instead of using graphic user interface (GUI), it runs tools by typing Python scripts. You will find that it is more efficient if you are familiar with the Python syntax.

*Task:*

Open the Python window (Analysis/Geoprocessing/Python dropdown/Python Window). Type in import arcpy followed by pressing Enter key. Then type arcpy.Dissolve_management and press space bar to see what happens. Let’s try to run this same tool on the Texas counties data in Python window. How do you like it?

• ModelBuilder provides a graphical modeling framework for designing and implementing geoprocessing models. Models are data flow diagrams that string together a series of tools and data to create advanced procedures and work flows.

*Task:* 

In Catalog, navigate to the GISC5351 class folder on the Y drive. Find the toolbox TestModel.atbx. Explore the tools that were built as a model. Select one and view its model design in ModelBuilder (Right-click/Edit). By viewing it in ArcGIS Pro, you can tell that a Model has the icon that is different from others. A model works just like a regular tool when you double-click to Open it.

• Script is a computer language. It can streamline a series of geoprocessing tools and run within its scripting application (e.g., Python), or can be added to a toolbox and run like any other tool from a dialog box. It is powerful in terms of the efficiency when you build a complex procedure.
Task: When the Toolbox is open, explorer to the script of Average Nearest Neighbor (search for the tool through Find Tools in the Processing pane). When the tool is located,
right-click to Open the script. Again, right-click to view the scripting language by clicking on Edit. As you can see, a script has an icon that is different from a regular tool.

• Scene works closely with 3D Analyst extension and lets you make realistic scenes in which you can navigate and interact with your GIS data. In a Scene you can more effectively manage your 3D GIS data, conduct 3D analysis, edit 3D features, and create layers with 3D viewing properties. A Local Scene is suitable for a limited area with more detailed information, whereas in a Global Scene spatially referenced data are placed on a 3D globe surface and displayed in its true geodetic location.

*Task:* 
In your ArcGIS Pro project, import an ArcScene document (Insert/Import Map) located at Y:|Graduate\GISC5351\guadalupe\guada_doqq.sxd. The data will be presented in a Scene that allows you to present GIS data in 3D context. Go to Catalog and look into the Table of Contents. All of your data views are listed in the Maps folder, while all layout views (map compositions) are in the Layout folder.

# Additional ArcGIS Applications

• ArcGIS Earth is a free application for exploring spatial data in the way similar to Google Earth. The Esri’s default view is based on the globe retrieved over the internet. There are different options for the basemap. Also, you can add your own data such as shapefile or KML, or data from ArcGIS Online and other internet sources. A view in ArcGIS Earth can be saved as an image file.
Task: Launch ArcGIS Earth and add the KML file Y:|Graduate\GISC5351\gps\TheWayHome.kml for some animation.

• ArcGIS Online is cloud-based platform that users can create, share and access maps, applications and data including authoritative basemaps published by Esri. With an organization account for ArcGIS Online, you are able to publish rich contents and share edits with other users over the internet.
Task: Open a map in you ArcGIS Pro project. Check the data source of it base map and you will find that it comes from ArcGIS Online over the internet. Add a different base map (Map/Layer/Basemap) and check its source again. Open Catalog and select ArcGIS Online in its Contents (Portal/ArcGIS Online). Search for contents in ArcGIS Online with the key words Stephen F. Austin State University. Open the one on the resulted list that comes as a Map Package. View its metadata to confirm that it is about Points of interest. Open it by right-click/Add And Open. A map will be added to your ArcGIS Pro project. Select the point feature layer and configure its pop-up (Right-click/Configure Pop-Ups) and add an Image item with its source coming from the URL that is stored in a field of its attribute table. View each point of interest feature on the map through its pop-up window.

In addition, open ArcGIS Online in a web browser (http://www.arcgis.com). Without sign-in, search for contents with the same keyword Stephen F. Austin State University. Try any of them on the list.
Need Help?

• Tooltip (Hover the mouse over an item to view brief information)
• ArcGIS Pro help (the question mark on the top-right of the program window)
• Esri Technical Support (http://support.esri.com)

## My First Map

• There are several elements which are essential to a map including map body, title, legend, scale, north arrow (direction rose), acknowledgement (source, author, date) and neat line (map border). Which one is the most important?

• In order to well organize your workspace, you might want to create a specific folder for each lab such as z:\gisc_5351lab\lab1\.

• Open a new ArcGIS Pro project and name it as Lab1Pro. In Catalog, explore the folder Y:|Graduate\GISC5351\texas\. What types of GIS dataset did you see? Preview a dataset by looking at both Geography and Table. Also check its Metadata.

• Insert a new map and rename it as Map Body. Add the layer of Y:\Graduate\GISC5351\texas\torp_region.lyr onto this new map.

• You might find that a layer named tx_county is listed on the Contents but not showing up on the map. It is noted by a red exclamation mark. Check its data source and redirect it to Y:\Graduate\GISC5351\texas\texas_data.gdb\statewide\tx_county.

• Another problem encountered is that the symbology setup is missing a relationship. Work on the layer’s symbology (Right-click/Symbology). Select Unique Values and assign the field REG_CODE for classification.



• Add the annotation from Y:\Graduate\GISC5351\texas\texas_data.gdb\torp_labels. The labels were generated beforehand and saved as feature class in the file geodatabase.

• When the layer is displayed properly, each color represents a planning region based on the Texas Outdoor Recreation Plan.

• Add the features of Texas cities from Y:\Graduate\GISC5351\texas\texas_data.gdb\statewide\tx_city to the same map.

• Set symbology of Texas cities based on the city total population of 2020 (Symbology/ Symbolize your layer by quantities/Graduated Colors based on the field of POP2020). Round the population break values to 10,000s and show thousand separators.

• Insert a new map and rename it as Locator to highlight Texas in the United States (Y:\Graduate\GISC5351\usa\census\states.gdb\states). Change the coordinate system of this map (Map Properties/Coordinate System) to a projected coordinate system such as North America Lambert Conformal Conic (Projected Coordinate System/ Continental > North America). In order to distinguish Texas, use Symbolize your layer by category/Unique Values in Symbology. Add Values of only Texas based on the field of STATE_NAME.

• Insert a new layout and add the two map frames, Map Body and Locator. Add essential elements such as title, scale, legend etc. to complete the map. Each added object can be selected and modified by right-click/Properties.

• A GIS Lab logo graph can be found at Y:\Graduate\GISC5351\gislogo3b.jpg. Insert it as Picture onto you layout. The logo represents your data source of the map.

• When the map is completed, print out the map as a hardcopy for you to keep. In the meantime, export the map as a softcopy in PDF format.

• A sample map for this assignment can be found in the Sample Work module of this course in D2L.

## ASSIGNMENTS:

• Complete your first map (Planning Regions of Texas Outdoor Recreation Plan with Major Cities) similar to the sample map found in D2L.


• Work on a second map as what is shown in D2L (Texas Ecoregions with Interstate Highways) and print it out (letter size). Data for this map can be found at Y:\Graduate\GISC5351\texas\texas_data.gdb\statewide\ecoregion and Y:\Graduate\GISC5351\texas\tx_highway.shp.

• For the second map, use a hillshade layer as background (Y:\Graduate\GISC5351\texas\texashill.tif). Hints: Set transparency on the Texas Ecoregions layer (Feature Layer/Effects/Transparency) and use the field of NAT_REGION for symbology (Unique Values) on this layer. Use proper case (e.g., “Blackland Prairies” instead of “blackland prairies” in finalizing the map layout. In order to block the black background of the Texas hillshade layer, set its Symbology and assign no color for the background value (Symbology/Mask/Display background value). For displaying only interstate highway segments, assign Layer Properties/Definition Query by setting a query where the field of "SIGNT1" is equal to 'I'. For labeling interstate highways, turn on the Label for this layer (Right-click/Label) and work on the label properties (Right-click/Labeling Properties). Select field SIGNN1 for attaining label values (Expression: $feature.SIGNN1). Then choose the symbol of interstate highway shield for display (Labeling/Text Symbol/Shield). Place the symbols horizontally (Labeling/Label Placement/Shield).

• Export each map as a pdf file for the submission.

• Compress your two PDF files of your maps into one zip file. Include your mySFA login username as part of your zip filename as stated in the syllabus, e.g., a1_hungikua.zip. Submit your zip file onto Desire2Learn.

FYI
The most recent Texas Roadway Inventory dataset can be downloaded from Texas Department of Transportation at http://gis-txdot.opendata.arcgis.com/datasets/txdot-roadway-inventory. This dataset contains more than 729,000 line features. The field RTE_PRFX differentiates the type of road such as interstate highway (IH), US highway (US), state highway (SH), and toll way (TL), whereas the field RTE_NBR contains the road number.


# RESULT

## Lab1 Map1 

<img width="688" height="886" alt="Screenshot 2025-09-20 105950" src="https://github.com/user-attachments/assets/7101f968-43d1-42f9-8b75-88fa7b6906bd" />


## Lab1 Map2


<img width="688" height="896" alt="Screenshot 2025-09-20 110214" src="https://github.com/user-attachments/assets/b0cf66a3-5ccd-4ce5-b680-6ba5eb5d05b2" />


