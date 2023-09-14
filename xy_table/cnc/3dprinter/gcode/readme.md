Exports from https://cnc-apps.com/en/app/texttogcode_line works. But all M1002 commands needs to be removed 

 cat thanks.nc | grep -v "M1002" | tee thanks_edit.nc 

and the a feed rate must be apllied to teh first G commands:

G00 X25.30859 Y76.38299 F1000

G01 X24.77777 Y58.77819 F1000
