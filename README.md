# ghost

GHOST ON-CHAIN smartBCH NFT by B_S_Z

![Ghost](img/Ghost512svg.svg)

Image is stored on-chain. However the image is not visible in Metamask app.

Symbol: GHOST

Name: GHOST ON-CHAIN

Contract id:

0xb189E7f125f2D7051a2824Ad3Ae727D620d9459F

This is an experimental NFT.

## Tutorial (this is not the best way to create on-chain NFT image)

Prepare an image in svg format (small size - about 10 kb)

Open [Base64 svg converter](https://base64.guru/converter/encode/image/svg) and upload the image. In the "Output Format" field choose `Data URI--data:content/type;base64`. Encode it.

Copy Base64 output string and paste it to eg. notepad. Save it. You can paste the string to a web browser to see the image.

It should be something like [this](ghostsvgbase64.txt)

Open sample_metadata.json and paste the encoded output string to `"image": "...",`

It should be something like [this](ghostmetadatabase64.json)

_You can try to add base64 encoded audio file to `"animation_url": "",`, but it will be probably too big._

Open [Base64 file converter](https://base64.guru/converter/encode/file), upload and encode the sample_metadata.json. In the "Output Format" field choose `Data URI--data:content/type;base64`. Encode it.

Copy Base64 output string and paste it to eg. notepad. Change `data:@file/json;` to `data:application/json;`. Save it. You can paste the string to a web browser to see the metadata.

It should be something like [this](ghostmetadatabase64.txt). This is the token uri used in on-chain NFT.

Compile and deploy ghost.sol in [Remix](https://remix.ethereum.org). Change token name and symbol.

In "Deploy & and run transactions" section use "mint" option to mint NFT. Use sample_metadata.json base64 encoded string as uri.

You can try it on smartBCH testnet:
```
Network name: Amber
RPC URL: http://35.220.203.194:8545/
Chain ID: 0x2711
Currency Symbol: BCH
```

[Get the code](https://github.com/mazetoken/ghost) and make it better.

[Here](https://github.com/PatrickAlphaC/all-on-chain-generated-nft) is another on-chain NFT example.

Have fun ;-)

------------------------------------------------------------

Powered by

[MAZE token](https://mazetoken.github.io)







