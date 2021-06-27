<p align="center">
    <img src="https://raw.githubusercontent.com/anish-lakkapragada/Restore/main/logo.jpg" 
    width = 300 height = 300>
</p>

# Restore

Invasive plants are a potent threat to natural environments, ecosystems, and biodiversity. To mitigate this issue and allow anyone to help combat the destruction of our natural environment, we developed this application. The app allows anyone, with real-time live feedback, to accurately detect and identify the top invasive species of plant in the Untied States. With time and effort, together, we can stop the spread of invasive species.

## Inspiration

While we are constantly being told that more greenery and plants are beneficial, we were surprised to hear that some plants (i.e. invasive plants) are actually detrimental to the environment. Not too long after that we learned that this was the case, we saw a demonstration at the Worldwide Developers Conference (WWDC) of flower detection using Apple’s CreateML framework. When we got the idea that AI could potentially detect invasive plants, we were instantly motivated to pursue it. No one, prior to the Restore team, has explored using AI in invasive species detection.

## What it does

## How we built it

In order to perform machine learning tasks, you need data. Because this problem hasn’t been solved or addressed before by AI, there were no pre-made datasets for us so we had to manually search up invasive plants on Google Images and scrape the results. Not all of the images were good or nice data, so we had to manually go through each of the about 5,000 images we collected and delete those that wouldn’t help in training the model. In the end, we ended up with around 2,000 images for training. 

We then used Apple’s CreateML format for us to train a model that could be used later in our app for iOS development. After doing this several times and experimenting with image augmentations we were able to achieve **91.4% validation accuracy** on detecting 4 of the most widespread invasive plants in the US. 

## Challenges we ran into

We were both fairly fluent in machine learning, but none of us ever had much experience at all with using Swift, CreateML, and CoreML to create iOS apps. We extensively relied on tutorials and web searches in order to figure out how we could create a real-time detection system that could take in an image, send a request to the model we created, and then show the predictions to the user. However, because most of these tutorials were old, they wouldn’t work with our current setup so we actually needed to create a virtual machine using Virtual Box to download a lower version of XCode to create our app!

We also ran into some challenges with model training. For instance, because our data was from Google Images it wasn’t of the highest quality, so when we first started training we were at 74% accuracy. However, through more and more manual cleaning of the data, and image augmentations, we were able to reach 84%, 87%, and eventually 91% with the CreateML platform. 

## Accomplishments that we're proud of

We are very proud of the fact that we were able to create a full-fledged app in Swift that can detect invasive species despite not knowing much Swift prior of Citro Hacks. We’re also super pumped about the fact that we have reached 91.4% accuracy in our dataset. 

## What we learned

We learned that in fast, deadlined environments like hackathons, you have to be okay with using duct tape solutions. When none of the tutorials for building models with XCode worked because they were older and not up-to-date with XCode12, we decided to take a very convoluted approach - we created a virtual machine to then download a later version of XCode so we could create our app with help from the tutorials. 

We also learnt to be persistent. We first started off at a mere 75% accuracy, but then with a little bit of patience we decided to manually take 2 hours to clean up our data which eventually led to 91% accuracy. We were unsure in those 2 hours whether our hard work would pay off, and we learnt at the end that if you want something to work its best to believe that it will work. 

## What's next for Restore

Restore has a lot of things that can be done going forward. One thing we plan to look at is increasing the number of invasive plants Restore can detect and also making Restore also work on Android and other non-iOS platforms. 



