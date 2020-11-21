Spiking

    Using generic_send)_tcp to do the spiking on a test non vuln part of the server  

        Stats.spk 

    s_readline(); 

    s_string("STATS "); 

    s_string_variable("0"); 

        Sends a lot of data to try to spike the STATS service  

        generic_send_tcp 10.0.2.4 9999 stats.spk 0 0 

        In a real test we would let it run all the way through  

        Below is the example of the Immunity debugger on a sucessful spiking  

![GetImage.png](../../_resources/5362b18c2747457398ac87bb404bb4a5.png)

