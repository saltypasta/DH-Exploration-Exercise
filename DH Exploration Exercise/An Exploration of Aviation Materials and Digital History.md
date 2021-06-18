# Contextualizing

The data used in this document has been taken from Ingenium Canada (Source: https://ingeniumcanada.org/collection-research/artifact-open-data-set-mash-up), and includes all artifacts from the Canada Agriculture and Food Museum, Canada Aviation and Space Museum, and Canada Science and Technology Museum. Although there are thousands of artifacts within this dataset it is important to consider that these were curated for their historical significance, and they are not a representative sample of all the artifacts from their respective periods. The omission of some artifacts may have significance in itself, and may influence the patterns visible within the data. For this reason, the following analysis is within the context of artifacts curated by the aforementioned museums and is not representative of the collections of other institutions.   

# Wrangling

# Excel

The data was loaded into Excel through a .Csv file, which generated a table. Each column represented the appropriate metadata of each historical artifact held by all three museums. Excel tables are very powerful as they allow for the data to be sorted easily by any of the metadata. Additionally, Excel can be used to generate charts and graphs to depict trends or patterns in the data selected. In this case, the data was sorted in excel by the category "Aviation" and then organized chronologically. After hiding the irrelevant columns, here is the resulting table:

![Condensed Excel Table](sorted Excel table ex.JPG)

There are several entries in this table that are missing metadata such as the year the artifacts originate from, or the materials they are composed of. Additionally, some pieces of the metadata were added within the same cell. This restricts the ability to sort the table by these terms without extracting them and categorizing each artifact appropriately. I am not aware of a way to do this within Excel, however it may be possible. This would also open up new ways to categorize the data and potentially new insights.

#Voyant

The data was then loaded into Voyant, once including the partial entries and then again omitting the partial entries. The entries without dates were not omitted in Chart A, and they were omitted in chart B.

![Chart A](Chart A.PNG)

![Chart B](Chart B.JPG)

After examining both charts, there is an obvious difference between omitting and not omitting the partial entries. One drastic difference is the increase in the relative frequency of "metal" in chart A versus chart B. If one was not aware of the partial entries, it would appear as though there is a drastic increase in metal artifacts in the 21st century. Upon closer examination, all non-dated entries were included at the end of the data after the most recent artifact. Chart B reflects the difference that omitting these entries makes on the graph. There are a few interesting trends visible in chart B. Around the year 1940, there is a large increase in the relative frequency of paper in the materials composing these artifacts. returning to the excel chart we can see that there are a significant quantity of maps and uniforms that are from this period. One might make the assumption that a selection of maps and uniforms are consistent with the use of fighter planes in the second world war. An equally plausible explanation might be that the increase in the artifacts selected is consistent with an increase in domestic flights during this period. Matthew Lincoln states the following in his piece titled *Confabulation in the humanities*: "we are particularly susceptible to confabulating these post-facto rationalizations with the idea that we somehow knew the results of this quantitative work already" (Lincoln 2015). By digging deeper into the metadata and examining the individual artifacts, it becomes clear that these maps are curated due to their significance to aviation in the second world war. Although this seems trivial, as Lincoln says it is worth our time to run experiments and analysis to confirm or contrast the narratives that we fabricate as historians.

#Antconc

Antconc is a powerful text analysis tool that allows us to make comparisons on a large scale. Antconc reads text files in the form of a "Corpus" and then allows the user to search for key terms. After running a search Antconc displays Concordance, a Concordance Plot, Collocates, a word list, and a keyword list. These can be used to find statistical relationships between words within the corpus. Using the data from the Excel spreadsheet, I searched the corpus for the term "suit" and then navigated to the "clusters/N-Grams" tab. The results are shown here:

![Antconc Suit Clusters](Antconc A.JPG)

Looking at the clusters, we can observe that the materials used in flight suits changed from natural materials such as wool, leather and cotton in the early 20th century to more Synthetic materials such as nylon, rubber and plastic. We could have observed this within the excel table as well, however Antconc allows for another powerful comparison. Antconc allows for multiple Corpora to be loaded and compared against one another. If we wanted to observe how this trend may compare to suits or other garments beyond the category of aviation, we can generate a new text file with this data and load it into Antconc.

#Storymaps

Storymaps is a tool that allows for slides to be pinned to a map to visualize the geographical aspect of a story. Using our data from the aforementioned museums, we can plot artifacts of interest to their geographical origin. This does not give an analysis of the quantity of artifacts per location, but rather serves to spark an interest in specific artifacts that are historically significant in an easily digestible format. The following is a story map generated from several artifacts I found interesting within the data.

<iframe src="https://uploads.knightlab.com/storymapjs/9a41b307b4ac7ce95adc10d60d389033/digital-history-exploration-exercise/index.html" frameborder="0" width="100%" height="800"></iframe>

Storymaps allows the viewer to appreciate the geographical aspect of the information presented, as well as the visual characteristics if one chooses to include images.


# What does this all mean?

Understanding context and how our manipulation of data can effect our analysis is absolutely critical. In a [twitter thread](https://twitter.com/amaliasl/status/1245544256212807680) Amalia S. Levi discussed gaps in digital archives and what they mean. She explains that gaps exist because digitization is selective. Sometimes archivists decide something is not relevant or important to include. As digital historians we will also be selective with our inclusion or exclusion of information during our analysis, and it is our responsibility to consider what these "gaps" mean. In some cases, an omission is a wise way to prevent skewing data in an unrealistic way. For example, we could see in Voyant how uncategorized data skewed the relative frequency curves for artifact materials. Although we omitted these entries, it is important to ask why those entries may be incomplete. Additionally, if they were to be appropriately categorized how might that effect the visible trends?

Questioning digital silences and supposedly "known" historical narratives are where digital historians can make meaningful insights. In addition to questioning digital silences, Digital Historians must question the origins of trends within the data they analyze. For example, Marie Hicks discusses a study by Laura Downs on British auto workers in her book *Programmed Inequality*. The study found "that the car manufacturer Rover classified women's work as "unskilled" despite its skilled nature by dividing work by gender...Management used the gendered organization of the work to construct a hierarchy of labor with women's work at the bottom" (Hicks 2018). In this case the data may show that women make up the large majority of unskilled labor within this industry, however that does not mean that the labor was unskilled. By understanding the context of this trend it becomes evident that a greater divide in gendered labor is indicative of a systemic oppression, and not of the values or capabilities of individual women.

Using the many tools Digital Historians have at their disposal allows for easy alternation between Micro and Macro perspectives of historical data. Digital Historians have the unique ability to analyze large amounts of data while maintaining the ability to contextualize trends on an individual level. Furthermore these insights can be used in academia to argue for or against supposedly established narratives; or they can be formatted into more digestible mediums for the public. As the paper *Digital History and Argument* by Stephen Robertson and Lincoln Mullen states "the digital medium permits engagement with public audiences outside of more traditional venues for public history".

Though Aviation materials and artifacts might not be groundbreaking research material for everyone, it serves to demonstrate that there is historical value in some of the most trivial things. By briefly playing with the data available on these artifacts, several valuable questions come to mind. Why was there a shift in the materials used in flight suits? did this correlate with any technological breakthroughs in other fields beyond aviation? Why is it that in the 1960s the relative frequencies of the terms "metal" and "Synthetic" appear to have an inverse relationship? Does this relate to the method of curation of these artifacts or technological changes? These types of questions combined with an understanding of why Digital History matters is what allows Digital Historians to make profound contributions to their field, and the world.
