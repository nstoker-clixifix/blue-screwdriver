# Blue Screwdriver

This project is following the expenses tracker section of the [EffectiveTesting with RSPEC 3](https://pragprog.com/titles/rspec3/effective-testing-with-rspec-3/) book. The [errata](https://pragprog.com/cms/errata/rspec3-errata/) for the book.

Any good stuff is from the book, errors and ommissions are all my own work.

The basic application is set up and working.

## Running manually

The server can be started by running `bundle exec rackup`.

To add a new record:

```bash
curl localhost:9292/expenses --data '{"payee":"Gannymede", "amount": 1.25, "date":"2020-09-11"}' -w "\n"
# {"expense_id":3}
```

To get expenses for a specific date:

```bash
curl localhost:9292/expenses/2020-09-11 -w "\n"
# curl localhost:9292/expenses --data '{"payee":"Gannymede", "amount": 1.25, "date":"2020-09-11"}' -w "\n"
```

## Documentation

Documentation [such as it is](doc/ExpenseTracker/index.html).

The [YARD](https://github.com/lsegal/yard) and [yard-sinatra](https://github.com/rkh/yard-sinatra) gems were used to produce the documentation.

To manually regenerate the documentation:

```bash
yard --plugin yard-sinatra --protected --private
```

## Lolcommits

Just for fun, [lolcommits](https://lolcommits.github.io/) has been enabled on this repository.

To enable (once the gem has been installed) type `lolcommits --enable`. To switch off `lolcommits --disable`.
