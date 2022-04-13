# 추천 시스템(Recommendation System)
### Recommendation system development using various methods and approaches

> 다양한 추천 시스템 방법론을 사용해 구현해보고 있습니다.

---
<p align="center">
<img src="https://user-images.githubusercontent.com/38115693/163110519-467e50c6-aa4b-4c8b-9ffc-2549282e60a5.png" width="70%" height="">
</p>

**1. 영화 추천 시스템 - 콘텐츠 기반 필터링(Content-based Filtering)**
- TMDB 5000 Movie Dataset (https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- Count Vectorizer를 사용해 장르 속성을 기반으로 각 아이템 간의 콘텐츠에 대해 유사도를 계산하고, 이를 기반으로 추천

**2. 영화 추천 시스템 - 아이템 기반(Item-based) 최근접 이웃(Nearest Neighbor) 협업 필터링(Collaborative Filtering)**
- MovieLens Latest Datasets (https://grouplens.org/datasets/movielens/latest/)
- 영화의 평점을 매긴 사용자와 평점 행렬 등의 데이터이며, 이 중 1MB짜리 small 데이터 사용
- '이 상품을 선택한 다른 고객들은 다음 상품도 구매했음'을 기반으로 추천
  - 사용자들이 어떤 아이템을 좋아하는지/싫어하는지 평가한 척도가 유사한 아이템을 추천
  - 즉, 각 아이템에 대해 사람들이 비슷하게 평가한 정도가 유사도가 되어 그에 기반한 추천

**3. 책 추천 시스템 - 콘텐츠 기반 필터링(Content-based Filtering)**
- Good Books Dataset (https://www.kaggle.com/zygmunt/goodbooks-10k)
- ratings, books, tag, book_tags, to_read의 10k(10,000) 데이터
- Tfidf Vectorizer를 사용해 authors, tag_name, 그리고 authors+tag_name을 합친 것을 기반으로 유사한 책 추천

---
## To-do
- 잠재 요인 협업 필터링(Latent Factor Collaborative Filtering)
  - Surprise 사용
- Doc2Vec
- 딥러닝
