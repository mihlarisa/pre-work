# Practice trading journal (Trading 212 practice account)

Rules (in `trader/config.json`, in US dollars because the tools work in USD;
assumes about $1.30 per £1, so adjust if the rate moves a lot):

| rule | £ | $ in config |
| --- | --- | --- |
| practice budget | £500 | 650 |
| max loss per trade (stop hit) | £5 | 6.50 |
| daily loss limit, then stop for the day | £15 | 20 |
| max trades per day | 3 | 3 |
| min reward : risk | 1.5 | 1.5 |
| new entries only | 2:45 to 8:30 PM UK (9:45 AM to 3:30 PM New York) | |
| flat by | 8:55 PM UK (3:55 PM New York) | |

No options, margin, short selling or leverage. Practice account only until
the log below has at least 20 trades and you have read it honestly.

## How a practice trade runs

1. `/trader-scanner` after 2:50 PM UK, then pick one chart yourself.
2. `/trader-news TICKER`, `/trader-entry TICKER`, `/trader-exit`.
3. `/trader-timemachine`: if it says coin flip, consider skipping.
4. `/trader-budget`, then `/trader-risk` must say PASS.
5. Place it by hand in the Trading 212 **practice** account: the buy, plus a
   stop order at the stop price and a limit sell at the target.
6. Close anything still open by 8:55 PM UK. Log it below.

UK clock note: US and UK daylight saving change on different dates in March
and in late October / early November, so the UK times shift by an hour for a
couple of weeks then. New York time is always what counts.

## Log

| date | ticker | setup | entry | stop | target | shares | exit | result £ | followed the rules? | note |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
