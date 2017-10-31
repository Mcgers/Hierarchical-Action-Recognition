# 层次化数据集分类

## 原则：
- 男女项目，以男子项目为准
- 忽略跑步、游泳中的米数，只关注动作
- 考虑团队与个人
- 
```
graph TD
Archery[Archery]
Archery-->Archery1[individual-70m]
Archery-->Archery2[team-70m]
```

--------------------------------------------------
```
graph TD
Athletics[Atheletics]
Athletics-->Athletics1[common run race]
Athletics-->Athletics2[race walk]
Athletics-->Athletics3[steeplechase]
Athletics-->Athletics4[hurdles]
Athletics-->Athletics5[relay]

Athletics-->Athletics6[decathlon]
Athletics-->Athletics7[discus throw]
Athletics-->Athletics8[hammer throw]
Athletics-->Athletics9[high jump]
Athletics-->Athletics10[javelin throw]
Athletics-->Athletics11[long jump]
Athletics-->Athletics12[marathon]
Athletics-->Athletics13[pole vault]
Athletics-->Athletics14[shot put]
Athletics-->Athletics15[triple jump]
```
--------------------------------------------------
```
graph TD
Diving[diving]
Diving-->Diving1[10m platform]
Diving-->Diving2[3m springboard]
Diving-->Diving3[synchronized diving 10m platform]
Diving-->Diving4[synchronized diving 3m springboard]
```
--------------------------------------------------
```
graph TD
Swimming[Swimming]
Swimming-->Swimming1[backstroke]
Swimming-->Swimming2[breaststroke]
Swimming-->Swimming3[butterfly]
Swimming-->Swimming4[freestyle]
Swimming-->Swimming5[individual medley]
Swimming-->Swimming6[freestyle relay]
Swimming-->Swimming7[medley relay]
```
--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------

--------------------------------------------------



## 总图

```
graph TD
Sports[Sports]


Sports-->Archery
Sports-->Diving
Sports-->Swimming
Sports-->Athletics

Archery[Archery]
Archery-->Archery1[individual-70m]
Archery-->Archery2[team-70m]


Athletics[Atheletics]
Athletics-->Athletics1[common run race]
Athletics-->Athletics2[race walk]
Athletics-->Athletics3[steeplechase]
Athletics-->Athletics4[hurdles]
Athletics-->Athletics5[relay]

Athletics-->Athletics6[decathlon]
Athletics-->Athletics7[discus throw]
Athletics-->Athletics8[hammer throw]
Athletics-->Athletics9[high jump]
Athletics-->Athletics10[javelin throw]
Athletics-->Athletics11[long jump]
Athletics-->Athletics12[marathon]
Athletics-->Athletics13[pole vault]
Athletics-->Athletics14[shot put]
Athletics-->Athletics15[triple jump]



Diving[Diving]
Diving-->Diving1[10m platform]
Diving-->Diving2[3m springboard]
Diving-->Diving3[synchronized diving 10m platform]
Diving-->Diving4[synchronized diving 3m springboard]


Swimming[Swimming]
Swimming-->Swimming1[backstroke]
Swimming-->Swimming2[breaststroke]
Swimming-->Swimming3[butterfly]
Swimming-->Swimming4[freestyle]
Swimming-->Swimming5[individual medley]
Swimming-->Swimming6[freestyle relay]
Swimming-->Swimming7[medley relay]
```