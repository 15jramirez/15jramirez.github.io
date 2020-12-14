---
layout: post
title:      "Payment Reminder App- Sinatra Project"
date:       2020-12-14 04:03:50 +0000
permalink:  payment_reminder_app-_sinatra_project
---



# About the project
I am the type of person who often forgets stuff, espesically when it comes to payments. I thought it would be nice to create an app where it helps keep track of all your payments in one place. In the app-Payment Reminder- the user will be able to create an account or login to view their account. Once logged in the user can see all of their payments- if they have none, they can create a payment. With their payments, the user can see them more in depth, edit, or delete a payment. 

# Structure
 For my structure, I stayed with the convention, so I had my Restful and CRUD for my payments. I first set up my files( config.ru, gemfile, rakefile, and enviorment) before I got started. This helped me make sure no huge errors to emerge while I was knee deep in code. 

 
# Challenges 
This biggest challenge with this project is funy enough working with one of the gems- tux. It was diffult to get it started working. I spent two days troubleshooting the gem to even get started on the project. It really helped to start tracing back where I made changes. I ended up not using tux due to the constant error. I found out that for some reason, my app kept crashing when I would raise an error for migrations not run in my config.ru. this is the code below:
```

if ActiveRecord::Migrator.needs_migration?
  raise 'Migrations are pending. Run `rake db:migrate` to resolve the issue.'
end
```

Though, the hardest challenge of this project was gettng my edit route to work. The main issue I kept on getting is that my params id would be nil or 0. So that took me a couple of days to figure out what had happened-- thank goodness for binding.pry. I found this to be exteremly helpful in figuring out where errors would pop up. Though, I learned how important it is to take breaks!





