# №3 Попарное тестирование значений для поля авторизации на сайте https://www.saucedemo.com
<table>
	<tbody>
		<tr>
			<td>Логин</td>
			<td>Пароль</td>
		</tr>
		<tr>
			<td>пустой</td>
			<td>пустой</td>
		</tr>
		<tr>
			<td>валидный standard_user</td>
			<td>валидный</td>
		</tr>
		<tr>
			<td>валидный locked_out_user</td>
			<td>невалидный</td>
		</tr>
		<tr>
			<td>валидный problem_user</td>
			<td></td>
		</tr>
		<tr>
			<td>валидный performance_glitch_user</td>
			<td></td>
		</tr>
		<tr>
			<td>невалидный</td>
			<td></td>
		</tr>
	</tbody>
</table>


Список полученных комбинаций
<table>
	<tbody>
		<tr>
			<td>№</td>
			<td>Логин</td>
			<td>Пароль</td>
		</tr>
		<tr>
			<td>1</td>
			<td>пустой</td>
			<td>пустой</td>
		</tr>
		<tr>
			<td>3</td>
			<td>пустой</td>
			<td>валидный secret_sauce</td>
		</tr>
		<tr>
			<td>3</td>
			<td>пустой</td>
			<td>невалидный (ucbydcgyu32555)</td>
		</tr>
		<tr>
			<td>4</td>
			<td>валидный standard_user</td>
			<td>пустой</td>
		</tr>
		<tr>
			<td>5</td>
			<td>валидный standard_user</td>
			<td>валидный secret_sauce</td>
		</tr>
		<tr>
			<td>6</td>
			<td>валидный standard_user</td>
			<td>невалидный (ucbydcgyu32555)</td>
		</tr>
		<tr>
			<td>7</td>
			<td>валидный locked_out_user</td>
			<td>пустой</td>
		</tr>
		<tr>
			<td>8</td>
			<td>валидный locked_out_user</td>
			<td>валидный secret_sauce</td>
		</tr>
		<tr>
			<td>9</td>
			<td>валидный locked_out_user</td>
			<td>невалидный (ucbydcgyu32555)</td>
		</tr>
		<tr>
			<td>10</td>
			<td>валидный problem_user</td>
			<td>пустой</td>
		</tr>
		<tr>
			<td>11</td>
			<td>валидный problem_user</td>
			<td>валидный secret_sauce</td>
		</tr>
		<tr>
			<td>12</td>
			<td>валидный problem_user</td>
			<td>невалидный (ucbydcgyu32555)</td>
		</tr>
		<tr>
			<td>13</td>
			<td>валидный performance_glitch_user</td>
			<td>пустой</td>
		</tr>
		<tr>
			<td>14</td>
			<td>валидный performance_glitch_user</td>
			<td>валидный secret_sauce</td>
		</tr>
		<tr>
			<td>15</td>
			<td>валидный performance_glitch_user</td>
			<td>невалидный (ucbydcgyu32555)</td>
		</tr>
		<tr>
			<td>16</td>
			<td>невалидный</td>
			<td>пустой</td>
		</tr>
		<tr>
			<td>17</td>
			<td>невалидный</td>
			<td>валидный secret_sauce</td>
		</tr>
		<tr>
			<td>18</td>
			<td>невалидный</td>
			<td>невалидный (ucbydcgyu32555)</td>
		</tr>
	</tbody>
</table>

### Тест-кейсы проверки авторизации

#### ТК №1

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ничего не вводить;
2. В поле пароль оставить пустым;
3. Нажать "LOgin".

ОР:
Сайт выдаст ошибку/запросит логин и пароль.

ФР:
Epic sadface: Username is required.

#### ТК №2

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ничего не вводить;
2. В поле пароль ввести secret_sauce ;
3. Нажать "LOgin".

ОР:
Сайт выдаст ошибку/запросит логин и пароль.

ФР:
Epic sadface: Username is required.

#### ТК №3

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ничего не вводить;
2. В поле пароль ввести ucbydcgyu32555;
3. Нажать "LOgin".

ОР:
Сайт выдаст ошибку/запросит логин и пароль.

ФР:
Epic sadface: Username is required.


#### ТК №4

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести standard_user;
2. В поле пароль ввести secret_sauce;
3. Нажать "LOgin".

ОР:
Авторизация пройдена, откроется витрина сайта

ФР:
Авторизация пройдена, открывается витрина сайта

#### ТК №5

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести standard_user;
2. В поле пароль оставить пустым;
3. Нажать "LOgin".

ОР:
Сайт выдаст ошибку/запросить логин и пароль.

ФР:
Epic sadface: Username is required.

#### ТК №6

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести standard_user;
2. В поле пароль ввести ucbydcgyu32555;
3. Нажать "LOgin".

ОР:
Сайт укажет на ошибку в пароле, авторизация не пройдена.

ФР:

Epic sadface: Username and password do not match any user in this service.

#### ТК №7

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести locked_out_user;
2. В поле пароль ввести secret_sauce;
3. Нажать "LOgin".

ОР:
Пользователь заблокирован, нет доступа к сайту.

ФР:
Epic sadface: Sorry, this user has been locked out.

#### ТК №8

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести locked_out_user;
2. В поле пароль оставить пустым;
3. Нажать "LOgin".

ОР:
Сайт выдаст ошибку/запросит пароль.

ФР:
Epic sadface: Password is required.

#### ТК №9

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести locked_out_user;
2. В поле пароль ввести ucbydcgyu32555;
3. Нажать "LOgin".

ОР:
Сайт укажет на ошибку в пароле, авторизация не пройдена.

ФР:

Epic sadface: Username and password do not match any user in this service.

#### ТК №10

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести problem_user;
2. В поле пароль ввести secret_sauce;
3. Нажать "LOgin".

ОР:
Авторизация пройдена, откроется витрина сайта

ФР:
Авторизация пройдена, открывается витрина сайта

#### ТК №11

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести problem_user;
2. В поле пароль оставить пустым;
3. Нажать "LOgin".

ОР:
Сайт выдаст ошибку/запросить логин и пароль.

ФР:
Epic sadface: Username is required.

#### ТК №12

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести problem_user;
2. В поле пароль ввести ucbydcgyu32555;
3. Нажать "LOgin".

ОР:
Сайт укажет на ошибку в пароле, авторизация не пройдена.

ФР:

Epic sadface: Username and password do not match any user in this service.

#### ТК №13

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести performance_glitch_user;
2. В поле пароль ввести secret_sauce;
3. Нажать "LOgin".

ОР:
Авторизация пройдена, откроется витрина сайта

ФР:
Авторизация пройдена, открывается витрина сайта

#### ТК №14

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести performance_glitch_user;
2. В поле пароль оставить пустым;
3. Нажать "LOgin".

ОР:
Сайт выдаст ошибку/запросить логин и пароль.

ФР:
Epic sadface: Username is required.

#### ТК №15

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести performance_glitch_user;
2. В поле пароль ввести ucbydcgyu32555;
3. Нажать "LOgin".

ОР:
Сайт укажет на ошибку в пароле, авторизация не пройдена.

ФР:

Epic sadface: Username and password do not match any user in this service.

#### ТК №16

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести gfynt2513;
2. В поле пароль ввести ucbydcgyu32555;
3. Нажать "LOgin".

ОР:
Сайт укажет на ошибку в логине/пароле, авторизация не пройдена.

ФР:

Epic sadface: Username and password do not match any user in this service.

#### ТК №17

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести gfynt2513;
2. В поле пароль остаивть пустым;
3. Нажать "LOgin".

ОР:
Сайт укажет на ошибку в пароле, авторизация не пройдена.

ФР:

Epic sadface: Password is required.

#### ТК №18

Предусловия:

1.Открыть сайт https://www.saucedemo.com

Шаги:
1. В поле логин ввести gfynt2513;
2. В поле пароль ввести secret_sauce;
3. Нажать "LOgin".

ОР:
Сайт укажет на ошибку в пароле, авторизация не пройдена.

ФР:

Epic sadface: Username and password do not match any user in this service.
