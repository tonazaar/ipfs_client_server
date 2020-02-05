A) Set IPFS_PATH=/home/rameshbn/ramipfs

B) Run jsipfs daemon

C) Provide permission
```
ipfs config Addresses.API /ip4/0.0.0.0/tcp/5001
ipfs config Addresses.Gateway /ip4/0.0.0.0/tcp/9001
You may also need to set CORS:
ipfs config --json API.HTTPHeaders.Access-Control-Allow-Origin '["*"]'
```

4) In one terminal
```
node command.js
[ { path: 'tmp/myfile.txt',
hash: 'QmNz1UBzpdd4HfZ3qir3aPiRdX5a93XwTuDNyXRc6PKhWW',
size: 11 },
{ path: 'tmp',
hash: 'QmWXdjNC362aPDtwHPUE9o2VMqPeNeCQuTBTv1NsKtwypg',
size: 67 } ]

```

5)  In another terminal
```
node measure.js
{"numObjects":"20","repoSize":"41357","repoPath":"/home/rameshbn/ramipfs","version":"7","storageMax":"9007199254740991"}


```
