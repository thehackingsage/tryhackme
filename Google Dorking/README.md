Google Dorking | https://tryhackme.com/room/googledorking

### [Task 2] Let's Learn About Crawlers

#1	What is the keyword for the contents that a "Search Engine" stores about a website? : ```index```

#2	What is the name of the technique that "Search Engines" use to retrieve this information about websites? : ```crawling```

#3	What is an example of the type of contents that could be gathered from a website? : ```keywords```

### [Task 3] Enter: Search Engine Optimisation

#1	Using the SEO Site Checkup tool on "tryhackme.com", does TryHackMe pass the “Meta Title Test”? (Yea / Nay) : ```Yea```

#2	Does "tryhackme.com" pass the “Keywords Usage Test?” (Yea / Nay) : ```Nay```

#3	Use https://neilpatel.com/seo-analyzer/ to analyse https://blog.cmnatic.co.uk , What "Page Score" does the Domain receive out of 100? : ```81/100```

#4	With the same tool and domain in Question #3 (previous), How many pages use “flash” : ```0```

#5	From a "rating score" perspective alone, what website would list first? tryhackme.com or blog.cmnatic.co.uk : ```blog.cmnatic.co.uk```

### [Task 4] Beepboop - Robots.txt

#1	Where would "robots.txt" be located on the domain "ablog.com" : ```ablog.com/robots.txt```

#2	If a website was to have a sitemap, where would that be located? : ```/sitemap.xml```

#3	How would we only allow Bingbot to index the website? : ```user-agent :bingbot```

#4	How would we prevent a "Crawler" from indexing the directory "/dont-index-me/"? : ```disallow: /dont-index-me/```

#5	What is another configuration file that we might want to hide from "Crawlers"? : ```.conf```

### [Task 5] Sitemaps

#1	What is the typical file structure of a "Sitemap"? : ```XML```

#2	What real life example can "Sitemaps" be compared to? : ```MAP```

#3	Name the keyword for the path taken for content on a website : ```route```

### [Task 6] What is Google Dorking?

#1	What would be the format used to query the site bbc.co.uk about flood defences : ```site: bbc.co.uk flood defences```

#2	What term would you use to search by file type? : ```filetype:```

#3	What term can we use to look for login pages? : ```intitle: login```
