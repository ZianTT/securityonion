### 2.3.120-20220425 ISO image built on 2022/04/25



### Download and Verify

2.3.120-20220425 ISO image:  
https://download.securityonion.net/file/securityonion/securityonion-2.3.120-20220425.iso

MD5: C99729E452B064C471BEF04532F28556  
SHA1: 60BF07D5347C24568C7B793BFA9792E98479CFBF  
SHA256: CD17D0D7CABE21D45FA45E1CF91C5F24EB9608C79FF88480134E5592AFDD696E 

Signature for ISO image:  
https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.120-20220425.iso.sig

Signing key:  
https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS  

For example, here are the steps you can use on most Linux distributions to download and verify our Security Onion ISO image.

Download and import the signing key:  
```
wget https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS -O - | gpg --import -  
```

Download the signature file for the ISO:  
```
wget https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.120-20220425.iso.sig
```

Download the ISO image:  
```
wget https://download.securityonion.net/file/securityonion/securityonion-2.3.120-20220425.iso
```

Verify the downloaded ISO image using the signature file:  
```
gpg --verify securityonion-2.3.120-20220425.iso.sig securityonion-2.3.120-20220425.iso
```

The output should show "Good signature" and the Primary key fingerprint should match what's shown below:
```
gpg: Signature made Mon 25 Apr 2022 08:20:40 AM EDT using RSA key ID FE507013
gpg: Good signature from "Security Onion Solutions, LLC <info@securityonionsolutions.com>"
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: C804 A93D 36BE 0C73 3EA1  9644 7C10 60B7 FE50 7013
```

Once you've verified the ISO image, you're ready to proceed to our Installation guide:  
https://docs.securityonion.net/en/2.3/installation.html
