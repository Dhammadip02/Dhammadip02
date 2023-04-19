- 👋 Hi, I’m @DhammadipMendhe
- 👀 I’m interested in making website.
- 🌱 I’m currently learning compatative programming,
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me 

<!---
Dhammadip02/Dhammadip02 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include <iostream>
using namespace std;

int binary_search(int arr[],int n,int item){
    int mid=0;
    int low=0,high=n-1;
    while(low<=high){
        mid=(low+high)/2;
        if(arr[mid]==item)
        {
            return mid;

        }
        else   if(arr[mid]<item)

        {
          low = mid -1;
        }

        else{
         high  = mid+1;
        }
    }
    return -1;

}

int main()
{
    int arr[100];
    int n,item;
    cout<<"enter the array lenght"<<endl;
   cin>>n;
    cout<<"enter the array elements"<<endl;
    for(int i=0;i<n;i++)
    {
    cin>>arr[i];
    }

   int index= binary_search(arr,n,55);
cout<<"item is at position "<<index;


    cout<<" array elements are"<<endl;
    for(int i=0;i<n;i++)
    {
    cout<<arr[i]<<endl;
    }


    return 0;
}
