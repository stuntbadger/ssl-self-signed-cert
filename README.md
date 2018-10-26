# ssl-self-signed-cert
creating a self signed SSL Certificate

edit the options.conf file to add all of the domains names you want to include in the certificate
edit the certificate-authority-options.conf if you want to tweek the settings used to generate the certifcate authority certifcate ( optional) 
run sudo ./generate-ssl.sh local.dev where local.dev is the name of the cert that will be genrated
The script will ask you for your system password which it needs to add the root certificate to Keychain
The next prompts for passwords will be just for the generation of the certs. It doesn't matter what your password is so long as you enter the same one every time it asks
That's it! Your certificate and private key will be in the your-certs/ directory. Do with them what you like.

Requirement of openssl to be installed for this to work. 
