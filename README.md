<p align="center">
    <img src="https://raw.githubusercontent.com/anish-lakkapragada/Restore/main/logo.jpg" 
    width = 300 height = 300>
</p>

# Restore

Invasive plants are a potent threat to natural environments, ecosystems, and biodiversity. To mitigate this issue and allow anyone to help combat the destruction of our natural environment, we developed this application. The app allows anyone, with real-time live feedback, to accurately detect and identify the top invasive species of plant in the Untied States. With time and effort, together, we can stop the spread of invasive species.

## Inspiration

While we are constantly being told that more greenery and plants are beneficial, we were surprised to hear that some plants (i.e. invasive plants) are in fact detrimental to the environment. Not too long after we learned that this was the case, we saw a demonstration from the Worldwide Developers Conference (WWDC) of flower detection using Apple’s CreateML framework. When we got the idea that AI could potentially detect invasive plants, we were instantly motivated to pursue it. No one, prior to the Restore team, has explored using AI in invasive species detection.

## What it does

As you walk around, our model detects and notifies you if it finds any invasive plants in its camera feed. The 4 invasive plants our model detects for are the Japanese Barberry, Japanese Honeysuckle, Wisteria, and Purple Loosestrife. If the model can’t find any invasive plants in the current frame, it simply outputs “Non Invasive.” We plan to implement the model into an app so that  anybody who cares about the cause can go into the wild and search for invasive plants to remove!

## How we built it

In order to perform machine learning tasks, you need data. Because this problem hasn’t been solved or addressed before by AI, there were no pre-made datasets for us so we had to manually search up invasive plants on Google Images and scrape the results. Not all of the images were of high-quality, so we had to manually curate each of the roughly 5,000 images we collected and delete those that wouldn’t help in training the model. In the end, we ended up with around 2,000 images for training. 

We then used Microsoft’s Lobe platform for us to train a model that could be used later After doing this several times we were able to achieve **88% accuracy** on detecting 4 of the most widespread invasive plants in the US. 

## Challenges we ran into

We ran into a lot of challenges with model training. For instance, because our data was from Google Images it wasn’t of the highest quality, so when we first started training we were at 74% accuracy. However, through more and more manual cleaning of the data, and image augmentations, we were able to reach 74%, 85%, and finally 88% accuracy on detecting invasive species. 

## Accomplishments that we're proud of


We are very proud of the fact that we were able to achieve 88% accuracy on this completely unexplored, novel task of detecting invasive species, with no pre-made datasets. 

## What we learned

We also learnt to be persistent. We first started off at a mere 75% accuracy, but then with a little bit of patience we decided to manually take 2 hours to clean up our data which eventually led to 91% accuracy. We were unsure in those 2 hours whether our hard work would pay off, and we learned at the end that if you want something to work its best to believe that it will work. 

We also got a rude awakening that it really is true that 80% of your time is found on finding data, good data, and only 20% of the time is found on your model. This gave us more insight into what it would be like to be a real data scientist in today’s messy world. 

## What's next for Restore

Restore has a lot of things that can be done going forward. One thing we plan to look at is increasing the number of invasive plants Restore can detect and also making an app so our model can be used by anyone who wants to remove invasive plants. 





