---
{"dg-publish":true,"permalink":"/newman/stem-programming-presentation/mad-libs-code/","noteIcon":""}
---


```
# ==============================================================================
#           THE ULTIMATE PYTHON MAD LIBS: INTERSTELLAR CHAOS EDITION
# ==============================================================================
# Rules:
# - strings go in "quotes"
# - integers are whole numbers (no quotes, no decimal point)
# - floats are decimal numbers (no quotes, must have a decimal point)
# - booleans are True or False (no quotes, capital first letter)
#
# PRO TIP: The weirder your inputs, the more catastrophic the script becomes.

# --- PERSON 1: THE PRESIDENT ---
p1_name = "Alex"                         # str: text/string value
p1_is_male = True                        # bool: True or False value
p1_age = 58                              # int: whole number
p1_height_inches = 73                    # int: height in inches, 73 inches = 6 ft 1 in
p1_dancing_skill = 7.4                   # float: dancing skill on a scale from 1.0 to 10.0
p1_hometown = "Toledo"                   # str: text/string value
p1_birthday = "July 4"                   # str: text/string value; used as the catastrophic invasion date
p1_fav_food = "spaghetti"                # str: text/string value
p1_fav_color = "neon green"              # str: text/string value
p1_fav_animal = "capybara"               # str: text/string value
p1_fav_team = "Chiefs"                   # str: text/string value; do NOT include "the" or "The"
p1_guilty_pleasure = "dad rock karaoke"  # str: text/string value
p1_reelected = True                      # bool: True or False value

# --- PERSON 2: THE SCIENCE ADVISOR ---
p2_name = "Jordan"                         # str: text/string value
p2_is_male = False                         # bool: True or False value
p2_age = 43                                # int: whole number
p2_height_inches = 64                      # int: height in inches, 64 inches = 5 ft 4 in
p2_singing_skill = 8.9                     # float: singing skill on a scale from 1.0 to 10.0
p2_known_since_year = 2019                 # int: whole number year
p2_birthday = "November 3"                 # str: text/string value; used as the top-secret discovery date
p2_fav_food = "tacos"                      # str: text/string value
p2_fav_color = "purple"                    # str: text/string value
p2_fav_animal = "raccoon"                  # str: text/string value
p2_fav_team = "Lakers"                     # str: text/string value; do NOT include "the" or "The"
p2_guilty_pleasure = "bad reality TV"      # str: text/string value
p2_speaks_alien = False                    # bool: True or False value

# --- EXPANDED UNHINGED VARIABLES ---
p1_cry = "Yeehaw"                    # str: battle cry, scream, or vocalization
target_body_part = "left pinky toe"  # str: anatomical feature
alien_action = "breakdancing"        # str: action verb ending in "-ing"
weird_unit = "bananas-per-hour"      # str: ridiculous unit of measurement
p1_food_unit = "bucket"              # str: how you count the favorite food, like bowl, slab, or vat

# ==============================================================================
# --- DO NOT EDIT BELOW THIS LINE --- (Unless you want to break the space-time continuum)
# ==============================================================================
import time

p1_pronoun = "he" if p1_is_male else "she"                         # str: subject pronoun
p1_possessive_pronoun = "his" if p1_is_male else "her"              # str: possessive pronoun
p1_object_pronoun = "him" if p1_is_male else "her"                  # str: object pronoun
p1_address = "Mr. President" if p1_is_male else "Madam President"   # str: formal address
p1_title = "sir" if p1_is_male else "ma'am"                         # str: polite title

p2_pronoun = "he" if p2_is_male else "she"                # str: subject pronoun
p2_possessive_pronoun = "his" if p2_is_male else "her"    # str: possessive pronoun
p2_object_pronoun = "him" if p2_is_male else "her"        # str: object pronoun

# Mathematical Absurdity Computations
height_difference = abs(p1_height_inches - p2_height_inches)  # int: positive height difference in inches

ship_count = int((p1_age * p2_age) / height_difference) if height_difference != 0 else 42
# int: calculated number of alien ships

ufo_speed = round((p1_age ** 2) * (p2_height_inches / 12), 1)
# float: calculated UFO speed

total_height_stack = round((p1_height_inches / 12) * ship_count, 2)
# float: calculated stacked ship height in feet

wormhole_intensity = round(p1_dancing_skill * p2_singing_skill, 2)
# float: calculated wormhole intensity based on dancing and singing

alien_head_circumference = round((p1_dancing_skill + p2_singing_skill) * 3, 1)
# float: calculated alien head circumference in inches

print("=" * 70)
print(f" CLASSIFIED TOP SECRET: THE {p1_name.upper()} CONTACT PROTOCOL")
print("=" * 70)
print()

time.sleep(1)

print(f"It was 3:00 AM in the Oval Office. President {p1_name}, the legendary")
print(f"{p1_fav_animal} enthusiast from {p1_hometown}, was sitting alone.")
print(f"Despite being {p1_age} years old and standing at a statuesque {p1_height_inches} inches tall,")
print(f"{p1_pronoun} was currently stress-eating a massive {p1_food_unit} of cold {p1_fav_food}")
print(f"directly off the historic Resolute Desk.")
print()

time.sleep(1)

print(f"Suddenly, the door exploded into splinters. Dr. {p2_name} ({p2_age} years old,")
print(f"with {p2_height_inches} inches of pure unhinged scientific energy) burst into the room.")
print(f"The advisor had known the President since {p2_known_since_year}, but had never looked")
print(f"this frantic. {p2_pronoun.capitalize()} was wearing a glowing {p2_fav_color} lab coat and")
print(f"clutching a secret weapon: a lukewarm serving of {p2_fav_food}.")
print()

print(f"'{p1_address}!' Dr. {p2_name} wheezed, sprinting forward. 'The countdown has ended!")
print(f"A subspace wormhole has just opened directly over the local Walmart in {p1_hometown}!'")
print(f"NASA later confirmed the wormhole had an intensity rating of {wormhole_intensity}.")
print(f"Apparently, {p1_name}'s dancing skill of {p1_dancing_skill} combined with")
print(f"Dr. {p2_name}'s singing skill of {p2_singing_skill} had created the first known")
print(f"musical tear in space-time.")
print()

print(f"The President choked on {p1_possessive_pronoun} {p1_fav_food}, letting out a sharp, panicked, '{p1_cry.upper()}!'")
print(f"'Explain yourself!' {p1_pronoun} demanded.")
print()

time.sleep(1)

print(f"'The aliens are invading on {p1_birthday}!' Dr. {p2_name} screamed. 'The Pentagon has bypassed")
print(f"Condition Red! The military is officially at DEFCON {p1_fav_color.upper()}!'")
print(f"'How many ships?' asked the President.")
print(f"'{ship_count} dreadnoughts,' whispered Dr. {p2_name}. 'They are tracking towards Earth")
print(f"at a staggering velocity of {ufo_speed} {weird_unit}!'")
print()

print(f"'And what do these ships look like?' {p1_name} whispered, sweat dripping down {p1_possessive_pronoun} face.")
print(f"'They look exactly like giant, interstellar {p2_fav_animal}s,' Dr. {p2_name} admitted.")
print(f"'We've actually had them captured in our zoos since {p2_birthday}, but I was too busy")
print(f"indulging in my secret {p2_guilty_pleasure} binges to realize they were spying on your {target_body_part}!'")
print(f"'While I was practicing my {p1_guilty_pleasure} sessions?!' gasped {p1_name}.")
print()

# --- THE DYNAMIC BOOLEAN SPEECH CHECK ---
print(f"--- ATTEMPTING ALIEN LINGUISTIC LINK: [ SPEAKS_ALIEN = {p2_speaks_alien} ] ---")
time.sleep(1)

if p2_speaks_alien:
    print(f"Dr. {p2_name} tapped a button on {p2_possessive_pronoun} watch. 'Luckily, I speak fluent alien.")
    print(f"I broadcasted a peace message, but because of a syntax error, I accidentally told")
    print(f"their commander that {p1_hometown} is built entirely out of weaponized {p1_fav_food}.'")
else:
    print(f"'We can't communicate!' Dr. {p2_name} wailed. 'Because I don't speak alien, I tried to")
    print(f"gesture with my hands and accidentally declared war on their entire solar system!'")
print()

print(f"'Then how do we stop them?' asked {p1_address}.")
print(f"Dr. {p2_name} smirked and held up a poster of the {p2_fav_team}. 'We challenge them to sports.'")
print(f"'The {p2_fav_team}?!' {p1_name} yelled. 'You could have used my beloved {p1_fav_team}!'")
print(f"'The aliens specifically intercepted a broadcast of the {p2_fav_team}, {p1_title}, and they")
print(f"consider it a holy text. I have the emails.'")
print()

time.sleep(1)

print(f"The President turned to the bulletproof window. Outside, descending from the sky and")
print(f"landing right onto the South Lawn, were the {ship_count} alien craft. Stacked on top of")
print(f"each other, they stood an imposing {total_height_stack} feet tall. Through the smoke,")
print(f"thousands of extraterrestrial {p2_fav_animal}s emerged—and they were all aggressively")
print(f"{alien_action} in perfect synchronized harmony while wearing tiny {p1_fav_color} sashes.")
print(f"Each alien had a suspiciously round head measuring {alien_head_circumference} inches around,")
print(f"which scientists agreed was 'too circular to be natural.'")
print()

print(f"'Sir,' Dr. {p2_name} said, passing the food forward. 'Our radar shows their hull armor")
print(f"is impenetrable to nukes, but it dissolves instantly when exposed to the acidic oils")
print(f"of a freshly prepared serving of {p2_fav_food}. We have a chance.'")
print()

print(f"President {p1_name} squared {p1_possessive_pronoun} shoulders, stuffed the remaining scraps of")
print(f"{p1_fav_food} safely into {p1_possessive_pronoun} suit pocket, and grabbed a weaponized handful of {p2_fav_food}.")
print(f"'Let's show these {p2_fav_animal}s how we do things in {p1_hometown},' {p1_pronoun} growled.")
print()

# --- THE DYNAMIC REELECTION CHECK ---
print(f"--- SECURING REELECTION STATUS RECORDS: [ REELECTED = {p1_reelected} ] ---")
time.sleep(1)

if p1_reelected:
    print(f"As a reelected leader, {p1_name} knew {p1_pronoun} had a mandate to protect the planet.")
    print(f"Or at least, a mandate to ensure {p1_guilty_pleasure} survived another four years.")
else:
    print(f"Since {p1_name} was NOT reelected, {p1_name} looked at the chaos and realized:")
    print(f"getting replaced by the opposing party was going to be a massive relief after today.")
print()

print(f"History would forever remember President {p1_name} as {p1_height_inches} inches of unyielding courage,")
print(f"who saved the world on {p1_birthday} using an absolute unit of {p1_fav_food} and sports strategy.")
print(f"History would remember Dr. {p2_name} as the genius who hid the truth since {p2_birthday},")
print(f"wasted time watching {p2_guilty_pleasure}, but brought tactical {p2_fav_food} to a first contact event.")
print(f"Together, their combined age was {p1_age + p2_age}, but their combined survival rate was anyone's guess.")
print()
print("=" * 70)
print("             [END OF TRANSMISSION // DEFCON STATUS CLEAR]")
print("=" * 70)
```