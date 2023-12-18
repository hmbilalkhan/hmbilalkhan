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
