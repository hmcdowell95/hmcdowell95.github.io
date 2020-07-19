---
layout: post
title:      "Rails Project"
date:       2020-07-10 12:29:56 -0400
permalink:  rails_project
---


The lesson I learned from this project that helped me in a tough spot was gems. Gems can be your friend. Right away you know your going to need to add "Omniauth" and "dotenv-rails". The gem that saved my project was "dynamic_form". One requirement is displaying errors on the text field on a form where an error occurred. Form_for automatically wraps div field_with_errors around each field but you still have to call out the errors in the form so the form has them to display. I struggled for hours trying to figure out how to make this work because I wasn't about to rebuild my form to form_tag. Then I found the gem dynamic_form, a simple gem that adds to FormBuilder and displays my errors with ease.
As I got closer to finishing my project I realized I didn't have one requirement. I needed a join table attribute that the user inputs. I wasn't sure what to do, I have users, systems, and games. With many-to-many relationships with users and games, and users and systems. So my join tables are usergames and usersystems. Since my main tables are users and games I focused on that. I thought about the relationship between a user and a game, then I realized what if a user inputs the last time they played that game. I added a migration to add :last_played attribute to UserGames, then I created a method in my games controller to take the last_played input from the user and save it. Lastly, I updated my games show page to display the last time the logged in user played the game if they have and they can enter and update the last time they played input. OH, and of course I added the method to my routes file. Finally, I have a new working attribute.
