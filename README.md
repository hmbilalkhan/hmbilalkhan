#include <iostream>
using namespace std;
int main()
{   int returnTotalBill(void);
   int totalbill=returnTotalBill();
   cout<<" Your total bill is "<<totalbill<<"!"<< endl;
   cout<<" Thanks for ordering food from our restaurant :)"<<endl;
}
int returnTotalBill()
{   char c;
    char items;
    char vegItems;
    char NonVeg;
    char SelectAgain;
    int billAmount=0;

    cout<<" --------------Welcome to Avengers restaurant---------------- "<<endl;
    cout<<"---------------Please follow the instructions---------------- "<<endl;
    cout<<" Step 1 : Please press s to start your order "<<endl;
    cout<<" Step 2 : You can order both Veg and nonVeg as per your wish "<<endl;
    cout<<" step 3 : Please press a to order veg items from the menu :) "<<endl;
    cout<<" step 4 : Please press b to order nonVeg items from the menu :) "<<endl;
    cout<<" you will get the your final bill after complete order "<<endl;
    start:
    cin>>c;
