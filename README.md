# Fake-Headline-New

# 1) Start the program
# 2) Import the 'random' module\
# 3) Create a list of _Subjects
# Example : ["Yogesh Bagal", "Amit Kumar", "Roshan Lal", "A Delhi City", "A Group of ERA ENGINEERING" ]
# 4) Create a list of Indian actions.
# Example : ["Lounches", "chancels"]

# Which form(s) of written Hindi can you read and write?

# 1) import the rendom module
import random

# 2) Create a subject in the list
subject=[
  "Roshan Lal",
  "Shahrukh Khan",
  "Amitab Bachan",
  "A Group of Era Engineering",
  "The Fire Fighting Services",
  "A CM in Delhi",
]

# Create a list of possible choices
action=[
  "lunches new app", 
  "cancel event",
  "a eats",
  "Great Celebration",
  "orders bitcoin",
  "relased a book story",
  ]

# create a place of 

places_or_thinks=[
  "at V3S Mall",
  "in the Delhi Metro",
  "in party on 23rd Oct 2025",
  "inside parliament",
  "a build new app",
  "at Pune",
]

# 3) Start the Headline Generation loop
while True:
  r_subject = random.choice(subject)
  r_action = random.choice(action)
  r_places_or_thinks = random.choice(places_or_thinks)
  
  headline = f" BREAKING NEWS: {r_subject} {r_action} {r_places_or_thinks} "
  print("\n" + headline)

  user_input = input("\nWould you like to generate another headline? (yes/no): ").strip().lower()
  if user_input == "no":
    break

# Print a thank you message
print("\nThank you for using the Headline Generator!")
