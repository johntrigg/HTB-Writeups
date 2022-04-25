


We begin with an NMAP scan of the target IP.

![1](https://lh3.googleusercontent.com/nqxqGNIPHM2RbMFcsc5cQ-ocSqn5-apSVmLpLMCQ5ZEC2QVGCBIBCi3Z-Up-4LFGpmRelJOiA4bmFlsY88lR9-isNvKkakwlt6sW6Fz89Sh0pIUd0uMziCD3zBtW2CO62Qio7VC7)

We discover that a FTP service is open, on port 21. We use Hydra to with a wordlist and manually guess usernames, until we find something that works.

![2](https://lh6.googleusercontent.com/sH_9X8oRRow2j6DrS4uXgo-QRXZEfzrollzfkdQmK60mfeieOo_Lbx2wRQS6VLjd8hgt1GIurNTsKoGixqnGWye6RKqB1ksEIaCdPe1vPacz2R6X_ZdGuBw1ynnOSp8jsImV0jNv)

We find the login "ftp:1". We login using ftp to the destination.

![3](https://lh6.googleusercontent.com/6SdZ_OuaobPyXni2HeJn7-w6ou5Nox4nwdO3UQIKRyrfFMLlt9Ff-BlFjFV6XvSNzXBgqAnY7no9sxRmGXpAYNTWsecqxg3fEJv9mKU1Hl-AjJum7TEuxO2zX0qzbaSsSPA4ZlTX)

From here, we're in. We ls to see what's here, and immediately find the flag. We exfiltrate it.

![4](https://lh6.googleusercontent.com/6SdZ_OuaobPyXni2HeJn7-w6ou5Nox4nwdO3UQIKRyrfFMLlt9Ff-BlFjFV6XvSNzXBgqAnY7no9sxRmGXpAYNTWsecqxg3fEJv9mKU1Hl-AjJum7TEuxO2zX0qzbaSsSPA4ZlTX)

We then cat the flag that we've exfiltrated to the host PC.

![4](https://lh4.googleusercontent.com/US6vRTk8AACM1Q8XC4AiHqmXZPWdIrwzJmN7-66o2o7QWKrQbx2RTsn9qL5KLxcimWMiIyzYstxSk0e1Hs0nKwQr4mk1WNWSwhkBabDI3B2_oaspHbSW50dZm4j0Yv-cfhc60Yxl)
