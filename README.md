# Forensics-Tasks
--> Zeroeth task is to extract the given tasks from a protected zipped folder.
    Using the Tool-'Fcrackzip' in Linux, got it.
  password found was "aaa"
--> b_challenge3.jpg
        |FLAG FOUND|== <Freedom.jpg> //Embedded file
        Tool Used: Binwalk
        Used for: Extracting the embedded data in files.
        Command used: binwalk <filename>, in Linux
--> E_challenge3.jpeg
         |FLAG FOUND|==696e6374667b337831663730304c5f69735f673030645f
         Tool Used: Exiftool
         Used for: Display Metadata of a file.
         Command Used: exiftool E_challenge3.jpeg // found flag as comment in metadata. 
--> s_challenge3.jpg
        |FLAG FOUND|==aW5jdGZ7c3RyaW5nc19hcmVfdXNlZnVsfQ //special sentence
        Tool Used: Strings
        Used for: Printable characters in file.
        Command Used: strings s_challenge3.jpg 
--> SS_challenge3.png
        |FLAG FOUND|==pctf{st3gs0lv3_ls_u53ful} // in red plane
        Tool Used: StegSolve
        Used for: 
        Command Used: java -jar stegsolve.jar
--> Z_challenge3.png
        |FALG FOUND|==flag{N0w_y0u_a_little_about_zbarimg}
        Tool Used: Zbar
        Used for: Read QR-code
        Command Used: zbarimg Z_challenge3.png
        
    
