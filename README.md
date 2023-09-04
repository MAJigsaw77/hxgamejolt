# hxgamejolt-api

![](https://img.shields.io/github/repo-size/MAJigsaw77/hxgamejolt) ![](https://badgen.net/github/open-issues/MAJigsaw77/hxgamejolt) ![](https://badgen.net/badge/license/MIT/green)

Haxe bindings for [GameJolt API](https://gamejolt.com/game-api)

### Installation

You can install it through `Haxelib`
```bash
haxelib install hxgamejolt-api
```
Or through `Git`, if you want the latest updates
```bash
haxelib git hxgamejolt-api https://github.com/MAJigsaw77/hxgamejolt-api.git
```

### Basic Usage Example

```haxe
import hxgamejolt.GameJolt as GJClient; // be sure you import this.

GJClient.init('game id', 'private key');

GJClient.authUser('user name', 'user token', function(json:Dynamic) // on Succeed
{
	// your code
}, function(message:String) // on Failure
{
	// your code
});

GJClient.fetchUser('user name', [], function(json:Dynamic) // on Succeed
{
	// your code
}, function(message:String) // on Failure
{
	// your code
});
```

### Licensing

**hxgamejolt-api** is made available under the **MIT License**. Check [LICENSE](./LICENSE) for more information.

