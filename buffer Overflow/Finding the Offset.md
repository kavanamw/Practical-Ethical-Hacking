Finding the Offset 

    Looking where to overwrite the elp 

    Patterncreate  

        Part of the metasploit framework 

        /usr/share/metasploit-framework/tools/exploit/pattern_create.rb -l 3000 

            3000 because that’s right about where the last program crashed  

    /usr/share/metasploit-framework/tools/exploit/pattern_create.rb -l 3000 -q 386F4337 

        When runs it returns the exact offset of 2003 

        Means that somewhere in the pattern_create it found 386F4337 and returned 2003 bytes 

            At exactly 2003 bytes you can overwrite the EIP 
            

![GetImage.png](../../_resources/c606ae43b80a46018d0449f85c0ea56d.png)

