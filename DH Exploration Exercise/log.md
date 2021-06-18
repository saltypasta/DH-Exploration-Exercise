# Step one: Get some Data

- Im going to use the data set from ingenium which includes artifacts from:
  - Canada Agriculture and Food Museum
  - Canada Aviation and Space Museum
  - Canada Science and Technology Museum
- Mostly because I go to these places and I think it would be cool to have some "big picture" insights in mind the next time I visit. Maybe it will add some value to the experience
- I downloaded the .csv File and imported it through Excel, just like in Part 2 of the class
- This is gorgeous.
- Fun fact: one of the oldest artifacts in this data is a "Plumb bob" estimated date back to the 12th century

# Step 2: Wrangling the data

- Sorting the data by Group. I will include all artifacts that are related to aviation and exclude all other categories
- Sorted by category to exclude archives, commemorative, models and services. Did this because I am interested in the change in materials used in aviation artifacts over time
- Going to try and make a graph depicting the change in materials used over time
  - Oh boy excel crashed, maybe I should google how to make this chart properly
  - When I load the data I want into a chart it works fine, but if I try and adjust where that data appears within the chart it seems to be a little too much for it to process
  - Ill google and figure out how to load everything in exactly where I want it so I can keep my meddling to a minimum
  - So there are other tools I could use but a simpler way is to isolate the data I care about for the chart I want to make and duplicate it on another work sheet, then ask excel to make a chart from that data instead of everything
  - Okay so I want to compare the materials used in the artifacts over time, however there are multiple materials used in artifacts and these are all stored in the same cell. Maybe I can use a count if function? That would only give me a number of instances of the material without being bound to the date in which it occurs...
  - Maybe using this in voyant would be better for now, as it will just count all the words?
  - Pasted the date and Material columns from my excel document into voyant. I probably could have saved this data as a csv or something Voyant can read but the paste is working so i will leave it.
  - Interesting: Metal and Synthetic are the most frequent terms in my corpus. In the relative frequency diagram, they look like they have an inverse relationship for a decent length of time.
  - Omit incomplete entries and run it through voyant again

- Made another sheet in excel that includes the artifact name, date, and material
  - Tried to paste this text into a text file to use with Antconc, however I got a bunch of junk from excel
  - used a formula (A1 & B1 & C1) to combine the text within the three cells into the D column, then copied this to Antconc
  - Since excel combined the text together with no spaces, when I search in antconc I need to place * where appropriate to allow it to find my keywords that are bunched together
  - There may be a way to adjust the formula I used to automatically add spaces but this is a *sketch* so it will do for now

- Used storymaps to make a quick presentation featuring artifacts I found Interesting
  - Storymaps didnt like the links for the images provided by ingenium so I downloaded them individually and uploaded them to each respective slide
