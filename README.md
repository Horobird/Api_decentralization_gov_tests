# Api_decentralization_gov_tests

________
 [<img src="https://img.shields.io/badge/JavaScript-0000FF?style=flat-square&logo=Javascript&logoColor=FFFF00"/>](https://en.wikipedia.org/wiki/JavaScript) [<img src="https://img.shields.io/badge/Node v19.8.1-7B68EE?style=flat-square&logo=Node .js&logoColor=00FF00"/>](https://nodejs.org/en) 
 [<img src="https://img.shields.io/badge/Postman v10.15.4-00FFFF?style=flat-square&logo=postman&logoColor=FFA500"/>](https://docs.cypress.io/guides/overview/why-cypress)    

   :small_orange_diamond:Api_decentralization_gov_tests is one example of API testing with the Postman tool. The object of testing was the API from [https://decentralization.gov.ua/](https://decentralization.gov.ua/).
   This resource is designed to provide information about the regions of Ukraine and their properties.     
   :small_orange_diamond: There are 4 requests in total in the collection. One of them is negative with an invalid 'url', a separate request for checking cookies and two, testing the parameters of all regions in the response and each separately.      
   - In the request to the list of all regions, in addition to traditional tests, a loop is implemented for checking the parameters of the "areas" array objects. Each loop checks for the existence of a key and whether it matches the type of its value. In fact - duplication of the tv4 library. Due to the loop, 185 tests are obtained in one iteration.     

![image](https://github.com/Horobird/Api_decentralization_gov_tests/assets/28702124/150c9219-f62c-440c-8aa7-4342c805b37e)    
   - In the request to each region separately, the parameters of the area object are already being tested using the "tv4" library with error messages output to the console. The "pre-request" contains a code that provides a random selection of the region during the subsequent iteration of the test.
   - 
![image](https://github.com/Horobird/Api_decentralization_gov_tests/assets/28702124/a785a49e-4b07-455a-ac75-dd1a2067e5e9)
I will be glad not only that this example may be useful to someone, but also grateful if I receive comments and corrections to it.
