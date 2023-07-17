# sort_by_year
A small shell script that uses exiftool to sort images by copying them into yearly directories.

Really this project was created for a very specific use-case scenario. Whenever you mount an iPhone in Linux, you get huge, unsorted directories called `DCIM/10XAPPLE` in which images are just dumped into. This script lets you choose a directory in which directories named after a year exist or will be created. Within those directories, a new directory is created (called "iphone_pics" by default). The script then sorts the images into `$YEAR/iphone_pics`. A directory is also be created to store untagged images.

To put it visually, here's more or less how my files are now sorted:

```
$ cd /mnt/personal-pix/
$ ls
2018  2019  2020  2021  2022  2023  iphone_nodate
$ ls 2023
cali_trip adventures more_fun_stuff iphone
$ ls 2023/iphone
IMG_0377.HEIC  IMG_0713.MOV   IMG_1034.HEIC ...
```
