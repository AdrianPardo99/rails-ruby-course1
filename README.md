# Ruby on Rails from the Ruby course 1 #
## For install rails ##
```bash
  gem update
  gem install rails
```
__If you maybe clone de project and rails not run you've added the gems__
```bash
  bundle install
```

# What's Ruby on Rails #
Rails is a web framework for develop applications and many things for the web. Rails is powerful if you want to make a view that contains Create, Update, Modify and Delete petition you can run the next command

```bash
#In the path of the application run:
  bin/rails generate scaffold <Name> <title>:<type-of-data>

#The view in the example names: Course title:string
```
If you want to run again the rails server, maybe the server makes and show you an error, for solving you only need to run
```bash
  bin/rails db:migrate
```

Many of the layouts and views in Rails works with the pattern desing MCV

You can interact with the rails console and you only have to run
```bash
  bin/rail console
```

In the Course Controller-View you can interact with the information if you want, This interactive mode runs a methods and functions with SQL statements
```ruby
  Course.exists? <id> # Bool return
  Course.first        # First reg return
  Course.last         # Last reg return
  Course.all          # All reg
#For create a new object o Reg
  var=Course.new
  var                 # For see the information, you can modify the information with the attr_accessor
  var.param=""

# For commit/save the information you only need to run
  var.save

# You can modify a register if you want
  v=Course.<statementFind>()
  v=Course.find(1)
  v.param="Modify information"
  v.save

# If you want to delete the register you need to run
  v=Course.find(1)
  v.destroy           # Destroy immediatly the register watch out
```
