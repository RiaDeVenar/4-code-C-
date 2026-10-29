# 4-code-C-
Отгадай карту за 6 вопросов
#include <iostream>
#include <string>
using namespace std;

int main()
{
string card;
string color;
string answer;
cout << "1) Это красная карта?: ";
cin >> answer;

if(answer == "да")
{
    cout << "2) Масть карты - черви?: ";
    cin >> answer;
    if(answer == "да")
    {
        color = "черви";
    }
    
       else 
    {
        color = "бубны";
    }
}

else
{
    cout << "2) Масть карты - пики?: ";
    cin >> answer;
    
    if(answer == "да")
    {
        color = "пики";
    }
    
       else 
    {
        color = "трефы";
    }
}

cout << "3) Эта карта 10 или ниже?: ";
cin >> answer;

if(answer == "да")
{
    cout << "4) 8 побьёт эту карту?: ";
    cin >> answer;
    
    if(answer == "да")
    {
        cout << "5) 7 побьёт эту карту?: ";
        cin >> answer;
    
        if(answer == "да")
        {
            cout << "6) Это 6? ";
            cin >> answer;
            card = "6";
        }

        else
        {
            cout << "6) Это 7? ";
            cin >> answer;
            card = "7";
        }
    }
    else
    {
        cout << "5) 9 побьёт эту карту?: ";
        cin >> answer;

        if(answer == "да")
        {
            cout << "6) Это 8? ";
            cin >> answer;
            card = "8";
        }
        
        else
        {
            cout << "6) Это 9? ";
            cin >> answer;
            
            if(answer == "да")
            {
            card = "9";
            }
            
            else
            {
            card = "10";
            }
        }
    }
}

else
{
    cout << "4) Это туз?: ";
    cin >> answer;
    
    if (answer == "да")
    {
        card = "Туз";
    }
    else
    {
        cout << "5) Это дама?: ";
        cin >> answer;
        
        if (answer == "да")
        {
            card = "Дама";
        }
        else 
        {
            cout << "6) Это король?: ";
            cin >> answer;
            
            if (answer == "да")
            {
                card = "Король";
            }
            else
            {
                card = "Валет";
            }
        }
    }
}
cout << "Твоя карта: " << card << " " << color << endl;
return 0;
}
