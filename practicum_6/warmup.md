## Санкт-петербургский парадокс

Единичное испытание в петербургской игре состоит в бросании правильной монеты до тех пор, пока не выпадет решка; если это произойдет при $r$-м бросании, игрок получает $2^r$ долларов из банка. Таким образом, с каждым бросанием выигрыш удваивается. Вопрос -- сколько следует заплатить игроку за участие в игре, чтобы игра стала безобидной (среднее значение, т.е. мат. ожидание, равно нулю)?

**Ответ:** при любом взносе игра не является безобидной в оригинальной постановке, потому что мат. ожидание всегда больше нуля. Действительно, рассмотрим вероятность окончания игры при $k$-м бросании. Она равна $1/2^k$. Тогда банк в среднем должен заплатить
$$
2 \frac{1}{2} + 4 \frac{1}{4} + \dots = 1 + 1 + \dots
$$
что составляет бесконечно большую сумму, так что игра может стать безобидной только при бесконечном взносе. Бюффон и Крамер предложили разрешить парадокс, предположив, что банке может заплатить только конечную сумму, например, миллион. Тогда мат. ожидание выигрыша
$$
2 \frac{1}{2} + 4 \frac{1}{4} + \dots + 2^{19} \frac{1}{2^{19}} + 10^6 \left( \frac{1}{2^{20}} + \frac{1}{2^{21}} + \dots \right) \approx 21
$$
(здесь мы использовали факт того, что $2^{19} < 10^{6} < 2^{20}$). Тогда игра становится безобидной при взносе в 21 доллар.

## Таблица истинности для импликации

Как выглядит таблица истинности для импликации $P \rightarrow Q$?

**Ответ:** из лжи может следовать что угодно, из правды только правда (пример: $P(x) := x > 2$ и $Q(x) := x^2 > 4$)

| $P$ | $Q$ | $P \rightarrow$ Q |
|-----|-----|-------------------|
| F | F | T |
| F | T | T |
| T | F | F |
| T | T | T |

## Группы

Известно, что $(\mathbb{Z}, +)$ является группой. Но является ли группой $(\mathbb{Z}_n, +)$, где $\mathbb{Z}_n$ - целые числа по модулю $n$, а "+" определен как $a + b = ((a + b) \mod n)$.

**Ответ:** да. Аксиомы группы:

1. ассоциативность: $(a + b) + c = a + (b + c)$
2. нейтральный элемент: $a + e = e + a = a$
3. обратный элемент: $a + a^{-1} = a^{-1} + a = e$

Тогда в силу симметрии относительно нуля $(\mathbb{Z}_n, +)$ будет группой.