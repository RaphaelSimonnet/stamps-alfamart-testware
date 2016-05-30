## Feature
Voice OTP
***

## Test Basis
<https://icemobile.atlassian.net/browse/LOP-8077>
<https://icemobile.atlassian.net/browse/LOP-8078>
 
<http://3mt81r.axshare.com>
password: 



***
## Test Scenario's Front-End

- category is created if there is a hashtag
for eg: #[Drinks] Coca Cola
- 'others' category appears only when 
    - a BSO does not contain a category. for eg: Coca Cola
    - improper way of creating a #[]. for eg: #[drinks Coca Cola
- BSO with title but with no hashtag category. for eg: #[ ] Coca Cola
- BSO category with too long string.for eg: #[DrinksDrinks DrinksDrinks DrinksDrinks DrinksDrinks DrinksDrinks ] Coca Cola
- BSO empty state
- When a BSO category is created then the BSO list/details page can never be empty
- when BSO category is created in different language other than English.for eg: #[minuman] Coca Cola   (minuman, meaning drinks in Indonisia)
- BSO category hashtag parser
    - hashtag with special character. for eg: #[@#$&**(}]] Coca Cola
    - hashtag like: #[] #[ Coca Cola 
- There No paging for BSO's, All the BSO s are loaded at once 
- Server error - similate using charles
- no internet connection 
    

***
## Notes


***
## Bugs


***


