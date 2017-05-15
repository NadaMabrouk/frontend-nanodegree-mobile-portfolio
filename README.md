## Website Performance Optimization portfolio project
In this project, there was a website that was full of Jank and was performing in more than 60 fps. And here is the [Un-Optimized Version of the Project](https://github.com/udacity/frontend-nanodegree-mobile-portfolio).

### Steps did to Optimize the Project
1. Minimized number of critical resources.
* Inlined CSS that was included in the external document style.css *This was done too to stop render blocking*
* Inlined JavaScript that was included in the external document perfmatters.js
* Minified both the CSS and Javascript before inlining.
2. Used *async* in the inlined Javascript used and in the script of analytics.js to stop parser blocking.
3. Minimized size of the Pictures used and resized the pizzeria.jpg and used it in the index.html document.
4. Used media tag in the call of the print.css file
5. Minified the bootstrap-grid.css 
### Javascript Optimization
1. Deleted the detemineDX function in main.js document and did its work inside changePizzaSizes function to get rid of the Forced Synchronous Layout.
2. Changed the logic of the UpdatePositions function to do all the Layout work first and then the styling work. 
3. Used requestAnimationFrame to call UpdatePositions function inside the eventlistener.

### PageSpeedInsight was used to check the Website speed And the results attached:

URL:       nadamabrouk.github.io/frontend-nanodegree-mobile-portfolio

Strategy:  mobile

Speed:     95

Usability: 100


|CSS size                                   | 1.09 kB|
:------------------------------------------:|-------:|
HTML size                                  | 4.87 kB
Image size                                 | 24.9 kB
JavaScript size                            | 30.3 kB
CSS resources                              | 1
Hosts                                      | 5
JS resources                               | 1
Resources                                  | 9
Static resources                           | 7
Total size of request bytes sent           | 1.23 kB
Leverage browser caching                   | 2.88
Optimize images                            | 0.71

------------------------------------------------------------------------------------------------------------
URL:       nadamabrouk.github.io/frontend-nanodegree-mobile-portfolio

Strategy:  desktop

Speed:     97


|CSS size                                   | 1.09 kB|
|:-----------------------------------------:|-------:|
HTML size                                  | 4.87 kB
Image size                                 | 24.9 kB
JavaScript size                            | 30.3 kB
CSS resources                              | 1
Hosts                                      | 5
JS resources                               | 1
Resources                                  | 9
Static resources                           | 7
Total size of request bytes sent           | 1.23 kB
Leverage browser caching                   | 1.92
Optimize images                            | 0.71
------------------------------------------------------

# [Link to my Optimized Version](https://nadamabrouk.github.io/frontend-nanodegree-mobile-portfolio/)






