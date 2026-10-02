---
layout: page
title: "Assignment 1: Mapping Features of Bahrain"
description: "An interactive GeoNames map and analysis of selected geographic features in Bahrain."
---

# Mapping Features of Bahrain

## Introduction

For this assignment, I chose Bahrain as the country to study using the GeoNames dataset. Bahrain is a small country, but it has many different kinds of places and features. It has cities, villages, islands, hotels, roads, an airport, and many other places. I thought Bahrain would be interesting to map because it is small enough to see patterns clearly, but it still has both physical and human features.

The goal of this project was not only to make a map. I also wanted to understand what kind of information GeoNames has about Bahrain and whether that information gives a complete picture of the country.

For my map, I chose four GeoNames feature codes: **PPL**, **ISL**, **HTL**, and **AIRP**. These stand for populated places, islands, hotels, and airports. GeoNames defines PPL as a populated place where people live and work, HTL as a hotel, and AIRP as an airport with facilities for passengers and cargo. The feature codes make it possible to separate the data into different groups and compare them. 

I chose these four features because together they show different parts of Bahrain. Populated places show where people live. Islands show the physical shape of the country. Hotels show tourism and business activity. The airport shows an important part of Bahrain's transport system.

## What GeoNames Shows About Bahrain

GeoNames gives different types of information for each place. The data can include the place name, latitude, longitude, feature code, population, elevation, and timezone.

When I started looking at the Bahrain data, I noticed that the information was not complete for every location. Some places had useful information, while others had many missing values.

For example, some populated places have a population number. Al Muharraq, Hamad Town, Riffa, Sitrah, and Jidd Hafs are examples of places with population values in the dataset. However, many other populated places show `N/A` for population. Elevation is also often shown as `Unknown`.

This was important because at first the dataset looked very detailed. There were many rows, names, and coordinates. However, after looking more closely, I saw that having many records does not mean that every record is complete.

This connects to an important idea from Kitchin and Lauriault. They explain that data should not be treated as simple facts that exist naturally. Data are created through people, systems, rules, categories, technology, and organizations. They argue that data are not fully neutral or "raw." They are shaped by the way they are collected and organized.

This idea helped me understand GeoNames differently. The database is useful, but it is still made through choices. Someone has to decide which places are included, what they are called, which feature code they receive, and what information is added.

## The Four Features I Chose

The first feature I chose was **PPL**, which means populated place. I chose this because I wanted to see where people live in Bahrain.

The populated places are mostly grouped in the northern and central parts of the country. There are many points around Manama, Muharraq, and nearby towns and villages. There are fewer populated-place points in the far south.

This gives a clear picture of where much of Bahrain's settlement is located.

The second feature was **ISL**, which means island. This was important because Bahrain is made up of more than one island. The dataset includes the main island of Bahrain, Muharraq Island, Sitrah, Hawar Island, Amwaj Islands, Umm an Nasan, and several smaller islands.

This layer changes the way Bahrain looks on the map. If I only look at populated places, I mainly see the urban north. When I turn on the island layer, I see that Bahrain also spreads across the sea and includes many smaller islands.

The third feature was **HTL**, or hotels. I chose hotels because they can show where tourism and business activity are located.

The hotel data creates one of the clearest patterns in the whole map. Most hotel points are strongly grouped around Manama and nearby areas such as Seef and Juffair. There are also hotels in Muharraq, Amwaj, and Zallaq.

This can be seen clearly in Figure 2.

### Figure 1: All Four GeoNames Features

![Overview of Bahrain showing populated places, islands, hotels, and airport]({{ '/assets/images/bahrain all features.png' | relative_url }})

*Figure 1. Bahrain with PPL, ISL, HTL, and AIRP layers turned on.*

The fourth feature was **AIRP**, which means airport. The selected data contains Bahrain International Airport. It is located on Muharraq Island.

The airport is close to many hotels and populated places. This makes sense because Bahrain International Airport is close to Manama and other major urban areas.

## Hotel Distribution

When I turned off the other layers and looked only at hotels, the pattern became much easier to see.

### Figure 2: Hotel Locations

![Hotel locations in northern Bahrain]({{ '/assets/images/bahrain hotel.png' | relative_url }})

*Figure 2. Hotels are strongly grouped around Manama, Seef, Juffair, and nearby areas.*

Most of the hotel points are in northern Bahrain. There are many around Manama and Juffair, as well as Seef and areas near Muharraq.

This shows how changing the layers can change what we notice. When all four layers are turned on, there are many points on top of each other. When only hotels are shown, the concentration becomes much clearer.

However, I also noticed that some hotel records appear more than once under slightly different names. For example, there are several similar versions of the same hotel names. This may mean that the dataset contains duplicates, older names, or slightly different records for the same place.

This is another reason why we should not automatically assume that every point on a map represents a completely different place.

## A Data Problem I Found

One of the most interesting things I found was a possible mistake in the data.

In Figure 1, Bahrain appears very small because the map is zoomed out and shows a large part of Saudi Arabia and Qatar. When I looked at the GeoNames points, I found that one PPL record has a longitude of `40`.

Bahrain is around longitude 50 degrees east, so a longitude of 40 places that point far west of the country.

Because the map automatically tries to include the data points, this one unusual record affects the full view of the map.

This is a good example of why checking data is important. If I only looked at the map and did not look at the records, I might not know why the map was showing such a large area.

It also shows that even a large geographic database can contain mistakes.

## Interactive Map

The interactive version of my map is below. The four layers can be turned on and off. Clicking on a point shows information such as the name, feature code, population, elevation, and timezone.

<iframe
  src="{{ '/BH_featuremapNEW.html' | relative_url }}"
  width="100%"
  height="600"
  style="border:0;"
  loading="lazy">
</iframe>

The map uses the Thunderforest Outdoors basemap. It also includes a legend, layer controls, and a metric scale bar.

## Do Maps Lie?

The **Do Maps Lie?** video explains that maps can influence the way people understand a place. Maps may use real data but still give different messages depending on how the information is chosen and shown.

One example in the video compares two maps of London house prices. One map uses equal price groups, while another compares London's prices with the UK average. The same general topic can look different because the data are grouped and shown differently.

The video also suggests asking three questions when looking at a map: **Who made it? Why did they make it? What does it tell us?** 

These questions also apply to my Bahrain map.

I made the map for this assignment, and I chose only four types of features. This means the map shows Bahrain through my choices.

For example, when the hotel layer is turned on, hotels become a major part of the map because there are so many hotel records. Someone looking at the map could think that hotels are one of the most important parts of Bahrain.

However, that is partly because I chose hotels as one of the four categories.

There are many things that are not shown on my map, such as schools, hospitals, mosques, malls, historical sites, factories, and roads.

So my map does not show the full reality of Bahrain.

This does not mean the map is false. It means that every map is selective. A map always includes some things and leaves out others.

The colors also affect what people notice. Each feature code has its own color. Because the hotel layer contains so many points, it can easily become the strongest visual part of the map.

The video helped me understand that a map should not be treated as a perfect copy of reality. We should always think about the choices made by the person who created it.

## Critical Data Studies

Kitchin and Lauriault make a similar argument about data.

They explain that data are often treated as if they are neutral and objective. However, they argue that data are shaped by the systems and people that create them.

They use the idea of a **data assemblage**. A data assemblage is not just a dataset. It also includes the technology, organizations, people, rules, standards, and systems involved in creating and using the data.

GeoNames can be understood in this way.

The Bahrain dataset did not appear by itself. People and systems had to collect place names, add coordinates, choose feature codes, add population values, and update the records.

The problems I found show this clearly.

Some population values are missing. Many elevations are unknown. Some hotels appear more than once. One populated-place coordinate appears far outside Bahrain.

These problems show that data are created and edited over time.

Kitchin and Lauriault also explain that databases affect what questions we can ask and how we understand the world.

This is clear in my project. GeoNames lets me ask questions such as where hotels are located or where populated places are grouped. But the answers depend on what GeoNames has recorded.

If some places are missing, duplicated, or incorrect, the map will also show those problems.

## Conclusion

This assignment helped me understand both Bahrain and geographic data in a new way.

The four feature types showed different patterns. Populated places and hotels are mostly grouped in northern Bahrain. Islands show that Bahrain is made up of many separate pieces of land. Bahrain International Airport is located on Muharraq Island close to major urban areas.

The project also showed some problems in the dataset. Many records are missing population or elevation values. Some hotel names seem to be repeated. I also found a coordinate that appears to be outside Bahrain and affects the way the full map is displayed.

The most important thing I learned is that a map is not simply a picture of reality.

The **Do Maps Lie?** video shows that the choices made by a mapmaker can change the message of a map. Kitchin and Lauriault also explain that data are created through people, systems, rules, and technology rather than simply existing as neutral facts.

Because of this, we should not only ask what a map shows. We should also ask where the data came from, what might be missing, and what choices were made when the map was created.

## Generative AI Statement

I used ChatGPT to help me with organizing the layout and design of the website and helping me with the codes.
