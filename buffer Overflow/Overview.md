Overview 

    Buffer space grows downward  

        If you fill the buffer space fills with like a bunch of A's and stops 

        Buffer overflow goes beyond the buffer space and into the EBP 

        After you fill the EBP you get to the EIP which will really be code to give us a reverse shell  

    Steps to conduct a buffer overflow 

        Spiking  

            Finding the vuln part of a program 

        Fuzzing 

            Sending the characters to overflow 

        Finding the offset 

            Finding the point where it was overflown 

        Overwriting the EIP 

        Finding Bad Characters 

        Finding the Right Module 

        Generating Shellcode 

        Reverse shell to get root  