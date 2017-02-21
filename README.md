# go-ipfs-box
a personal storage system across devices built on ipfs


## globals

SHARED_DIRECTORY=~/go-ipfs-box/shared/

## description

I wanted to play with go-ipfs, and I have files that I'd like my server at home
to replicate for backup, and to perhaps share them across devices.

This needn't necessarily be on ipfs, but:

1) I want to explore go-ipfs
2) content addressing seems useful
3) IPLD's Merkle DAG could eventually be used for a bunch of versioning /
relational stuff
3) go-ipfs handles transport, syncing, bunch of low level stuff for free

`go-ipfs-box` should be run on each node in what becomes a private ipfs network.
All files in $SHARED_DIRECTORY are automatically pinned by each node.

I'll document functionality as I figure stuff out.
