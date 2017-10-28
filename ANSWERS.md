# Q0: Why is this error being thrown?

Because we haven't created a model for Pokemon yet.
# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *

The defaults seeds.rb file generated a couple pokemons once we seed the database, and the Home controller randomly selects the pokemons without a trainer. The common factor is that they don't have a trainer.
# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.

The line creates a button that sends a patch to path capture_path, which leads to the capture function in the Pokemon controller. It passes in the id of the Pokemon being captured so that the function can correctly assign and update the new trainer of the Pokemon.
# Question 3: What would you name your own Pokemon?

Boss
# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?

I passed in train_path with the trainer id of the trainer I wanted to render.
# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.

It catches the error using flash and renders the appropriate message.
# Give us feedback on the project and decal below!

Great class! Nothing to say.
# Extra credit: Link your Heroku deployed app
