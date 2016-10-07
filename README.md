#>>VARIABLE SCOPE

So we are writing some code to help create a user for our website. 

	def user(username)
  		puts username
	end

Our first method takes in a desired username and returns it.

	def user(username)
  		puts username
	end

	def password(password)
		puts password
	end	

Our next method takes in a persons password

	def user(username)
  		puts username
	end

	def password(password)
		puts password
	end	
	
	def user_info
		puts username
  		puts password
	end
	
And last but not least, we create a method that prints both of those variables for us. Let's run these methods:

	user("ladybug2000")
		>>"ladybug2000"
	password("1234")
		>>"1234
	user_info
		>>in `user_info': undefined local variable or method `username' for main:Object (NameError)

Uh oh. The method `user_info` doesn't seem to know what these variables are....		

In Ruby, variables have a set scope. They are only known to their 'local' environment- here, because both `username` and `password` were defined within methods, only those methods know about those variables. This makes passing around info from method to method a headache of sorts. 		Good thing Ruby has a solution for us, that we'll learn about next.

