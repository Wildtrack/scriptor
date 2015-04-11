#Scriptor

This repo contains a ton of digital ocean related scripts.  To use them you need to set your environment variables to include your digital ocean information:

    export DO_API_KEY=xxxxxxxxxxxxxxx
    export DO_CLIENT_ID=xxxxxxxxxxxxxxxxxx

There are three scripts.  One for setting up a canary, one for a proxy and one for a live node.  They are all run in essentially the same way:

	ansible-playbook -i ./hosts/digital_ocean.py create_canary.yml

Just swap out canary for live or proxy.  Additionally there is a chunk of code in main.js that can be used to provision droplets.  There are two constants on lines 3 and 4 that will need to be set with the api key values.
