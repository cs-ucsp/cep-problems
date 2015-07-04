## Solución

Lo primero que debemos observar es que el límite para el precio de una naranja es $1000$ soles (deben ser naranjas muy especiales), y si consideramos que el costo de la última naranja podría ser $10^{12}$ soles nos daremos cuenta de que ese es un número muy grande.
En C++ los enteros (generalmente) son almacenados en un tipo de dato llamado integer de 4 bytes, eso quiere decir que tiene 32 bits (31 en realidad porque almacenamos el signo en un bit) para representar números, esto es cualquier número entre $2^{31}$ ($–2,147,483,648$) hasta $2^{31}-1$ ($2,147,483,647$), es decir approximadamente (2.1 veces) $10^9$.

Como el costo total podría exceder esa cantidad no podemos utilizar integers para resolver el problema. Por suerte también existe otro tipo de dato que nos permite almacenar números enteros mayores y es el long long con 8 bytes, por lo tanto tiene 64 bits para representar números (63 quitando el bit del signo), esto es cualquier número entre $-2^{63}$ ($-9,223,372,036,854,775,808$) hasta $2^{63}-1$ ($9,223,372,036,854,775,807$).

Entonces la solución más simple sería

``` cpp
#include <iostream>

using namespace std;

void main() {
	int k, w, n;
	cin >> k >> n >> w;
	long long total = 0;
	for (int i = 1; i <= w; ++i)
		total += i*k;
	if (total > n)
		cout << total - n << endl;
	else
		cout << 0 << endl;
}
```

Sin embargo, si recordamos nuestras clases de matemática podemos ver que $k$ siempre es una constante, entonces podríamos factorizarlo y luego nos quedamos con un sumatorio de la siguiente forma $1 + 2 + 3 + \ldots + w$ que para nuestra suerte tiene una fórmula cerrada que es $\sum_{i=1}^{w} = \frac{w(w+1)}{2}$.

Si modificamos ligeramente el código tenemos:

``` cpp
#include <iostream>

using namespace std;

void main() {
	long long k, w, n;
	cin >> k >> n >> w;
	long long total = k * (w *(w + 1)) / 2;
	cout << (total > n ? total - n : 0 ) << endl;
}
```
