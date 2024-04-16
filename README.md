# MBTI 

## country wise MBTI person

    for ind, trait in enumerate(one_slice):
         print(ind, trait)                               #slice  #mbti         
      columns_to_sum = list(filter(lambda x : x[ind] == trait, types))
         print(columns_to_sum)
      traits_df[trait] = new_df[columns_to_sum].sum(axis=1) * 100

  * 나라별 'i' , 'n', 'f', 'p' 비율
    
  ![image](https://github.com/kim-chanhee/MBTI/assets/116836230/93959541-c497-45a2-b21a-8e4aea0d94f0)

  *  각 특성(trait)에 대한 세계 지도(Choropleth)를 생성하고 반복하여 특성, 특성 이름, 투영 유형을 사용합니다.
    
  ![image](https://github.com/kim-chanhee/MBTI/assets/116836230/b2a32775-c384-45d7-8b4d-fc290edcbce7)


---
## MBTI500


---
## mbti_wordcloud
 
  ※ 데이터 : https://gall.dcinside.com//mgallery/board/lists/?id=enfj
  
  ※ enfj 관련 데이터를 크롤링하여 가장 많이 사용되는 단어들을 wordcloud로 표현하였다. (명사 추출, 단일 단어 제거)
  
  
    for word in list(words.keys()):
      if len(word) == 1 :
          del words[word]       
          continue
          
      if words[word] == 1:
          del words[word]
  
  
  ![image](https://github.com/kim-chanhee/MBTI/assets/116836230/49ed81f1-ce62-4d5b-9afa-7b88325cc38c)
