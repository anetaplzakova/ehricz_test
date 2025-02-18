---
title: MemoMap | Interactive Holocaust History 
layout: training
type: training
date: 2024-09-09
---

{{< intro >}}
The MemoMap project allows you to study the history of the Holocaust through urban spaces and sites of persecution. The name is based on the term memory map, i.e. a map that connects myriad information about people in history and the places where persecutions took place.
It’s one of several projects that load information about the Holocaust into a map. MemoMaps strive to use extremely vast datasets, including databases of victims, digitized documents from public and private archives, historic maps, and different contextual information. 
Our MemoMap of Prague is currently available and we’re working on a similar application for the town of Pacov. We hope to add other locations and additional functions in the coming years.
{{< /intro >}}

[Enter the app.](http://www.memomap.cz)
[More about MemoMap Prague](/services/memomap/prague/)


{{< figure src="/images/memomap.png" class="fig-float fig-right" >}}


### MemoMaps and spatial arrangement
The MemoMaps project was inspired by the research on geographic information systems (GIS) and the latest advances in geography and cartography, such as critical approaches in the social construction of spaces. We now know that space isn’t merely determined by coordinates and measurable distances, but it’s equally made up of people’s everyday encounters, actions, and ideas. Maps and spatial policies are instruments of power that can create social hierarchies, or, in this case, lead to the exclusion and persecution of a group of people labelled as racially “other.”

We realize that not everything can be expressed in geographic coordinates and displayed on a regular map using points, lines, and other geometric shapes. What people feel about a particular space and place, as well as events associated with certain locations—often things that can’t be determined—are extremely important. This is why we’re supplementing the approaches used in geographic information systems with historical documents and additional information, and thinking about ways to connect victim narratives with various types of interactive non-geometric data.

Spatial arrangement is a complex historical subject. MemoMaps intelligently interact with the contemporary public space and help researchers think about the mechanisms of social inclusion and exclusion in everyday life. Using the application not only makes users more knowledgeable, but it also makes them perceive places and spaces more clearly. To achieve this goal and even go beyond what similar apps offer, the project prioritizes data that enrich our spatial experience and awareness of shared spaces.

### Who can use MemoMaps? 
Anybody. Our philosophy is that anyone can be a researcher. Academics as well as the public at large are free to use them. The MemoMaps application is adapted to mobile devices, allowing users to access them as they walk through urban spaces and stop by important sites of commemoration.

They help researchers formulate new questions about the history of the Holocaust (for instance on the process of social exclusion, spatial segregation, or forms of resistance by the persecuted), use statistics, and work directly with most datasets stored in MemoMaps, primarily through the EHRI Geospatial Repository (see below).

The maps help both students and residents to research the history of the Holocaust in the places where they live, work, or frequently spend their time. For victims' families, they can supplement the already known information published in Terezín memoirs and in the database of victims about where they were located in the city. 

You can also use the application as an educational tool to teach about human rights, the Holocaust, or the history of racism and antisemitism. It supports modern approaches to teaching history and other subjects that encourage students to research independently and offers an interactive platform for work in the public space. 

By including personal accounts, photographs, and documents, it complements the study of “big history” by adding microhistory methods.

For tourists, it’s another way of exploring historic sites as it significantly expands existing museum exhibits and memorials.

### The software
The user interface of MemoMaps is the result of the feedback and data acquired from testing the mobile application and the temporary web hosted on the QGIS server. The brand-new software allows us to easily modify the user interface, include a timeline, and offer the full-text search of names and addresses.

From its very inception, the new MemoMap has been optimized for mobile devices. Its code is based on opensource libraries and tools (ASP.NET Core, Blazor WASM). Users can run this responsive web application on computer browsers and both Android and iOS operating systems. Due to the large number of entries and documents, and to keep everything up-to-date, the application requires a permanent internet connection.

The project supports maximum openness and duplicability. The code of the application is available for free on Github and you can use it to develop other projects.

With the exception of information subject to personal data protection, the data used in MemoMaps is also available in the EHRI Geospatial Repository. You can therefore work with it in any GIS software or in any other way.

### About the project
The MemoMap application was created by [the Masaryk Institute and Archives of the Czech Academy of Science](https://www.mua.cas.cz/en) as a service of the Czech national node of the European Holocaust Research Infrastructure (EHRI), which is part of the LINDAT/CLARIAH-CZ infrastructure that is fully supported by the Czech Ministry of Education, Youth, and Sports as part of their large research infrastructure program. The preparation of the data and the creation of the new software was also made possible thanks to the support of the Foundation for Holocaust Victims and the Strategy AV21 program [City as Laboratory of Change.](https://strategie.avcr.cz/en/programy/mesto)

The new app is based on the MemoGIS Prague application that was the result of the Integration and Segregation in Cityspace: The History of the Holocaust in Prague Through a Web Application project (identifier TL01000366), which was supported by [the Technology Agency of the Czech Republic](https://www.tacr.cz/en/) as part of the public tender ÉTA 1. The Masaryk Institute and Archives developed the original MemoGIS application together with [the Terezín Initiative Institute](http://www.terezinstudies.cz/en) and [Multicultural Center Prague.](https://mkc.cz/en/about)
