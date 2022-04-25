


We begin with an NMAP scan of the target IP.

![1](https://lh3.googleusercontent.com/KtQ090VJ9Lyndr4zxta1T-VAw3usQ7EsyMwAZuuurMZ-vmpSEMDjG8K1ayJUvG3DbpyYuohAwD3uBEWoFI2BJ47RlXBYbMWOotEyQJqDkT60_Uc8UoLVaCWqQqLsQstRuwUHMtvL)

We discover that a Telnet service is open, on port 23. Let's investigate.

![2](https://lh6.googleusercontent.com/9B6QWcBRyvmymiP6o07xn1lH9xl3qpjupfJYW-ika4v_hmJUAS7iraYQJmgcVXZv8tr_Yyt_ha7g2L_O10Ym6W0u7e74_t_ezmVjwaKgxUSigr9ihOwNFQjdSeAV6BpgvzSwRqQG)

Connecting to the service prompts us for a login.

![3](https://lh6.googleusercontent.com/99zxGpn3O-avRCJe5vmhYzz33var92P40z1Pe9OnvkayePBXnOqC-l5fp7e-o8ZQ_fdhIJ3BMYK1kTilqr5H2HRpiAdJtiiYFoDmDZUzJhM5GXChPJqRDJyAbCp7vcGXXsEFq330)

Login Root with no passwords works. 

![4](https://lh3.googleusercontent.com/6PTxvAMJaOXgEJbKz0ZUVTRAZWxHks7e4pSnbq3BUKzkRv-AHs6lmKTuUBfXhZe3dnfBOTUGj-rkLNQlR1ypUQ8M3_f8XOmTLUdvBlrdWEt_4bVtdVh_3HJo4zkvvtYKm5VbOcfK)

Once in, we LS, find flag.txt, and cat it.
