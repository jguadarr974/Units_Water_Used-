
#include <iostream>
using namespace std;
//Programmer: Jennifer Guadarrama
//This program is to calculate the total number of units of water used. Fees are charged $8 for customers. People on the Super Savings Plan will be charged $6. 6% of taxes is added on the total bill.
int main(int argc, const char * argv[]) {
    int id, val1, val2, val3, ans;
    float bill=0, rate, tax, charge,total;
    cout<<"Enter your ID number ";
    cin>>id;
    cout<<"Enter last reading of water meter ";
    cin>>val1;
    cout<<"Enter new reading of water meter ";
    cin>>val2;
    cout<<"Are you in the Super Savings Plan?\n"<<"Enter 1 for yes or 0 for no\n";
    cin>>ans;
    val3= val2- val1;//number of units water was used
    if (val3< 200)
        rate= val3 * 0.08;
    if (val3<800)
        rate= val3 * 0.07;
    else
        rate= val3 * 0.05;
    if (ans==1)
        bill= 14 + rate;//$6 fee plus $8 for service charge= $14
    else if ( ans==0)
        bill= 8 + rate;
    if (ans==1&&bill>35)
        bill= bill* .8;//20% discount
    tax= bill * 0.06;//6% of taxes
    charge=bill;//to display the charge only, before taxes
    total= charge + tax;
    total=(int)(total * 100 + 0.5)/100.0;
    cout<<"Customer ID: "<<id<<endl<<"Previous reading: "<<val1<<endl<<"New Reading: "<<val2<<endl<<"Units of water used: "<<val3<<endl<<"charges: "<<charge<<endl<<"Tax: "<<tax<<endl<<"Amount due: "<<total<<endl;
}
