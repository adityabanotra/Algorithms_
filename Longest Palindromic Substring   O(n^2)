int max(int a,int b)
{
    if(a>b)
        return a;
    return b;
}
int countPalindromeSubstrings(char s[]) {
	
    int n=strlen(s);
    
    int ans =0;
    for(int i=0;i<n;i++)
    {
        int l=i-1,r=i+1;
        
        int count = 1;
        while(l>0&&r<n)
        {
            if(s[l]!=s[r])
                break;
            count+=(r-l);
            l--;
            r++;
        }
        
        ans=max(ans,count);
    }
    
    for(int i=0;i<n-1;i++)
    {
        if(s[i]==s[i+1])
        {
            int l=i-1,r=i+2;
        
        int count = 2;
        while(l>0&&r<n)
        {
            if(s[l]!=s[r])
                break;
            count+=(r-l-1);
            l--;
            r++;
        }
        
        ans=max(ans,count);
        }
    }
    
    return ans;
	
}


int main() {
    char input[10000];
    cin >> input;
    cout << countPalindromeSubstrings(input) << endl;
}
