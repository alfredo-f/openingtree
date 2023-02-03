# Openingtree
Code for [openingtree.com](https://www.openingtree.com). It downloads chess games in form of a pgn from any source, applies specified filters and constructs an openingtree. 
The tree is visualized on a chessboard. It also shows win percentages and other statistics with different moves

## Architecture diagram
This does not correlate one to one with the code modules but the interactions at a high level are depicted accurately.

![GitHub Logo](/docs/images/architecture.png)

## Run locally

Can't use PyCharm magic because yarn commands need

```
--network-timeout 100000
```

For Powershell, you need to set SSL as per
https://stackoverflow.com/questions/69692842/error-message-error0308010cdigital-envelope-routinesunsupported

```
$env:NODE_OPTIONS="--openssl-legacy-provider"
```

```
yarn
yarn start
```
starts a server on port `3000`

## Build for production
```
yarn build
```


