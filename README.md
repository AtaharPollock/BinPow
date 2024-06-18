ll binpow(ll a,ll b)
{
    ll ans=1;
    while(b>0)
    {
        if(b&1)
        {
           //ans*=a;
           ans=(ans*a)%mod;
        }

        a=(a*a)%mod;
        //a*=a;
        b>>=1;
    }
    return ans;
}
