###Using seeds.rb and new app 

####Create new app
Create new app
```rails new demoapp08 -B -T
cd demoapp-08
bundle install --local```
Create model 
```rails g model Person name:string```
Run rake command 
```rake db:reset```
Open Rails Console
``` rails c 
Person.count
=>0```
Open db/seeds.rb with sublime text
```subl db/seeds.rb```
###seeds.rb data
####Create a new person on seeds.rb
```people = Person.create([{name: "Oğuz"}])```
Rub rake command
```rake db:seed```
###Open rails console
```rails c
Person.count
=>1
Person.first.name
=>"Oğuz"```
