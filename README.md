\# Bank Account


Учебный проект на Python, моделирующий банковский счет и транзакции.


\## Возможности


\- создание счета с начальным балансом;

\- добавление транзакций;

\- запрет операций, уводящих баланс в минус;

\- неизменяемые транзакции через `dataclass`;

\- пользовательские исключения;

\- создание счета из CSV-строки.

## Technologies

- Python 3
- OOP
- Dataclasses
## Usage

```python
from account import Account, Transaction

account = Account("Oleg", 1000)
account.add_transaction(Transaction(-250, "Shopping"))

print(account.balance)