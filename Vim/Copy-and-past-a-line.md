# Copying and moving text Yank, Delete, PUT

The vi command-mode equivalent of "copy and paste" is yank and put; the equivalent of "cut and paste" is delete and put.


##Copy Lines

    :yy or :Y   #(Yank) To copy a line
    :11yy # to yank 11 lines 
    :p    # To paste a below
    :P    # To paste above

## Moving lines

    :dd # delete
    :5dd # delete 5 lines
    :p    # To paste a below
    :P    # To paste above

# Using name buffer to repeatedly insert a group od lines
  
  You specify named buffers by preceding a command with double quotes (") and a name for the buffer
    :"a4yy" # to yank four lines into a the buffer called a.You can overwrite named buffers with new lines 
    :"b3dd" # to delete 3 lines into the named buffer b
    :"bp"  # insert the lines saved in buffer b below
    :"bP"  # insert the lines saved in buffer b above


[source](https://docs.oracle.com/cd/E19455-01/806-2902/editorvi-53/index.html)

