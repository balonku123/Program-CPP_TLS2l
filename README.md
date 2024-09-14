#include <iostream>
using namespace std;
int main() {
    
    string a,b;
    double c,d;
    cout<< "From (Kelvin/Celcius/Fahrenheit): "; cin >> a;
    cout<< "To   (Kelvin/Celcius/Fahrenheit): ";cin>> b;
    cout<<"Degree: ";cin>> c;
    
    
    if (a==b){
        cout << c<< " "<<a<< " = "<<c<<" "<<a;
    }
    else { if (a=="Kelvin" and b=="Celcius")
    {
            d=c-273;
        }
        else if (a=="Kelvin" and b=="Fahrenheit")
        {
            d=(c-273)*9/5+32;
        }
        else if (a=="Celcius" and b=="Kelvin")
        {
            d=c+273;
        }
        else if (a=="Celcius" and b=="Fahrenheit")
        {
            d=(c*9/5)+32;
        }
        else if (a=="Fahrenheit" and b=="Kelvin")
        {
            d=(c-32)*5/9+273;
        }
        else if (a=="Fahrenheit" and b=="Celcius")
        {
            d=(c-32)*5/9;
        }
    cout <<c<<" "<< a << " Equals to "<<d<<" "<<b ;
       
    }       

    return 0;
}
