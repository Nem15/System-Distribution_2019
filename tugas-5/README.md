# Test Method #
- Run the pyro nameserver.
   shell
     pyro4-ns -n localhost -p 50001
   ``
- Create a directory for the fileserver in accordance with the name of the fileserver. In this work, the names fs1 and fs2 are used.
   shell
     mkdir fs1 fs2
   ``
- Run the server using the file server.py with the program input parameter being the name of the fileserver. In this work, the names fs1 and fs2 are used.
   shell
     python3 server.py fs1
   ``
- Run the shell script assign_fs_id.sh to set the id of each fileserver instance that has been created.
   shell
     bash assign_fs_id.sh
   ``
- Run client.py to start using the fileserver accompanied by the name of the fileserver accessed by the client.
   shell
     python3 client.py fs1
   ``