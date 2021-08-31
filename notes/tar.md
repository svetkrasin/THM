#Create an archive

tar cf archive.tar file1 file2 folder/

#List an archive

tar tf archive.tar

#Extarct an archive

tar xf archive

#Create an incremental archive
##Create the level 0 backup
tar cWf archive.tar --listed-incremental=reference.snar --level=0 folder
##View and verify the contents of the **level 0** backup by using tar
tar tf reference.snar --incremnetal
##Create an incremental backup
tar cWf archive_new.tar --listed-incremental=reference.snar folder
