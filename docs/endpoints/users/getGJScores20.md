# getGJScores20.php

Gets the leaderboard scores.

## Parameters

### Required Parameters

**secret** - Wmfd2893gb7

### Optional Parameters

**gameVersion** - 21

**binaryVersion** - 35

**gdw** - 0

**accountID** - The account ID of the user viewing the leaderboards

**gjp** - The user's [GJP](/topics/gjp.md)

**type** - Can be `top`, `relative`, `friends`, or `creators`. If left out it defaults to `top`

**count** - Returns the amount of players specified

## Response

Returns a list of [user objects](/resources/server/user.md) in order based on which leaderboard you're viewing, separated by pipe `|` characters.

## Example

<!-- tabs:start -->

### **Python**

```py
import requests

data = {
    "secret": "Wmfd2893gb7",
    "type": "top",
	"count": 20
}

req = requests.post('http://boomlings.com/database/getGJScores20.php', data=data)
print(req.text)
```

**Response**
```py
1:xMiguel007:2:2866103:13:149:17:7219:6:1:9:37:10:35:11:3:14:0:15:2:16:70846:3:65710:8:0:46:12879:4:1073|1:shaggy23:2:1995959:13:149:17:4321:6:2:9:51:10:39:11:29:14:0:15:2:16:2888:3:65595:8:21:46:11847:4:1115|1:Michigun:2:703929:13:149:17:12312:6:3:9:22:10:15:11:12:14:0:15:2:16:34499:3:61161:8:16:46:14600:4:997|1:Cool Dash:2:1148292:13:149:17:7026:6:4:9:37:10:20:11:17:14:0:15:2:16:4825:3:52931:8:0:46:14630:4:641|1:Kaernk:2:1282100:13:149:17:11908:6:5:9:51:10:18:11:12:14:0:15:2:16:118843:3:51821:8:0:46:17073:4:533|1:DeathHogz:2:1396933:13:149:17:5250:6:6:9:57:10:37:11:12:14:0:15:2:16:104119:3:51791:8:2:46:11948:4:435|1:Franchet:2:9576358:13:149:17:9840:6:7:9:30:10:15:11:12:14:0:15:2:16:1999478:3:51504:8:0:46:18616:4:670|1:Leksitoo:2:933105:13:149:17:4125:6:8:9:29:10:5:11:12:14:0:15:2:16:205:3:50530:8:14:46:13852:4:666|1:Superchat:2:2945295:13:149:17:5150:6:9:9:98:10:12:11:17:14:0:15:0:16:1098021:3:45706:8:2:46:14101:4:1201|1:Darky84:2:8513170:13:149:17:5864:6:10:9:37:10:12:11:25:14:0:15:2:16:1244088:3:44313:8:0:46:7444:4:1031|1:IvanNyan:2:14999317:13:149:17:5693:6:11:9:35:10:11:11:23:14:1:15:2:16:5148877:3:43785:8:0:46:6:4:563|1:GK NK 98:2:4803050:13:147:17:6491:6:12:9:2:10:12:11:23:14:6:15:2:16:890741:3:43163:8:2:46:14155:4:586|1:BonnieABoss:2:18158058:13:149:17:5572:6:13:9:105:10:15:11:3:14:0:15:2:16:5810059:3:43099:8:0:46:4743:4:778|1:FixTop100:2:18119007:13:149:17:801:6:14:9:1:10:0:11:3:14:0:15:0:16:5316700:3:43099:8:0:46:3559:4:323|1:TheRealAir:2:9035779:13:149:17:1270:6:15:9:35:10:12:11:25:14:0:15:2:16:2382846:3:42096:8:0:46:12808:4:665|1:XShadowWizardX:2:10670782:13:149:17:6097:6:16:9:85:10:12:11:7:14:0:15:2:16:1919857:3:41209:8:6:46:14083:4:540|1:CleanTop100:2:6552455:13:149:17:7111:6:17:9:30:10:7:11:12:14:0:15:2:16:2835706:3:40810:8:0:46:13243:4:871|1:xSuwako:2:14287615:13:149:17:2778:6:18:9:96:10:37:11:12:14:0:15:2:16:3984642:3:40695:8:0:46:11827:4:878|1:Civitrex2:2:14674984:13:149:17:7418:6:19:9:37:10:12:11:13:14:0:15:2:16:4156730:3:40576:8:0:46:13981:4:922|1:AdrianDlaCruz:2:16219796:13:148:17:2689:6:20:9:103:10:12:11:40:14:0:15:2:16:4771465:3:40286:8:0:46:4489:4:982|
```

<!-- tabs:end -->