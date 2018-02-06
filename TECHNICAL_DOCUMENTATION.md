# Cryptospy - Technical Documentation

## Data Storage

Cryptospy stores exchange rates in a SQLite database. The database consists of the single table "exchange_rates".

| Column | Type | Comment |
| :-: | :-: | :- |
| moment | INTEGER | Date and time when the exchange rate was valid. |
| crypto_cur | TEXT | Symbol of the crypto currency. |
| real_cur | TEXT | Symbol of the real currency. |
| exc_rate | REAL | Exchange rate (value of 1 crypto_cur in real_cur). |

The table can be created using the following SQL command: `CREATE TABLE exchange_rates (moment INTEGER, crypto_cur TEXT, real_cur TEXT, exc_rate REAL)`

