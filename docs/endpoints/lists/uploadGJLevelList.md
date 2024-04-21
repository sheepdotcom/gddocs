# uploadGJLevelList.php

Uploads a list of levels.

## Parameters

### Required Parameters

**secret** - Wmfd2893gb7

**add** - the rest later

**seed** - 

**seed2** - 

### Optional Parameters

**probably** - something here

## Response

Returns a list of [level objects](/resources/server/level) separated by pipes `|` and sorted by the parameters, a list of objects denoting the authors sorted by increasing player ID (format is `PLAYERID:USERNAME:ACCOUNTID`) which are also separated by pipes `|`, and a list of [song objects](/resources/server/song) sorted by increasing song ID and separated by `~:~`. The indexers for each are `:`, `:` and `~|~` respectively.

## Example

<!-- tabs:start -->

### **curl**

```cmd
curl -H "User-Agent:" http://www.boomlings.com/database/getGJLevelLists.php -X POST -d "secret=Wmfd2893gb7&type=6"
```


**Response**
```py
1:17:2:The Demon Trial:3:Q2FuIHlvdSBiZWF0IGFueXRoaW5nPw==:5:1:49:1187377:50:YunHaSeu14:10:12:7:10:14:2:19:1:51:10565740,3979721,28220417,42584142:28:1687427379:29:0|1:16:2:My New List:3:U2Vjb25kIGxpc3QuIFRlc3RpbmcgdmVyc2lvbnMu:5:4:49:71:50:RobTop:10:11:7:1:14:1:19:1:51:91530036,91427162:28:1687427214:29:1687478036#16:RobTop:71|36314:YunHaSeu14:1187377#1:0:10#f5da5823d94bbe7208dd83a30ff427c7d88fdb99
```

<!-- tabs:end -->
