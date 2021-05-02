# Resume Project 
In this repository I have a collection of my experience and projects. 

##Introduction 

Project Name: StockApp 


Stroy: 1 BASE HTML (#Base-html)
  
  
![Base_Commented](https://user-images.githubusercontent.com/63297077/116815203-bab6b400-ab19-11eb-8885-030d30c35a68.PNG)

  This is the base HTML that get extended to all other html files in the templates folder. Doing HTML again after a while took a second to get back into the swing of it. But it was also great because of its simplicity compared to other languages I've learned in the meantime. The link is repeated twice because I was having issues with the first one not working when going into the details. So, I added the other method to link to the CSS sheet. I also opted to include the NavBar in the StockApp_base.html however in hindsight I would have put it into its own html document and had a link in the base so it would extend with the base but also be easier to adjust and style. 
  
  

Story: 2 Model 
  
 ![MODEL_COMMENTED](https://user-images.githubusercontent.com/63297077/116815905-0028b080-ab1d-11eb-8937-68e769efd51c.PNG)
 The Model was one of the easier sections of this project. I was familiar with the needed import and the different fields that could be used. The part that took the longest funny enough was deciding what variables I wanted to track. Name was a given, Market Cap could be useful for sorting later, Time Stamp because the data is time sensitive and old data isn't very actionable, and price was essential. 
  
  
Story: 3 URLS  
 
  
    from django.urls import path
    from . import views

    urlpatterns = [

    path('', views.home, name='StockApp_home'),
    path('StockApp_base/', views.base, name='StockApp_base'),
    path('StockApp_newstock/', views.new, name='StockApp_newstock'),
    path('StockApp_Watchlist/', views.watchlist, name='StockApp_Watchlist'),
    path('<int:pk>/StockApp_Details/', views.details, name='StockApp_Details'),
    path('<int:pk>/StockApp_confirm/', views.confirm, name="StockApp_confirm"),
    path('<int:pk>/StockApp_edit/', views.edit, name='StockApp_edit'),

    ]

  urls.py is straight forward I had some delays with passing in the pk as int syntax. Had to double check the info needed in the views and the info I sent through the html page. 

  
  
Story: 4 WATCHLIST HTML AND FUNCTION 
  
  StockApp Watchlist displays all the objects (stocks) in the database using a for loop. Every item gets its own box with all the data fields in the Model displayed. 
  
 ![Stock_App_Commented](https://user-images.githubusercontent.com/63297077/116819354-045cca00-ab2d-11eb-948f-5c20c6809966.PNG)
  
  The display function is straight forward. Upon request for function watchlist it will send in the information from the database. 
  ![Top of functions no comments](https://user-images.githubusercontent.com/63297077/116819533-a8df0c00-ab2d-11eb-9009-86e4d838806c.PNG)

  
Story: 5 DELETE AND EDIT 
  
  The delete and edit function was a challenge I was having problems with the request method was GET only and couldn't get it to send as a post. So, I removed the else statement from my confirm preventing it from just trying to send the user to a different page, preventing the if statement from initiating. I got some assistance from an instructor and reformatted my function removing some redundant code that linked 1 variable to another name. 
  
 ![FUNCTIONS PIC](https://user-images.githubusercontent.com/63297077/116820049-44717c00-ab30-11eb-8cee-077c44bec022.PNG)

CONCLUSION AND THINGS TO IMPOROVE AND RESEARCH *cough *cough CSS 

## Jump To: [Base HTML](#Base-html)

## Other Skills Learned 
*
*
*
*
*
