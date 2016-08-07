# fine_ants_app 🐜

Designed to be used in conjunction with
[fine_ants](https://github.com/searls/fine_ants).  🐜

## setup

**This app isn't secured! At all! It's meant to be run locally! Don't go
deploying it to Heroku or Google or the Cloud!**

### install

```
$ git clone git@github.com:searls/fine_ants_app.git #  🐜
$ cd fine_ants_app
$ bundle
$ bundle exec rake db:create db:migrate
$ bundle exec rails s
```

That'll get the server going at [http://localhost:3000](http://localhost:3000).

### create stuff

1. Create a bank (e.g. named "Vanguard", adapter "vanguard")
[here](http://localhost:3000/admin/banks/new)
2. Create a user for that 🐜 bank with your user and password
[here](http://localhost:3000/admin/users/new)
3. Head 🐜 back to the [dashboard](http://localhost:3000/) and click
"Update Accounts" to kick off update process. This will save off `Snapshot`
models for each of your accounts
4. After the 🐜 update finishes, your dashboard should tally up your accounts based
on their latest snapshots, giving you the grand total

