#include <iostream>
using namespace std;




int returnTotalBill()
{   char c;
    char items;
    int vegItems;
    int NonVeg;
    char SelectAgain;
    int billAmount=0;


    cout<<" --------------Welcome to Avengers restaurant---------------- "<<endl;
    cout<<"---------------Please follow the instructions---------------- \n"<<endl;
    cout<<" Step 1 : Please press s to start your order !\n"<<endl;
    cout<<" Step 2 : You can order both Veg and nonVeg as per your wish :)\n"<<endl;
    cout<<" step 3 : Please press a to order veg items from the menu :)\n "<<endl;
    cout<<" step 4 : Please press b to order nonVeg items from the menu :)\n "<<endl;
    cout<<"Note : you will get the your final bill after complete order !\n"<<endl;
    cout<<" Enter option : ";
    start:
    cin>>c;


    if(c=='s' || c=='S'){
        items:

       cout<<" Please enter your choice "<<endl;
       cout<<" (a): Veg items            (b):NonVeg items "<<endl<<" Enter option : ";

       cin>>items;
if(items=='a'|| items=='A'){
        vegitemsList:   


        cout<<" Please select 1 , 2 , 3 , 4 , 5, 6, 7, 8,as per your choice "<<endl;
        cout<<" (1) : mix veg     ::::::  price : Rs = 150 \n "<<endl;
        cout<<" (2) : veg roll    ::::::  price : Rs = 200 \n"<<endl;
        cout<<" (3) : Veg rice    ::::::  price : Rs = 170 \n"<<endl;
        cout<<" (4) : Veg macroni ::::::  price : Rs = 210 \n"<<endl;
        cout<<" (5) : Veg cutlus  ::::::  price : Rs = 120 \n"<<endl;
        cout<<" (6) : lobia       ::::::  price : Rs = 80  \n"<<endl;
        cout<<" (7) : Daal        ::::::  price : Rs = 70  \n"<<endl;
        cout<<" (8) : Aloo bangan ::::::  price : Rs = 100 \n"<<endl;
        
        cin>>vegItems;


        if(vegItems==1){
            billAmount=billAmount+150;

        }else if(vegItems==2){
            billAmount=billAmount+200;
        }else if(vegItems==3){
            billAmount=billAmount+170;

        }else if(vegItems==4){
            billAmount=billAmount+210;
        }else if(vegItems==5){
            billAmount=billAmount+120;
        }else if(vegItems==6){
            billAmount=billAmount+80;
        }else if(vegItems==7){
            billAmount=billAmount+70;
        }else if(vegItems==8){
            billAmount=billAmount+100;
        }else{
            cout<<" you have entered wrong value , please try again :) "<<endl;
            goto vegitemsList;


        }cout<<" Do you want to add more items : y or no ? "<<endl;
        cin>>SelectAgain;
        if(SelectAgain=='y' || SelectAgain == 'Y'){
            goto items;

        }else{
            return billAmount;
        }

       }
       
       }else if(items=='b'||items=='B'){

        NonvegitemsList: 


          cout<<" Please select 1 , 2 , 3 , 4 , 5, 6 ,7 ,8 as per your choice \n"<<endl;
        cout<<" (1) : Chicken tikka   ::::::   price : Rs = 250 \n"<<endl;
        cout<<" (2) : Chicken biryani ::::::   price : Rs = 200 \n"<<endl;
        cout<<" (3) : BBQ Pizza       ::::::   price : Rs = 700 \n"<<endl;
        cout<<" (4) : Dry Chili       ::::::   price : Rs = 450 \n"<<endl;
        cout<<" (5) : Beef boti       ::::::   price : Rs = 350 \n"<<endl;
        cout<<" (6) : Burger          ::::::   price : Rs = 500 \n"<<endl;
        cout<<" (7) : Dumba karahi    ::::::   price : Rs = 2500 \n"<<endl;
        cout<<" (8) : Grill Fish      ::::::   price : Rs = 1500\n"<<endl;
        

        cin>>NonVeg;
        
        if(NonVeg==1){
            billAmount=billAmount+250;

        }else if(NonVeg==2){
            billAmount=billAmount+200;

        }else if(NonVeg==3){
            billAmount=billAmount+700;

        }else if(NonVeg==4){
            billAmount=billAmount+450;

        }else if(NonVeg==5){
            billAmount=billAmount+350;

        }else if(NonVeg==6){
            billAmount=billAmount+500;

        }else if(NonVeg==7){
            billAmount=billAmount+2500;

        }else if(NonVeg==8){
            billAmount=billAmount+1500;

        }else{
            cout<<" you have entered wrong value , please try again :) "<<endl;
            goto NonvegitemsList;


        }cout<<" Do you want to add more items : y or no ? "<<endl;
        cin>>SelectAgain;

        if(SelectAgain=='y'){
            goto items;
        }else{
            return billAmount;
        }
        } if(items=='c'||items=='C'){

       Drinkslist: 


          cout<<" Please select 1 , 2 , 3 , 4 , 5, 6 ,7 ,8 as per your choice \n"<<endl;
        cout<<" (1) :  Kashmiri Chai   ::::::   price : Rs = 130 \n"<<endl;
        cout<<" (2) :  Oreo shake      ::::::   price : Rs = 220 \n"<<endl;
        cout<<" (3) :  Pepsi           ::::::   price : Rs = 140 \n"<<endl;
        cout<<" (4) : Orange juice     ::::::   price : Rs = 200 \n"<<endl;
        cout<<" (5) : Lemon green tea  ::::::   price : Rs = 130 \n"<<endl;
        cout<<" (6) :  Mint Margarita  ::::::   price : Rs = 270 \n"<<endl;
        cout<<" (7) : dhoodh pati chai ::::::   price : Rs = 120 \n"<<endl;
        cout<<" (8) : coffee           ::::::   price : Rs = 140\n"<<endl;
        

        cin>>drinks;
        
        if(drinks==1){
            billAmount=billAmount+130;

        }else if(drinks==2){
            billAmount=billAmount+220;

        }else if(drinks==3){
            billAmount=billAmount+140;

        }else if(drinks==4){
            billAmount=billAmount+200;

        }else if(drinks==5){
            billAmount=billAmount+130;

        }else if(drinks==6){
            billAmount=billAmount+270;

        }else if(drinks==7){
            billAmount=billAmount+120;

        }else if(drinks==8){
            billAmount=billAmount+140;

        }else{
            cout<<" you have entered wrong value , please try again :) "<<endl;
            goto Drinkslist;


        }cout<<" Do you want to add more items : y or no ? "<<endl;
        cin>>SelectAgain;

        if(SelectAgain=='y'){
            goto items;
        }else{
            return billAmount;
        }
        }if(items=='d'||items=='D'){

       RotiList: 


          cout<<" Please select 1 , 2 , 3 , 4 , 5, 6 ,7 ,8 as per your choice \n"<<endl;
        cout<<" (1) :  Chapati       ::::::   price : Rs = 20 \n"<<endl;
        cout<<" (2) :  Naam          ::::::   price : Rs = 25 \n"<<endl;
        cout<<" (3) :  Puri paratha  ::::::   price : Rs = 100 \n"<<endl;
        cout<<" (4) : Garlic naam    ::::::   price : Rs = 120 \n"<<endl;
        cout<<" (5) : Kulcha         ::::::   price : Rs = 70 \n"<<endl;
        cout<<" (6) :  Makhni Naan   ::::::   price : Rs = 130 \n"<<endl;
        cout<<" (7) : Sada paratha   ::::::   price : Rs = 60 \n"<<endl;
        cout<<" (8) :Tandoori Naan   ::::::   price : Rs = 40\n"<<endl;
        

        cin>>roti;
        
        if(roti==1){
            billAmount=billAmount+20;

        }else if(roti==2){
            billAmount=billAmount+25;

        }else if(roti==3){
            billAmount=billAmount+100;

        }else if(roti==4){
            billAmount=billAmount+120;

        }else if(roti==5){
            billAmount=billAmount+70;

        }else if(roti==6){
            billAmount=billAmount+130;

        }else if(roti==7){
            billAmount=billAmount+60;

        }else if(roti==8){
            billAmount=billAmount+40;

        }else{
            cout<<" you have entered wrong value , please try again :) "<<endl;
            goto RotiList;


        }cout<<" Do you want to add more items : y or no ? "<<endl;
        cin>>SelectAgain;

        if(SelectAgain=='y'){
            goto items;
        }else{
            return billAmount;
        }
        }if(items=='e'||items=='E'){

       DessertsList:


          cout<<" Please select 1 , 2 , 3 , 4 , 5, 6 ,7 ,8 as per your choice \n"<<endl;
        cout<<" (1) :  Chocolate lava cake ::::::   price : Rs = 400 \n"<<endl;
        cout<<" (2) :  Ras Malai           ::::::   price : Rs = 300 \n"<<endl;
        cout<<" (3) :  Blueberry Ice cream ::::::   price : Rs = 270 \n"<<endl;
        cout<<" (4) :  Falooda             ::::::   price : Rs = 330 \n"<<endl;
        cout<<" (5) :  Kheer               ::::::   price : Rs = 170 \n"<<endl;
        cout<<" (6) :  Brownie             ::::::   price : Rs = 280 \n"<<endl;
        cout<<" (7) :  3 milk cake         ::::::   price : Rs = 650 \n"<<endl;
        cout<<" (8) :  Strawberry icecream ::::::   price : Rs = 520 \n"<<endl;
        

        cin>>desserts;
        
        if(desserts==1){
            billAmount=billAmount+400;

        }else if(desserts==2){
            billAmount=billAmount+300;

        }else if(desserts==3){
            billAmount=billAmount+270;

        }else if(desserts==4){
            billAmount=billAmount+330;

        }else if(desserts==5){
            billAmount=billAmount+170;

        }else if(desserts==6){
            billAmount=billAmount+280;

        }else if(desserts==7){
            billAmount=billAmount+650;

        }else if(desserts==8){
            billAmount=billAmount+520;

        }else{
            cout<<" you have entered wrong value , please try again :) "<<endl;
            goto DessertsList;


        }cout<<" Do you want to add more items : y or no ? "<<endl;
        cin>>SelectAgain;

        if(SelectAgain=='y'){
            goto items;
        }else{
            return billAmount;
        }
        

       }else 
       cout<<" you have entered the wrong value , please try again :) "<<endl;
       goto items;



    }else{
    cout<<" you have entered wrong character, please enter s! "<<endl;
    goto start;

    }return billAmount;
}


int main()
{  
    int returnTotalBill();
    int totalbill=returnTotalBill();

    cout<<" Your total bill is "<<totalbill<<"! \n"<< endl;
    cout<<" * * * * * * * * * * * * * * * * * * \n"<<endl;
    cout<<" Thanks for ordering food from our restaurant :)\n"<<endl;
    cout<<" * * * * * * * * * * * * * * * * * * ";
}
