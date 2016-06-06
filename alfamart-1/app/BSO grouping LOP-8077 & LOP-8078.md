## Feature
BSO parsing and grouping
***

## Test Basis
<https://icemobile.atlassian.net/browse/LOP-8077>
<https://icemobile.atlassian.net/browse/LOP-8078>
 
<http://3mt81r.axshare.com>
password: 



***
## Test Scenario's Front-End


- BSO empty state
- When a BSO category is created then the BSO list/details page can never be empty
- BSO category hashtag parser
    - hashtag category. for eg: #[Drinks] Coca Cola
    - hashtag category starts with white spaces. for eg: #[  Drinks] Coca Cola 
    - hashtag category with 2 words. for eg: #[Soft Drinks] Coca Cola 
    - hashtag category with hypenated 2 words. for eg: #[Soft-Drinks] Coca Cola 
    - hashtag category ends with brackets. for eg: #[  Drinks]] Coca Cola 
    - hashtag category starts with brackets. for eg: #[[Drinks] Coca Cola 
    - hashtag category extra with hashtag. for eg: ##[Drinks] Coca Cola 
    - hashtag category extra with hashtag separated with white space. for eg: # #[Drinks] Coca Cola 
    - hashtag category too long . for eg:  eg: #[DrinksDrinks DrinksDrinks DrinksDrinks DrinksDrinks DrinksDrinks ] Coca Cola (TBD : max of 3 lines is displayed in app ????)
    - Empty hashtag category. for eg: #[ ] Coca Cola
    - hashtag category with special character. for eg: #[@#$&**(}] Coca Cola
    - hashtag category with unicode character. for eg: #[⌧ϔڅྵϢ] Coca Cola
    - hashtag category with 2 hashtags : #[] #[ Coca Cola 
    - hashtag category is created in different language other than English.for eg: #[minuman] Coca Cola   (minuman, meaning drinks in Indonisia)
- 'others' category appears only when 
    - a BSO does not contain a category. for eg: Coca Cola
    - improper way of creating a #[]. for eg: #[drinks Coca Cola
- There No paging for BSO's, All the BSO s are loaded at once 
- Server error - simulate using charles
- no internet connection 
- hashtag category is updated
- BSO title under a BSO hashtag category is updated


***
## Notes


***
## Bugs


***


