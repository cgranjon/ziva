# ziva
A collection of scripts for ZivaVFX

Please keep in mind that all scripts are based of my use of the software, some of the tools might not work properly in your setup.

At the moment, warning and error messages might not be coded to guide the user.

_____________________________________________________________________________________________________________
# ziva_loa_rebuild.mel
Please make sure that you have all dependencies listed below before using:
- https://plus.google.com/108730905615837309068/posts/GdL56AbxQ32

Names are important:
- all rivets must have a prefix "L" or "R" and a suffix "_rivet#" (automatic if created via command) 
- all curves must have a prefix "L" or "R" and a suffix "_LOA" (automatic if created via command)


How to use ?
The script is a collection of commands, here how to use them.


How to create a rivet ?
Select two polygon edges and run cg_ziva_create_rivet_check();


How to create a curve to drive a zLineOfAction ?
Selection order is important. Select two rivets first and then a muscle (on that has a zTissue and a zFiber on it) and run cg_ziva_create_loa();


How to import/export my setup ?
Use cg_ziva_write_loa_setup_ui();


How to mirror my rivets and curves setup ?
At the moment it is designed to work with zTissues with zFiber only, so the script will not work if you did not build the setup attaching it to muscle(s) at the same time. Select your setup (rivets + curves) and run cg_ziva_mirror_loa_setup();
