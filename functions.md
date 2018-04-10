
// 最大公约数
int gcd ( int n , int m )
{
    int r = 0;
    while ( m )
    {
        r = n % m;
        n = m;
        m = r;
    }
    return n;
}
