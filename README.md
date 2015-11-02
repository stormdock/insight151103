##### Insight UI

A Bitcoin blockchain explorer web application service for [Bitcore Node](https://github.com/bitpay/bitcore-node) using the [Insight API](https://github.com/bitpay/insight-api).

#####
This is my own personal clone of
[Insight]
(https://github.com/bitpay/insight.git).

Follow the instructions
[here]
(https://github.com/stormasm/bitcore-notes/tree/master/mynode-insight)
first prior to trying to develop your own bitcoin blockchain explorer.

Once you have mastered the above instructions and understand
[services]
(https://bitcore.io/guides/service-development)
in the context of the bitpay ecosystem then you are able to understand
the next set of instructions.

This assumes you have a working copy of the **testnet** data synced on your local machine.
In this example the testnet data is located at

```
"datadir": "/miabitcore/testnet/data",
```

but you can place your data anywhere you want.  This one parameter tells the bitcoin
node where to write the blockchain data after each new block is mined.

##### To get a local copy of the blockchain explorer running

So that you can do local development on
[angular.js]
(https://docs.angularjs.org/guide)
in the context of insight, run these commands...

```
npm install
bower install
grunt compile
npm link ./bitcore-node
bitcore start
```

[http://localhost:3001/insight]
(http://localhost:3001/insight)

[http://localhost:3001/insight-api/status]
(http://localhost:3001/insight-api/status)

##### .bowerrc needs to have this in it...

```
{
  "directory": "public/lib"
}
```
