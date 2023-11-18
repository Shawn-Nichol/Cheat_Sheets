Steghide is a steganography y program that is able to hide data in various kinds of image and audio files. 

Features include the compression and encryption of the embedded data and automatic integrity checking using a checksum. The JPEG, BMP, WAV, and AU file formats are supported for us as cover file. There are no restrictions on the format of the secret data. 


EXTRACTING
       If you have received a file that contains a message that has been embedded with steghide, use the extract command to extract it. The following arguments can be used with this command.

       ‐sf, ‐‐stegofile filename
              Specify the stego file (the file that contains embedded data). If this argument is omitted or filename is ‐, steghide will read a stego file from standard input.

       ‐xf, ‐‐extractfile filename
              Create  a  file  with  the name filename and write the data that is embedded in the stego file to it. This option overrides the filename that is embedded int the stego file. If this argument is omitted, the embedded
              data will be saved to the current directory under its original name.

