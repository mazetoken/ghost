# ghost

GHOST ON-CHAIN smartBCH NFT by B_S_Z

![Ghost](img/Ghost512svg.svg)

NFT image and metadata are stored on-chain.

Symbol: GHOST

Name: GHOST ON-CHAIN

Contract id:

0xb189E7f125f2D7051a2824Ad3Ae727D620d9459F

[GHOST transaction](https://www.smartscan.cash/transaction/0x908c97e9b7fad303365af4b776989c84b61fb01a98a45be567dc882433281fdf) on smartBCH mainnet.

This is an experimental NFT.

## Tutorial (this is not the best way to create on-chain NFT image)

Prepare a small image in png format.

Open [Base64 svg converter](https://base64.guru/converter/encode/image/png) and upload the image. In the "Output Format" field choose `Data URI--data:content/type;base64`. Encode it.

Copy Base64 output string and paste it to eg. notepad. Save it. You can paste the string to a web browser to see the image.

It should be something like [this](ghostsvgbase64.txt). Example is in svg format, however svg images are not displayed in the MetaMask wallet app.

Open sample_metadata.json and paste the encoded output string to `"image": "...",`

It should be something like [this](ghostmetadatabase64.json)

_You can try to add base64 encoded audio file to `"animation_url": "",`, but it will be probably too big._

Open [Base64 file converter](https://base64.guru/converter/encode/file), upload and encode the sample_metadata.json. In the "Output Format" field choose `Data URI--data:content/type;base64`. Encode it.

Copy Base64 output string and paste it to eg. notepad. Change `data:@file/json;` to `data:application/json;`. Save it. You can paste the string to a web browser to see the metadata.

It should be something like [this](ghostmetadatabase64.txt). This is the token uri used in on-chain NFT.

Open ghost.sol in [Remix](https://remix.ethereum.org). Change token name and symbol. Compile it and deploy.

In "Deploy & and run transactions" section use "mint" option to mint NFT. Use your sample_metadata.json base64 encoded string as uri.

You can try it on smartBCH Amber testnet:

[Get the code](https://github.com/mazetoken/ghost) and make it better.

[Here](https://github.com/PatrickAlphaC/all-on-chain-generated-nft) is another on-chain NFT example.

Have fun ;-)

------------------------------------------------------------

Powered by

[MAZE token](https://mazetoken.github.io)

![MAZE](maze200.png)

[Telegram](https://t.me/mazetokens)







