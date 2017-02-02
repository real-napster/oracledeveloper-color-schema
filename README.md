# oracledeveloper-color-schema
Microsoft SQL-Server Managemnt Studio color scheme for Oracle SQL Developer

# Installation

Unfortunately Oracle doesn't make it easy to import a new colour scheme into SQL Developer, thus a little bit of hacking is required.
* Close SQL Developer. This is important! If you modify the scheme file while SQL Developer is open, your changes won't be saved.
* Locate file `dtcache.xml` in the SQL Developer's settings directory.
  * On my system `C:\Users\Username\AppData\Roaming\SQL Developer\system4.1.5.21.78\o.ide.12.2.1.0.42.151001.541`
* Locate `<schemeMap>` tag inside `dtcache.xml` file.
* Insert the content of `ssms.xml` file inside `<schemeMap>` alongside the other colour schemes. Be careful not to break the XML.
* Launch SQL Developer. Navigate to menu Tools -> Preferences, then select item Code Editor -> PL/SQL Syntax Colours in the left pane.
* Select "MS SQL" in the "Scheme" drop down list on the top.
