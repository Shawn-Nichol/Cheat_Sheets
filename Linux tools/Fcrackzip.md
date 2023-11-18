Searches each zipfile given for encrypted fiels and tries to guess the password. All files must be encrypte with the same password, the more fiels you provide the better. 


EXAMPLES
       fcrackzip -c a -p aaaaaa sample.zip
              checks the encrypted files in sample.zip for all lowercase 6 character passwords (aaaaaa ... abaaba ... ghfgrg ... zzzzzz).

       fcrackzip --method cpmask --charset A --init AAAA test.ppm
              checks the obscured image test.ppm for all four character passwords.

       fcrackzip -D -p passwords.txt sample.zip
              check for every password listed in the file passwords.txt.
