
# 데이터베이스 연습

### 지마켓 베스트 아이템 종목들을 카테고리별로 데이터베이스에 저장
### Schema

#### items
|Field|Type|Null|Key|Default|Extra| 
|:---|:---|:---|:---|:---|:---|
|item_code|varchar(20)|NO|PRI|NULL||  
|title|varchar(200)|NO||NULL||
|ori_price|int|NO||NULL||
|dis_price|int|NO||NULL||
|dis_percent|int|NO||NULL||
|provider|varchar(100)|YES||NULL|

#### ranking
|Field|Type|Null|Key|Deafault|Extra|
|:---|:---|:---|:---|:---|:---|
|num|int|NO|PRI|NULL|auto_increment|
|main_category|varchar(50)|NO||NULL||
|sub_category|varchar(50)|NO||NULL||
|item_ranking|tinyint unsigned|NO||NULL||
|item_code|varchar(20)|NO|MUL|NULL||
