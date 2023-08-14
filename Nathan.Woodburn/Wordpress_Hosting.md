# Wordpress Hosting

## Introduction
This project is to allow easy hosting of Wordpress websites on Handshake domains.  
It is likely to be a paid service (due to compute resources required), but the installation scripts will be available for free to allow anyone to host their own Wordpress server.  

## Features
- Easy setup scripts to allow easy expansion of the service  
One line command to install all the required software (Docker and nginx)

- Full admin control of the Wordpress server for the domain owner.

- Easy to assign wordpress servers  
  Probably via a discord bot with a license key to allow creation of the server.  
  API to create a license key when the user pays for the service. (optionally via ADMIN discord command)

- Full SSL support to allow secure connections to the Wordpress server


## Estimated project timeline
1. Finalise the Wordpress server setup script to remove any bugs that may be present.
2. Create a script that takes in a license key and domain and will create a Wordpress server for that domain if the license key is valid.
3. Update the HNSHosting discord bot to allow Wordpress hosting.
4. Test the Wordpress hosting system with a few users (by giving a few licenses away for free).
5. Verify that the system is working correctly and fix any bugs that may be present.
6. Release the Wordpress hosting system to the public.
7. Finalise the Wordpress hosting system and release the scripts to allow anyone to host their own Wordpress server. (This script will take in a Discord Bot token and set everything up for you on a new linux VPS)