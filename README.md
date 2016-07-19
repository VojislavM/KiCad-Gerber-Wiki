# KiCad-Gerber-Wiki
Documentation how to generate Gerber files from KiCad for PCB manufacturing at [dirtypcbs][DIRTY_PCB_LINK]. 

On this link, you can find all information about [dirtypcbs info][DIRTY_PCB_ABOUT_LINK] PCB manufacturing. 

There are several things need to be done before sending files to manufacture PCBs. Files are generated with KiCad EDA tool, and these are the steps to send your files to [dirtypcbs][DIRTY_PCB_LINK] and get your boards as you want.

When board file is finished:
1. Set the origin: Go to **Place** -> **Drill and Place offset** and then set the origin near the corner of the board.
2. Generate Gerber files PDF: Go to **File** -> **Plot**. New Window will appear, like in picture 1. Click on **Plot** and it will generate Gerber files in PDF form so they could be checked. 

![Picture 1][pic1]

3. Generate Gerber files: In the same window click change the **Plot format** from PDF to **Gerber**, a window will change and it will look like in picture 2. Some additional boxes need to be checked and everything should be like in picture 2. Then click on **Plot** and Gerber files will be generated.

![Picture 2][pic2]

4. Generate Drill File: Next click on the **Generate Drill File** and the new window will appear, like in picture 3. Again everything should be like in picture 3. When everything is set click on **Drill File**, and Drill file will be generated. 

![Picture 3][pic3]

5. Change extensions: Extensions of files that contains Edge of the board and Drills needs to be changed. Go to project folder, than go to folder **/Gerber** and change extensions for Drill file from **.drl** to **.txt** and Edge (keepout) file from **.gm1** to **.gko**.


After that everything is ready, just check your Gerber files in Gerber viewer and send them to manufacturing.




[//]: # (These are reference links used in the body)
[DIRTY_PCB_LINK]:<http://dirtypcbs.com/>
[DIRTY_PCB_ABOUT_LINK]:<http://dirtypcbs.com/about.php>
[pic1]: https://raw.githubusercontent.com/VojislavM/KiCad-Gerber-Wiki/master/pictures/plot_pdf.png
[pic2]: https://raw.githubusercontent.com/VojislavM/KiCad-Gerber-Wiki/master/pictures/plot_gerber.png
[pic3]: https://raw.githubusercontent.com/VojislavM/KiCad-Gerber-Wiki/master/pictures/drill_files.png