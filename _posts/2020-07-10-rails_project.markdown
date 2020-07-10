---
layout: post
title:      "Rails Project"
date:       2020-07-10 16:29:55 +0000
permalink:  rails_project
---


The lesson I learned from this project that helped me in a tough spot was gems. Gem can be your friend. Right away you know your going to need to add "Omniauth" and "dotenv-rails". The gem that saved my project was "dynamic_form". One requirement is displaying errors on the text field on a form where an error occurred. Form_for automatically wraps div field_with_errors around each field but you still have to call out the errors in the form so the form has them to display. I struggled for hours trying to figure out how to make this work because I wasn't about to rebuild my form to form_tag. Then I found the gem dynamic_form, a simple gem that adds to FormBuilder and displays my errors with ease.
