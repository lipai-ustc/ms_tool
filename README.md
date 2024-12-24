# ms_tool (Materials Studio tool for batch setup and batch export to vasp format)  

lipai@mail.ustc.edu.cn  

### Batch Processing of Atomic Structures with Materials Studio
Materials Studio offers excellent visualization of atomic structures; however, many settings apply only to individual structures rather than globally. When dealing with a batch of structures that need visualization in Materials Studio (MS), individually configuring each can be inconvenient. Therefore, this small program has been developed to handle batch visualization settings for MS. Additionally, the program supports batch export of structures (in POSCAR or xyz formats) for VASP calculations, among other uses.

Below is an illustration of the program interface:  

<img src="https://github.com/user-attachments/assets/d5b83030-f092-4a57-a80a-c0623d84ed04" width="500">

The program includes two independent modules: Batch Settings and Batch Export, both sharing a common WorkPath.  

Alternative download Link: [Cloud Storage](https://link.zhihu.com/?target=https%3A//pan.cstcloud.cn/s/MBtSe8sPSsQ) 

### Batch Settings Module
This module allows setting configurations for "Lattice", "Atom", and "Background Color". Here's how you can use it:  

<img src="https://github.com/user-attachments/assets/a0c1867f-bdb7-49a2-8852-374b6a3455b6" width="500">

Suppose you have a main directory in MS named metals containing multiple atomic structure models. To modify the visualization settings for all structure models within the metals folder, follow these steps:

Locate the Absolute Path: Right-click on any structure file within the metals folder, select Properties, and note the path shown in the window that pops up.  

<img src="https://github.com/user-attachments/assets/12657518-0991-46b7-80fc-6c16c47e6c44" width="500">

Copy the Path: Highlight the path using your mouse, press Ctrl+C to copy it.

<img src="https://github.com/user-attachments/assets/369a7f3f-ae77-499a-bc29-e1ef5343ff66" width="300">

<ins>**Then close the all small windows of the individual structure models.**</ins> 

<img src="https://github.com/user-attachments/assets/995550d5-4b9d-4349-a4be-dc4fbfe08228" width="500">

Paste into WorkPath: Paste the copied path into the WorkPath field of our program and make the desired settings. Click Apply. 

Element: Specify the elements you wish to modify. If set to `All`, changes will apply to all elements.  

<img src="https://github.com/user-attachments/assets/83bac947-8718-48d9-8a98-17485421554d" width="500">

View Changes: Reopen the structure model windows in Materials Studio to see the updated visualization settings.   

<img src="https://github.com/user-attachments/assets/b9cdb258-7858-4a9b-82c4-b90dded66272" width="500">

### Batch Export Module
This module enables batch exporting of structures in either POSCAR or xyz format.  

<img src="https://github.com/user-attachments/assets/32fb317e-56f0-4049-9db3-3ab53ee49371" width="500">

<ins>**Before performing batch export, ensure that all structure model windows are closed (Close All).**</ins>

WorkPath: This is the path to the folder in MS (e.g., the metals path mentioned earlier). The method to obtain this path is the same as described above (Properties).
Exporting Structures: In the batch export feature, there is a "Path" field where exported structure files will be saved. By default, the export location is the user's desktop. Choose the desired format (POSCAR or xyz) from the Format dropdown menu. Click Save to export all structure files within WorkPath (including those in subdirectories) to the directory specified in the "Path" field.

File Naming Convention:
Structures directly under WorkPath are saved as filename.vasp (or .xyz).
Structures within subdirectories are saved as foldername~filename.vasp (or .xyz).

By following these instructions, you can efficiently manage the visualization settings and export of multiple atomic structures in Materials Studio. This tool significantly streamlines the process when working with large datasets, ensuring consistency and saving time.

Enjoy!
