
// 最大公约数
int gcd ( int x , int y )
{
    if ( 0 == x
         || 0 == y )
    {
        return 0;
    }

    int z = y;
    while ( x % y != 0 )
    {
        z = x % y;
        x = y;
        y = z;
    }
    return z;
}
