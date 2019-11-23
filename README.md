# mstr-bom
This is the Buid Of Materials used as parent for any MSTR Web component.

Use this component as your MSTR Component base. It provides references to all MSTR jar files needed to build your MSTR components.

You need to add the JARs in your maven repository (<user_home>/.m2/repository). To install the JAR files, there is a Window BAT script located in folder: mstr_config. Inside this folder, there is a folder per respective MSTR version, and all Jar files for such version are are included along with the BAT file.

For instance, MSTR v10.4:
mstr_config/
  mstr_lib_104/
    mvn_install_mstr_jars_104.bat
    
    
This BOM is used mainly as:
 - Parent for mstr-plugin-bom: this is the BOM used to build your custom MSTR Web SDK plugins
 - Parent for your MSTR Web app; you need to create a maven project that will include your MSTR Web content. Make sure to remove the JAR files from WEB-INF/libs. If you need an example, please send me an email to daniel@mstrsdk.com

---

This BOM was provided by [MSTR SDK](https://www.mstrsdk.com)

Written by [Daniel Parra](mailto:daniel@mstrsdk.com)

November 2019
