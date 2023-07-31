# Exploring-mininet

It is highly recommended that you carry out the programs in a Linux system/subsystem with following
dependencies

-> g++ installed

-> mininet installed

-> xterm installed

-> python installed [also python Mininet API]

Also the largest file ‘warandpeace.txt’ ~[3.2 MB] is also present
Various commands
1)
Link topology with 2 hosts and 1 switch with varying bandwidth

```console
$ sudo mn --link=tc,bw=10 //for 10Mbits and similarly for others
mininet> xterm h1 h2
```
[this will launch two xterm windows, run the server in the ‘h1’ window and the client in ‘h2’]

Link topology with 2 hosts and 1 switch with varying delay

```console
$ sudo mn --link=tc,delay=1ms,bw=1000 //for 1ms delay and similarly for others
mininet> xterm h1 h2
```
[once again repeat the steps as given in varying bandwidth part]
```console
$ sudo mn --link=tc,loss=1,bw=1000 //for 1% link loss and similarly for others
mininet> xterm h1 h2
```
[once again repeat the same steps]
For the last experiment we have to run custom mininet programs using python
(all the files have been submitted)

```console
$ sudo python switch_2.py //for 2 switches and similarly for others
mininet> xterm h1 h2
```
[once again repeat the same steps]
Sample screenshot(s) of the same
