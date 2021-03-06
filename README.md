# data_analytics_hw2

Dataset : https://www.kaggle.com/jiashenliu/515k-hotel-reviews-data-in-europe

## 問題:
 - 由一則對於某間旅館的評論來判斷此飯店是否值得推薦
 - 評論不可信也視為不推薦

## 特徵:
 - 旅館平均分數
 - 評論內負面字詞數
 - 評論內正面字詞數
 - 旅館評論總數
 - 評分
 - 旅客評論數

## 限制:(初始皆為推薦)
  - 負面字詞數>300 不推薦
  - 正面字詞數<20 不推薦
  - 負面字詞數+正面字詞數<50 不推薦
  - 負面字詞數/正面字詞數>2 不推薦
  - 旅客評論數<2 不推薦
  - 旅館平均分數<3
  - 評分>9.5 不推薦
  - 評分<1 不推薦
  - |旅館平均分數-評分|>7 不推薦
  - 旅館評論總數<300 不推薦

## 結論:
  - 因為他是用已知的data去推算規則，所以通常無法回推到準確的規則
  - 一條簡單的規則，在tree裡面通常使用一個以上的node來實現
  - 如果增加預設的規則，有機會使準確率提升，因為在建tree時使用的二分法有更多明確的案例可以遵循
  - 如果增加tree的高度，通常會使準確率提高，因為可以把判斷流程分成更多node，而每個node都代表一個判斷
  
