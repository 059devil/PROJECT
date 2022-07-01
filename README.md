# PROJECT
RELATED TO HOTEL MANAGEMENT SYSTEM
/
#include <iostream>
using namespace std;


int main()
{
int quantites;
  int choice;
  int  Qrooms=0,Qpasta=0,Qburger=0,Qnoodles=0,Qshake=0,Qchicken=0;
  int  Srooms=0,Spasta=0,Sburger=0,Snoodles=0,Sshake=0,Schicken=0;
  int Total_rooms=0,Total_pasta=0,Total_burger=0,Total_noodles=0,Total_shake=0,Total_chicken=0;
  cout<<"\n\tQuantity of items we have";
  cout<<"\n Rooms avaliable:";
  cin>>Qrooms;
  cout<<"\n Quantity of pasta:";
  cin>>Qpasta;
  cout<<"\n Quantity of burger:";
  cin>>Qburger;
  cout<<"\n Quantity of noodles:";
  cin>>Qnoodles;
  cout<<"\n Quantity of shake:";
  cin>>Qshake;
  cout<<"\n Quantity of chicken:";
  cin>>Qchicken;

  m:
  cout<<"\n\t\t\t please select from the menu option";
  cout<<"\n\n1) rooms";
  cout<<"\n2) pasta";
  cout<<"\n2) burger";
  cout<<"\n4) noodles";
  cout<<"\n5) shake";
  cout<<"\n6) chicken";
  cout<<"\n7) information regarding sales and collection";
  cout<<"\n2) please exit if your wise";


  cout<<"\n\n please enter your choice !!";
  cin>>choice;


  switch(choice)
  { 
    case 1:
      cout<<"\n\n enter the number of rooms you want from this hotel ::";
       cin>>quantites;
    if(Qrooms-Srooms>=quantites)
    {
      Srooms=Srooms+quantites;
      Total_rooms=Total_rooms+quantites*1200;
      cout<<"\n\n\t\t"<<quantites<<"rooms have been alloted to you";
    }
    else
    {
      cout<<"\n\t only"<<Qrooms-Srooms<<"rooms remaining in hotel ";
      break;
    }
    case 2:
      cout<<"\n\n enter the number of pasta you want from this hotel ::";
       cin>>Qpasta;
    if(Qpasta-Spasta>=quantites)
    {
      Spasta=Spasta+quantites;
      Total_pasta=Total_pasta+quantites*120;
      cout<<"\n\n\t\t"<<quantites<<"pasta have been ordered to you";
    }
    else
    {
      cout<<"\n\t only"<<Qpasta-Spasta<<"pasta remaining in hotel ";
      break;
    }
    case 3:
      cout<<"\n\n  enter the number of burger  you want from this hotel ::";
       cin>>quantites;
    if(Qburger-Sburger>=quantites)
    {
      Sburger=Sburger+quantites;
      Total_burger=Total_burger+quantites*220;
      cout<<"\n\n\t\t"<<quantites<<"burger have been ordered to you";
    }
    else
    {
      cout<<"\n\t only"<<Qburger-Sburger<<"burger remaining in hotel ";
      break;
    }
    case 4:
      cout<<"\n\n enter the number of plate of noodles you want from this hotel ::";
       cin>>quantites;
    if(Qnoodles-Snoodles>=quantites)
    {
      Snoodles=Snoodles+quantites;
      Total_noodles=Total_noodles+quantites*320;
      cout<<"\n\n\t\t"<<quantites<<"noodles have been alloted to you";
    }
    else
    {
      cout<<"\n\t only"<<Qnoodles-Snoodles<<"noodles remaining in hotel ";
      break;
    }
    case 5:
      cout<<"\n\n enter the number of shakes you want from this hotel ::";
       cin>>quantites;
    if(Qshake-Sshake>=quantites)
    {
      Sshake=Sshake+quantites;
      Total_shake=Total_shake+quantites*222;
      cout<<"\n\n\t\t"<<quantites<<"shakes have been gave to you";
    }
    else
    {
      cout<<"\n\t only"<<Qshake-Sshake<<"shake remaining in hotel ";
      break;
    }
    case 6:
      cout<<"\n\n enter the number of pieces chicken you want from this hotel ::";
       cin>>quantites;
    if(Qchicken-Schicken>=quantites)
    {
      Schicken=Schicken+quantites;
      Total_chicken=Total_chicken+quantites*110;
      cout<<"\n\n\t\t"<<quantites<<"chicken  have been ordered for you";
    }
    else
    {
      cout<<"\n\t only"<<Qchicken-Schicken<<"chicken remaining in hotel ";
      break;
    }
    case 7:
    cout<<"\n\t details of sales and collection";
    cout<<"\n\n number of rooms we had: "<<quantites;
    cout<<"\n\n number of rooms we gave for rent"<<Srooms;
    cout<<"\n\n remaining rooms we have "<<Qrooms-Srooms;
    cout<<"\n\n total rooms collected for the day is !!"<<Total_rooms;

   cout<<"\n\n number of pasta we had: "<<Qpasta;
    cout<<"\n\n number of pasta we gave to you"<<Spasta;
    cout<<"\n\n remaining pasta we have "<<Qpasta-Spasta;
    cout<<"\n\n total pasta collected for the day is !!"<<Total_pasta;

    cout<<"\n\n number of burger we had: "<<Qburger;
    cout<<"\n\n number of burger we gave to you"<<Sburger;
    cout<<"\n\n remaining burger we have "<<Qburger-Sburger;
    cout<<"\n\n total burger collected for the day is !!"<<Total_burger;

    cout<<"\n\n number of noodles we had: "<<Qnoodles;
    cout<<"\n\n number of noodles we gave to you"<<Snoodles;
    cout<<"\n\n remaining noodles we have "<<Qnoodles-Snoodles;
    cout<<"\n\n total number of plate collected for the day is !!"<<Total_noodles;

    cout<<"\n\n number of shake we had: "<<Qshake;
    cout<<"\n\n number of shake we gave to you "<<Sshake;
    cout<<"\n\n remaining shakes we have "<<Qshake-Sshake;
    cout<<"\n\n total number of shakes collected for the day is !!"<<Total_shake;


    cout<<"\n\n number of chicken we had: "<<Qchicken;
    cout<<"\n\n number of chicken we gave to you"<<Schicken;
    cout<<"\n\n remaining chicken we have "<<Qchicken-Schicken;
    cout<<"\n\n total number we collected for the day is !!"<<Total_chicken;

    case 8:
     exit(0);
    default:
    cout<<"\n please select the numbers mentioned above!!";


    
  }
  goto m;
}

