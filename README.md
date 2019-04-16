# data_analytics_hw2

## 問題:由一則對於某間旅館的評論來判斷此飯店是否值得推薦(評論不可信也視為不推薦)

## 特徵:旅館平均分數、評論內負面字詞數、評論內正面字詞數、用戶評論總數、評分

## 限制:(初始皆為推薦)

- 負面字詞數>80 不推薦
- 正面字詞數<100 不推薦
- 負面字詞數/正面字詞數>2 不推薦
- 用戶評論總數<2 不推薦
- 旅館平均分數<4.5
- 評分>8 不推薦
- 評分<2 不推薦
- |旅館平均分數-評分|>4 不推薦
