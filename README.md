# dsa1
//do union (using sets)
#include <iostream>
#include <bits/stdc++.h>

using namespace std;

int doUnion(int a[], int n, int b[], int m)
{
    unordered_set<int> s;
    for (int i = 0; i < n; i++)
        s.insert(a[i]);
    for (int j = 0; j < m; j++)
        s.insert(b[j]);
    return s.size();
}
int main()
{
    int a[] = {1, 2, 3, 4, 5, 6};
    int b[] = {6, 7, 8, 2, 9, 0, 5, 12};
    int n = sizeof(a) / sizeof(a[0]);
    int m = sizeof(b) / sizeof(b[0]);
    cout << doUnion(a, n, b, m);
    return 0;
