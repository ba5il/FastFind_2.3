# FastFind_2.3
Rebuild original FastFind UDF by FastFrench. Some errors fixed, new function added, window snapshot function rebuild.

1. Now the SnapShot function takes a screenshot of a desktop at the coordinates of the window set by FFSetWnd(). So if the window is overlapped it will be overlapped in the snapshot. If the window is minimized you will get an error. Without window handle the function captures the whole screen as it used to.

2. You can pass any number of coordinates to FFSnapShot(). In previous versions you had to write all four coords even if you needed to pass only Left or Left,Top. Now, if Top is omitted it will be 0. If Right or Bottom are omitted they will get a value of a window width, height.

3. The last version (year 2015) of C++ project of the author on GitHub is fully Unicode, so some changes were made to the UDF file.

4. New function (LoadFromFile) was also implemented by the author in the project. I added it to the UDF - FFLoadFromFile('file path' [, snapshot_num])

DLLs are embeded.
